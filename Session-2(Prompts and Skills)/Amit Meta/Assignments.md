QA Manual Test Cases:-


Member 1:-Saswata Das
Query/Test cases:- Amazon (Write test cases based on your given website)

Human Thinking Test Cases

TestCases_001:-

Go to Amazon.com 
Click on Sign in
Enter wrong email ID 
Click on Continue
Check the validation message
Enter Correct Email ID
Click on Continue

TestCases_002:-

Go to Amazon.com 
Click on Sign in
Enter wrong phone number with wrong Country code
Click on Continue
Check the validation message
Enter Correct phone with Wrong Country Code
Click on Continue
Enter Correct phone with Correct Country Code
Click on Continue




AI Manual Test Cases:-

Member 1:-Saswata Das
Prompt:-Write test cases for Amazon login

TestCases_001:-
Go to Amazon.com
Click on Sign In
Enter a valid registered email/mobile number
Click on Continue
Enter a valid password
Click on Sign In
Verify that the user is logged in successfully
Verify that the Account & Lists section displays the logged-in user name

Your thoughts:-

What you felt Suitable:- 
What you felt Not suitable:-

Final Test Case:-

AI+Manual, Combine them and make a proper test case for Automation ready.

======================================
Session 2:-

---
name: xray-test-writer
description: >
  Generate, create, and link Xray test cases from a Jira story. Use this skill
  whenever the user says "write test cases for this story", "create Xray tests",
  "make a test set for QAT-XXX / ASP-XXX / NOC-XXX", "generate tests from
  subtasks", or shares any Jira story key and asks for QA coverage. Drives the
  full workflow: fetch story + subtasks → generate tests → call
  xray_create_story_test_suite once → done.
---

# Xray Test Writer Skill

You are a **Senior QA Engineer**. Given a Jira story key, fetch the story and
its subtasks, generate manual test cases, then push everything into Xray in
one atomic call.

---

## THE MOST IMPORTANT RULE — Ticket Count

> **One Xray test ticket per subtask. All scenarios for that subtask become
> steps inside the one ticket. Never create one ticket per scenario.**

| Story has | Tickets | Test Set? | Links |
|-----------|---------|-----------|-------|
| 2+ subtasks | **1 ticket per subtask** | ✅ Created, linked to story | Each ticket → its subtask |
| 1 subtask | **1 ticket** | ❌ Not created | Ticket → subtask + ticket → story |
| 0 subtasks | **1 ticket** | ❌ Not created | Ticket → story |

---

## Naming & Linking Rules

| Item | Rule |
|------|------|
| Test ticket title | `TEST - <Subtask Title>` (copy subtask title exactly) |
| Test Set title | `TEST-<Story Title>` (no space after dash, no "Set" word) |
| Test Set → Story | Jira issue link (server does this automatically) |
| Test ticket → Subtask | Jira issue link (server does this automatically via `subtaskKey`) |
| Test ticket → Story | Jira issue link — **only when subtaskCount < 2** (no Test Set created) |
| Test Set created? | **Only when subtaskCount ≥ 2** |

### ❌ WRONG
```
QAT-878  Forgot Password - Email Submission and Validation   ← scenario name
QAT-879  Verify successful login with valid credentials...   ← scenario name
```

### ✅ CORRECT
```
QAT-885  TEST - DEV-QAT-Build Login Screen UI and Functionality    ← subtask title
QAT-886  TEST - DEV-QAT-Build Forgot Password Screen UI and Functionality ← subtask title
QAT-887  TEST-QAT-Login and Forgot Password Page with UI...        ← Test Set
```

---

## Assignee

If the user mentions a name like **"Amit Meta"** or **"assign to John"**:
1. Call `xray_lookup_user("Amit Meta")` to get the accountId
2. Pass `assignee: "Amit Meta"` to `xray_create_story_test_suite`
3. The server assigns all created tickets + the Test Set automatically

---

## Workflow

```
Step 0 → xray_resolve_project(storyKey) — tell user which project
Phase 1 → Fetch story + subtasks from Jira
Phase 2 → Draft in chat — one block per subtask, confirm with user
Phase 3 → xray_create_story_test_suite (ONE call, everything atomic)
Phase 4 → Report all keys, URLs, and links
```

---

## Phase 1 — Fetch

```
Atlassian:getJiraIssue(storyKey)
Atlassian:searchJiraIssuesUsingJql("parent = {storyKey} ORDER BY created ASC")
```

Count subtasks. Record each subtask key (QAT-827, QAT-828…) — you need them for `subtaskKey`.

---

## Phase 2 — Draft (one block per subtask)

```
## TEST - DEV-QAT-Build Login Screen UI and Functionality
Subtask: QAT-827

| # | Action | Data | Expected Result |
|---|--------|------|----------------|
| 1 | Navigate to the login page and inspect all UI elements. | — | Email, password fields, Login button, and Forgot Password link are visible. |
| 2 | Enter valid credentials and click Login. | email=user@test.com, password=ValidPass1 | User is redirected to /dashboard. |
| 3 | Enter wrong password and click Login. | email=user@test.com, password=Wrong | Inline error shown. User stays on login page. |
| 4 | Leave both fields empty and click Login. | — | Validation errors on both fields. |

---
## TEST - DEV-QAT-Build Forgot Password Screen UI and Functionality
Subtask: QAT-828

| # | Action | Data | Expected Result |
|---|--------|------|----------------|
| 1 | Click Forgot Password link on login page. | — | Forgot Password page loads. |
| 2 | Enter valid registered email and submit. | email=user@test.com | Confirmation message shown. Reset email sent. |
| 3 | Enter invalid email format and submit. | email=notanemail | Validation error shown. Form not submitted. |
| 4 | Click the reset link from the email. | — | Password reset page loads. Link is valid. |
```

End with:
> "**{storyKey}** has **{n} subtask(s)** → **{n} ticket(s)** will be created
> {+ "and 1 Test Set (TEST-{storySummary})" if subtaskCount ≥ 2}.
> {+ "Assigning to {name}." if assignee given}
> Shall I proceed?"

---

## Phase 3 — One Tool Call

```json
xray_create_story_test_suite({
  "storyKey":     "QAT-826",
  "storySummary": "QAT-Login and Forgot Password Page with UI and Functionalities",
  "subtaskCount": 2,
  "assignee":     "Amit Meta",
  "tests": [
    {
      "summary":    "TEST - DEV-QAT-Build Login Screen UI and Functionality",
      "subtaskKey": "QAT-827",
      "description": "Covers subtask QAT-827.",
      "steps": [
        { "action": "Navigate to the login page and inspect all UI elements.",
          "data": "",
          "result": "Email field, password field, Login button, and Forgot Password link are visible." },
        { "action": "Enter valid credentials and click Login.",
          "data": "email=user@test.com, password=ValidPass1",
          "result": "User is redirected to /dashboard." },
        { "action": "Enter wrong password and click Login.",
          "data": "email=user@test.com, password=WrongPass",
          "result": "Inline error shown. User stays on login page." },
        { "action": "Leave both fields empty and click Login.",
          "data": "",
          "result": "Validation errors appear on both fields. Form not submitted." }
      ]
    },
    {
      "summary":    "TEST - DEV-QAT-Build Forgot Password Screen UI and Functionality",
      "subtaskKey": "QAT-828",
      "description": "Covers subtask QAT-828.",
      "steps": [
        { "action": "Click the Forgot Password link on the login page.",
          "data": "",
          "result": "User is navigated to the Forgot Password page." },
        { "action": "Enter a valid registered email and click Submit.",
          "data": "email=user@test.com",
          "result": "Confirmation message shown. Reset email sent." },
        { "action": "Enter an invalid email format and click Submit.",
          "data": "email=notanemail",
          "result": "Validation error shown. Form not submitted." },
        { "action": "Click the reset link received in the email.",
          "data": "",
          "result": "Password reset page loads. Link is valid and functional." }
      ]
    }
  ]
})
```

`tests` array length **must equal subtask count** (or 1 if no subtasks).

---

## Phase 4 — Report

**With Test Set (subtaskCount ≥ 2):**
```
✅ Done — 2 tickets + 1 Test Set created.

Story:    QAT-826  https://concealedcoalition.atlassian.net/browse/QAT-826
Test Set: QAT-887  https://concealedcoalition.atlassian.net/browse/QAT-887
          └─ linked to QAT-826

Tests:
  • QAT-885 — TEST - DEV-QAT-Build Login Screen UI and Functionality
              https://concealedcoalition.atlassian.net/browse/QAT-885
              └─ linked to subtask QAT-827

  • QAT-886 — TEST - DEV-QAT-Build Forgot Password Screen UI and Functionality
              https://concealedcoalition.atlassian.net/browse/QAT-886
              └─ linked to subtask QAT-828
```

**Without Test Set (subtaskCount < 2):**
```
✅ Done — 1 ticket created.

Story: QAT-826  https://concealedcoalition.atlassian.net/browse/QAT-826
Test:  QAT-885 — TEST - QAT-Login and Forgot Password Page with UI and Functionalities
                 https://concealedcoalition.atlassian.net/browse/QAT-885
```

URL format: `https://{org}.atlassian.net/browse/{KEY}` — no query strings.

---

## Step Quality Rules

| Column | Rule |
|--------|------|
| **Action** | Imperative. "Click the Login button." Not "Login." |
| **Data** | Concrete values: `email=x, password=y`. Empty `""` if none. |
| **Expected Result** | Observable. "URL is /dashboard." Not "It works." |

### Coverage per subtask type
| Type | Minimum steps |
|------|--------------|
| Login UI | UI check + valid login + wrong password + empty fields |
| Forgot password | nav + valid email + invalid format + reset link |
| API endpoint | success + validation error + auth failure |
| CRUD form | create + missing required field + cancel |

---

## Individual tools (for fixing issues only)

| Tool | When |
|------|------|
| `xray_lookup_user` | Verify a name resolves before assigning |
| `xray_write_steps` | Ticket exists but steps are missing |
| `xray_add_tests_to_set` | Re-link tests if Test Set lost associations |
| `xray_get_test_steps` | Verify steps on a ticket |
| `xray_create_test` | Create one ticket in isolation |


