****QA Manual Test Cases
Project: DemoBlaze Testing Application: https://www.demoblaze.com/ 
Tester: Bisakha Pati**

**Human Thinking Test Cases**

## MODULE 1 — HOME
=====================================================================

TestCases_001:- Home page
1.Open https://www.demoblaze.com/
2.Verify by default it lands on the "Home" page.
3.Verify all the menus are there — Home, Contact, About us, Cart, Log in, 4.Sign up — and each one is clickable.
5.Verify the category filters — Phones, Laptops, Monitors — and after 6.clicking any filter it shows only that type of product.
7.Verify the carousel slides and Next/Previous work and images load fine.
8.Pick any product, open it, and verify the details page shows the correct image, price and description with an "Add to cart" button.
9.Add it to cart, verify the "Product added." message, and check it actually shows up in the Cart.
10.Click the logo and verify it brings you back to Home.

=====================================================================
## MODULE 2 — LOGIN
=====================================================================

TestCases_002:- Login
1.Click on Log in.
2.Verify login with valid credentials — should close the popup and show "Welcome <username>" with Log out.
3.Verify wrong password shows "Wrong password." and unknown user shows "User does not exist."
4.Verify blank fields shows "Please fill out Username and Password."
5.After logging in, refresh and move between pages — verify the session stays logged in.
6.Click Log out and verify it goes back to the logged-out state.

=====================================================================
## MODULE 3 — SIGN UP
=====================================================================

TestCases_003:- Sign up
1.Click on Sign up.
2.Verify a new unique username + password shows "Sign up successful."
3.Verify a duplicate username shows "This user already exist."
4.Verify blank fields shows "Please fill out Username and Password."
5.Verify that after signing up it does NOT auto-login (still shows Log in / Sign up).
6.Take the new credentials and log in with them — verify the account actually works.

=====================================================================
## MODULE 4 — CONTACT
=====================================================================

TestCases_004:- Contact
1.Click on Contact.
2.Verify sending a message with valid Email, Name and Message shows "Thanks for the message!!"
3.Verify what happens when all fields are blank and you hit Send — currently it still says "Thanks for the message!!" with no validation (raise as a bug).
4.Verify an invalid email format like "abc" is still accepted (raise as a bug/limitation).
5.Verify Close and the × dismiss the popup without sending.

=====================================================================
## MODULE 5 — ABOUT US
=====================================================================

TestCases_005:- About us
1.Click on About us.
2.Verify the popup opens with the video player.
3.Verify the video plays and play/pause controls work.
4.Verify clicking Close / × stops the video — check the audio doesn't keep playing in the background (raise as a bug if it does).
5.Verify reopening About us loads the video fresh with no double audio.

**AI Manual Test Cases**


## MODULE 1 — LOGIN
=================================================================

**TestCases_001:-** (Valid login — positive)
1. Go to https://www.demoblaze.com/
2. Click on "Log in"
3. Enter a valid Username and correct Password
4. Click on "Log in"
5. Verify successful login and "Welcome <username>" is shown


**TestCases_002:-** (Empty fields)
1. Go to https://www.demoblaze.com/
2. Click on "Log in"
3. Leave Username and Password blank
4. Click on "Log in"
5. Verify the alert "Please fill out Username and Password." is displayed


**TestCases_003:-** (Username only / Password only)
1. Go to https://www.demoblaze.com/
2. Click on "Log in"
3. Submit with Username only, then with Password only
4. Verify "Please fill out Username and Password." each time


**TestCases_004:-** (Password masking)
1. Go to https://www.demoblaze.com/
2. Click on "Log in"
3. Type characters into the Password field
4. Verify the characters are masked (shown as dots/asterisks)


**TestCases_005:-** (Cancel / dismiss)
1. Go to https://www.demoblaze.com/
2. Click on "Log in"
3. Dismiss using "Close" and then the ×
4. Verify the modal closes and no login occurs


==================================================================
## MODULE 2 — SIGN UP
====================================


**TestCases_006:-** (Valid registration — positive)
1. Go to https://www.demoblaze.com/
2. Click on "Sign up"
3. Enter a unique Username and Password
4. Click on "Sign up"
5. Verify the alert "Sign up successful." is displayed


**TestCases_007:-** (Duplicate username)
1. Go to https://www.demoblaze.com/
2. Click on "Sign up"
3. Enter a Username that already exists
4. Click on "Sign up"
5. Verify the alert "This user already exist." is displayed


**TestCases_008:-** (Empty fields)
1. Go to https://www.demoblaze.com/
2. Click on "Sign up"
3. Leave both fields blank and click "Sign up"
4. Verify the alert "Please fill out Username and Password." is displayed


**TestCases_009:-** (Username only / Password only)
1. Go to https://www.demoblaze.com/
2. Click on "Sign up"
3. Submit with Username only, then with Password only
4. Verify "Please fill out Username and Password." each time


==================================================================
## MODULE 3 — HOME
=================================================================


**TestCases_010:-** (Navbar links)
1. Go to https://www.demoblaze.com/
2. Click Home, Contact, About us, Cart, Log in, and Sign up
3. Verify each link opens its correct page/modal


**TestCases_011:-** (Each category individually)
1. Go to https://www.demoblaze.com/
2. Click "Phones" and verify only phones display
3. Click "Laptops" and verify only laptops display
4. Click "Monitors" and verify only monitors display


**TestCases_012:-** (Pagination Next/Previous)
1. Go to https://www.demoblaze.com/
2. Click "Next", then "Previous"
3. Verify the product set changes correctly with no duplicate or blank cards


**TestCases_013:-** (Carousel controls)
1. Go to https://www.demoblaze.com/
2. Use the carousel Next/Previous controls and the indicators
3. Verify the slides change accordingly


**TestCases_014:-** (Product card + open detail)
1. Go to https://www.demoblaze.com/
2. Verify each product card shows image, name, price, and description
3. Click a product and verify the detail page opens with matching data


==================================================================
## MODULE 4 — CONTACT
==================================================================


**TestCases_015:-** (Valid message send)
1. Go to https://www.demoblaze.com/
2. Click on "Contact"
3. Enter a valid Email, Name, and Message
4. Click on "Send message"
5. Verify the alert "Thanks for the message!!" is displayed


**TestCases_016:-** (Single-field-empty validation)
1. Go to https://www.demoblaze.com/
2. Click on "Contact"
3. Submit with Email empty only, then Name empty only, then Message empty only
4. Verify and document the validation behavior in each case


**TestCases_017:-** (Dismiss without sending)
1. Go to https://www.demoblaze.com/
2. Click on "Contact"
3. Dismiss using "Close" and the ×
4. Verify the modal closes and nothing is sent


==================================================================
## MODULE 5 — ABOUT US
==================================================================


**TestCases_018:-** (Modal opens / video loads)
1. Go to https://www.demoblaze.com/
2. Click on "About us"
3. Verify the modal opens and the video player/source loads without error


**TestCases_019:-** (Playback controls)
1. Go to https://www.demoblaze.com/
2. Click on "About us"
3. Use play, pause, and seek controls
4. Verify each control functions correctly


**TestCases_020:-** (Reopen + dismiss paths)
1. Go to https://www.demoblaze.com/
2. Open About us, close it, then reopen it
3. Dismiss using "Close" and the ×
4. Verify the modal resets on reopen and closes consistently each time


**Final Test Cases**


## MODULE 1 — LOGIN
=========================================================

**TestCases_001:-** (H) Valid login
1. Go to https://www.demoblaze.com/
2. Click on "Log in" and enter a valid Username and correct Password
3. Click on "Log in"
4. Verify the modal closes and "Welcome <username>" with "Log out" is shown


**TestCases_002:-** (H) Wrong password / unknown user
1. Go to https://www.demoblaze.com/
2. Log in with a valid Username but wrong Password
3. Verify the alert "Wrong password."
4. Log in with a Username that does not exist
5. Verify the alert "User does not exist."


**TestCases_003:-** (AI) Empty / single-field validation
1. Go to https://www.demoblaze.com/
2. Click on "Log in"
3. Submit blank, then Username-only, then Password-only
4. Verify "Please fill out Username and Password." each time


**TestCases_004:-** (H) Session persists + log out
1. Go to https://www.demoblaze.com/
2. Log in, refresh, and navigate Home → Cart → Home
3. Verify the user stays logged in
4. Click "Log out" and verify the logged-out state is restored


**TestCases_005:-** (H) Switch users — no state bleed
1. Go to https://www.demoblaze.com/
2. Log in as User A → Log out → Log in as User B
3. Verify no cart/session data from User A remains


=====================================================================
## MODULE 2 — SIGN UP
=====================================================================


**TestCases_006:-** (H) New user registration
1. Go to https://www.demoblaze.com/
2. Click on "Sign up" and enter a unique Username and Password
3. Click on "Sign up"
4. Verify the alert "Sign up successful."


**TestCases_007:-** (H) Duplicate username
1. Go to https://www.demoblaze.com/
2. Click on "Sign up" and enter an existing Username
3. Click on "Sign up"
4. Verify the alert "This user already exist."


**TestCases_008:-** (AI) Empty / single-field validation
1. Go to https://www.demoblaze.com/
2. Click on "Sign up"
3. Submit blank, then Username-only, then Password-only
4. Verify "Please fill out Username and Password." each time


**TestCases_009:-** (H+AI) Register then log in — end to end
1. Go to https://www.demoblaze.com/
2. Register a new unique user
3. Click on "Log in" and enter the same credentials
4. Verify the login succeeds (account persisted)


**TestCases_010:-** (H) No auto-login after signup
1. Go to https://www.demoblaze.com/
2. Register a new user successfully
3. Verify the user is still logged out


=====================================================================
## MODULE 3 — HOME
=====================================================================


**TestCases_011:-** (H) Default product load + data sanity
1. Go to https://www.demoblaze.com/
2. Verify products load with image, title, price, and description
3. Verify no missing titles, broken images, or invalid prices


**TestCases_012:-** (H+AI) Category filtering
1. Go to https://www.demoblaze.com/
2. Click "Phones", "Laptops", "Monitors" in turn
3. Verify the grid is scoped to the selected category each time


**TestCases_013:-** (H) Category + pagination scoping
1. Go to https://www.demoblaze.com/
2. Select a category, then click "Next"
3. Verify pagination stays within that category (no other categories leak in)


**TestCases_014:-** (AI) Pagination + carousel controls
1. Go to https://www.demoblaze.com/
2. Click "Next" then "Previous" on the product grid
3. Use the carousel Next/Previous and indicators
4. Verify both navigate correctly with no duplicate/blank cards


**TestCases_015:-** (H) Open product detail + add to cart
1. Go to https://www.demoblaze.com/
2. Open a product and verify name, price, description, image
3. Click "Add to cart" and verify "Product added." and the Cart updates


**TestCases_016:-** (AI) Navbar links + logo
1. Go to https://www.demoblaze.com/
2. Click each navbar link, then click the "PRODUCT STORE" logo
3. Verify each link works and the logo returns to home


=====================================================================
## MODULE 4 — CONTACT
=====================================================================


**TestCases_017:-** (H) Valid message send
1. Go to https://www.demoblaze.com/
2. Click on "Contact", fill Email, Name, and Message
3. Click on "Send message"
4. Verify the alert "Thanks for the message!!" and the modal closes


**TestCases_018:-** (H) Empty-form submit — defect hunt
1. Go to https://www.demoblaze.com/
2. Click on "Contact", leave all fields blank
3. Click on "Send message"
4. Verify behavior (currently accepted with no validation — log the defect)


**TestCases_019:-** (AI) Single-field-empty + dismiss
1. Go to https://www.demoblaze.com/
2. Click on "Contact"
3. Submit with each field empty in turn and document the result
4. Dismiss via "Close" / × and verify nothing is sent


=====================================================================
## MODULE 5 — ABOUT US
=====================================================================


**TestCases_020:-** (H) Modal opens and video plays
1. Go to https://www.demoblaze.com/
2. Click on "About us" and click play
3. Verify the player is shown and playback (play/pause) works


**TestCases_021:-** (H+AI) Video stops on close
1. Go to https://www.demoblaze.com/
2. Click on "About us", play the video, then click "Close" / ×
3. Verify the video stops; if audio persists, log the defect

--------------------------------------------------------------------------------------------------------------------------------------------------------

**TestCases_022:-** (AI) Reopen reset + dismiss paths
1. Go to https://www.demoblaze.com/
2. Open About us, close and reopen it
3. Dismiss using "Close" and the ×
4. Verify the video resets on r

--------------------------------------------------------------------------------------------------------------------------------------------------------
--------------------------------------------------------------------------------------------------------------------------------------------------------
**Session 2** :
Senior QA Test Case Generation Skill
--------------------------------------------------------------------------------------------------------------------------------------------------------
Skill Name :
Senior QA Test Case Generation Expert
---------------------------------------------------------------------------------------------------------------------------------------------------------
**Description**
   Generate comprehensive QA test cases as a Senior QA Engineer (10+ years), and
  convert them into Playwright automation scripts in JavaScript/TypeScript.
  Produces one consolidated final manual test-case set in a structured,
  module-based house format, plus the surrounding analysis (requirement summary,
  scenarios, positive/negative/boundary/edge cases, test data, requirement gaps,
  risks, regression). Use whenever the user wants to create, write, draft, or
  expand manual test cases or test scenarios, OR to automate them with Playwright
  (.spec.ts/.spec.js, getByRole locators, web-first assertions, dialog handling)
  — from a user story, BRD/FRS, acceptance criteria, API spec, UI design,
  workflow, or a live site (e.g. demoblaze). Also triggers on "this
  style/format," module-based suites like Login/Sign up/Home, "write automation
  tests," or "convert these test cases to Playwright." Prefer this skill whenever
  the deliverable is manual test cases or their Playwright automation.**


# QA Manual Test Cases

Produce manual QA test cases the way a senior tester would: analyze the
requirement first, enumerate scenarios, then write tight, executable test cases
in a consistent module-based house format — and surround them with the analysis
a real QA hand-off needs (test data, requirement gaps, risks, regression).

The output is always a single, consolidated **final** test-case set. Do not
split work into separate "human" and "AI" passes, and do not tag cases by
origin — produce one clean, deduplicated suite.

This skill covers two deliverables that share the same source of truth: the
**manual test cases** (below) and the **Playwright automation scripts** (JS/TS)
that implement them. A QA can use it to test by hand and to generate the
automated suite from the very same cases — see "Playwright automation" near the
end. When the user asks to "automate," "write Playwright tests," or "convert
these to scripts," produce automation that traces back one-to-one to the manual
`TestCases_NNN`.

## Role

Act as a **Senior QA Engineer with 10+ years of experience** across functional,
system, integration, regression, and user-acceptance testing, plus API, web, and
mobile application testing. The objective is complete validation of the
requirement through comprehensive, reusable test cases — not just happy-path
checks. Bring the judgment of someone who has shipped real software: anticipate
the failure modes, the ambiguous requirements, and the modules a change will
ripple into.

## Inputs the skill accepts

Work from any of these; if only an app/URL is given, explore the feature areas
directly and infer the requirements:

- User stories and acceptance criteria
- Business Requirement Documents (BRD) and Functional Requirement Specs (FRS)
- API specifications
- UI designs, workflow diagrams, and process documents
- A live application or URL to test against

## Output structure

For a full requirement, generate these sections in order. For a small or casual
ask ("just give me test cases for the login modal"), lead with the test cases
and include the analysis sections only where they add value.

1. **Requirement Summary** — a concise restatement showing you understood the
   requirement and its intent.
2. **Test Scenarios** — the list of everything worth testing, before drilling
   into steps (e.g. "Verify successful password reset," "Verify expired reset
   link," "Verify password policy validation").
3. **Test Cases** — the detailed cases in house format (see below), grouped into
   modules.
4. **Test Data** — concrete valid inputs, invalid inputs, and boundary values.
5. **Requirement Gaps** — missing validations, undefined rules, ambiguous or
   contradictory requirements you noticed while writing the cases.
6. **Risks** — security, data-loss, performance, and dependency concerns.
7. **Regression Areas** — the modules and services likely impacted, so the team
   knows what to re-test (e.g. Login module, User profile, Notifications,
   Authentication services).

## Document header

When producing a standalone test-case document, open with this block:

```
QA Manual Test Cases
Project: <project / company name>
Application: <application name + URL>
Tester: <tester name>
```

## Module structure

Group test cases into **modules** — one per feature area (Login, Sign up, Home,
Contact, About us, Cart, Checkout, etc.). Separate modules with a full-width line
of `=` characters above and below the heading, which uses an em dash:

```
=====================================================================
MODULE 1 — LOGIN
=====================================================================
```

Number cases continuously across the whole document.

## Anatomy of a single test case

House format — numbered, imperative steps ending in a verification:

```
TestCases_001:- (Valid login)
Preconditions: A registered user exists
Priority: High
1. Go to https://www.demoblaze.com/
2. Click on "Log in" and enter a valid Username and correct Password
3. Click on "Log in"
4. Verify the modal closes and "Welcome <user>" with "Log out" is shown
```

Rules that make a case look right:

- **ID:** `TestCases_NNN`, zero-padded to three digits, followed by `:-`, then a
  short descriptor in parentheses naming what the case covers — e.g.
  `(Empty fields)`, `(Duplicate username)`, `(Password masking)`.
- **Preconditions:** state any required setup (logged-in user, item in cart,
  existing record). Omit the line when there are none.
- **Priority:** `High`, `Medium`, or `Low`, based on business impact. Omit when
  not meaningful.
- **Steps:** imperative and concrete. Most cases start with `Go to <URL>`, then
  `Click on "<exact label>"`, then the action.
- **Last step is the verification.** Always end on a `Verify …` step stating the
  expected result.
- **Quote UI text exactly.** Button labels, field names, and especially alert/
  toast messages go in straight quotes verbatim:
  `"Please fill out Username and Password."`, `"Sign up successful."`,
  `"This user already exist."`, `"Wrong password."`, `"User does not exist."`,
  `"Product added."`, `"Thanks for the message!!"`. Exact strings are what make a
  case executable, so never paraphrase them.

If the user prefers a tabular layout (common for spreadsheets/hand-offs), use
these columns instead: **Test Case ID | Test Scenario | Preconditions | Test
Steps | Test Data | Expected Result | Priority**.

## Coverage — write across all four case types

A senior-quality suite is not just happy paths. For each feature, deliberately
cover:

- **Positive** — expected behavior with valid input (valid login, successful
  registration, correct submission).
- **Negative** — invalid conditions (wrong credentials, invalid formats, empty
  mandatory fields).
- **Boundary** — minimum and maximum limits (shortest/longest password, max
  input length, date limits, just-inside/just-outside values).
- **Edge** — unusual situations (special characters, duplicate records, session
  timeout, network interruption, multiple browser tabs, back-button after
  submit).

Also validate, where applicable: mandatory vs optional fields, data formats,
length restrictions, error messages, unauthorized/role-based access, session
handling, input validation, navigation clarity, field labels, and accessibility.

## Test design techniques

Apply standard techniques to decide which cases are worth writing, rather than
brute-forcing every combination:

- **Equivalence Partitioning** — one representative per input class.
- **Boundary Value Analysis** — values at and just past the limits.
- **Decision Table Testing** — for combinations of conditions and rules.
- **State Transition Testing** — for flows with states (logged out → logged in →
  locked, draft → submitted → approved).
- **Error Guessing** — experience-driven probing of likely-fragile spots.
- **Pairwise Testing** — to cover interactions without combinatorial explosion.

## Defect-hunting is built in

This style deliberately writes cases that probe known-weak behavior and tells the
tester to log it. When a case targets a likely defect, say so inline:

- `(raise as a bug)` / `(raise as a bug/limitation)`
- `(log the defect)`
- append `— defect hunt` to the descriptor

Classic examples: a contact form that accepts an all-blank submit with no
validation, an "email" field that accepts `abc`, or audio that keeps playing
after a video modal is closed. Include these probing cases, not only happy paths.

## Worked example

Requirement: *"As a user, I want to reset my password so that I can regain access
to my account."* Rendered in full house style:

```
Requirement Summary
A logged-out user can request a password reset by email and set a new password
via a time-limited link, subject to the password policy.

Test Scenarios
- Verify password reset request with a registered email.
- Verify request with an unregistered / invalid email.
- Verify the reset link expires after its validity window.
- Verify the new password is enforced against the password policy.
- Verify an already-used reset link cannot be reused.

=====================================================================
MODULE 1 — PASSWORD RESET
=====================================================================
TestCases_001:- (Valid reset request)
Preconditions: A registered account with a known email exists
Priority: High
1. Go to the login page and click "Forgot password".
2. Enter the registered email and click "Send".
3. Verify "Reset link sent to your email" is shown and an email is received.

TestCases_002:- (Unregistered email)
Priority: Medium
1. Click "Forgot password", enter an unregistered email, click "Send".
2. Verify an appropriate error/notice is shown and no link is sent.

TestCases_003:- (Expired link — defect hunt)
Preconditions: A reset link older than its validity window
Priority: High
1. Open the expired reset link.
2. Verify "This reset link has expired" is shown and the form is blocked.

TestCases_004:- (Password policy validation)
Priority: High
1. Open a valid reset link and submit a weak password (e.g. "123").
2. Verify the policy error is shown and the password is not changed.

Test Data
- Valid: registered email, policy-compliant password.
- Invalid: unregistered email, malformed email "abc", weak password "123".
- Boundary: password at minimum and maximum allowed length.

Requirement Gaps
- Link validity duration is unspecified.
- Behavior on reusing an already-consumed link is undefined.

Risks
- Token reuse / link guessing (security).
- Account lockout if reset throttling is missing (usability + dependency).

Regression Areas
- Login, Authentication service, Email/notification service, Session handling.
```

## Domain knowledge

Adapt vocabulary and scenarios to the domain when known: Banking (transactions,
payments, account management), E-Commerce (cart, checkout, payments, orders),
Healthcare (patient management, appointments, claims), Insurance (policy
management, claims processing), and CRM (leads, opportunities, customer
management). Adapt modules to the actual app — don't force demoblaze modules onto
a different site.

## Coverage checklist (so nothing obvious gets missed)

For a typical e-commerce / form-driven web app, make sure the suite covers, where
applicable:

- **Auth:** valid login, wrong password, unknown user, empty/single-field
  validation, password masking, dismiss paths, session persistence across
  refresh + navigation, log out, no state bleed when switching users.
- **Sign up:** valid unique registration, duplicate username, empty/single-field
  validation, no auto-login after signup, register-then-login end-to-end.
- **Home / catalog:** navbar links, logo returns home, each category filter
  individually, category + pagination scoping (no leakage), carousel controls,
  product card data sanity (image/title/price/description), open detail + add to
  cart with the exact added message.
- **Forms (Contact etc.):** valid send, all-blank submit (defect hunt),
  single-field-empty behavior, invalid email accepted (defect hunt), Close and ×
  dismiss without sending.
- **Media modals (About us etc.):** modal opens / source loads, play/pause/seek,
  video stops on close (audio-persists defect hunt), reopen resets cleanly.

## Quality standards

Generated test cases must be clear, concise, unambiguous, reusable, follow
industry standards, and together give complete requirement coverage.

## Playwright automation (JavaScript / TypeScript)

When the user wants automated scripts — "automate these," "write Playwright
tests," "convert to automation," or asks for a runnable suite — generate
Playwright tests in JS/TS that implement the **same final test cases**. The
manual cases are the source of truth: every automated test traces back to a
`TestCases_NNN`, and the assertions check the exact Expected Result.

### Conventions

- Use the official `@playwright/test` runner. Default to **TypeScript**
  (`*.spec.ts`); offer plain JS (`*.spec.js`) if the user prefers.
- One spec file per module, named after it (`login.spec.ts`, `signup.spec.ts`).
- Map **module → `test.describe(...)`** and **manual case → `test('TestCases_001 - Valid login', ...)`** so the test title carries the ID for traceability.
- Put **Preconditions** in `test.beforeEach` (or a fixture). Keep every test
  independent and parallel-safe — no shared mutable state between tests.
- Set `baseURL` in `playwright.config.ts` and navigate with `page.goto('/')`.
- Mirror the numbered manual steps with `test.step('...')` blocks when it makes
  the report easier to read.

### Locators — prefer user-facing, avoid brittle selectors

Resolve elements the way a user perceives them, so tests survive markup changes:
`getByRole`, `getByLabel`, `getByPlaceholder`, `getByText`, `getByTestId`. Reach
for CSS/`#id` only when the app exposes no accessible name (many legacy apps,
including demoblaze's modal fields, do not) — and note that as a candidate
accessibility gap in the manual **Requirement Gaps** section.

### Assertions — web-first and auto-waiting

Use auto-waiting assertions: `await expect(locator).toBeVisible()`,
`.toHaveText()`, `.toContainText()`, `.toHaveValue()`, `.toHaveURL()`. Assert the
verbatim UI strings from the manual case. Never use fixed sleeps
(`waitForTimeout`) to "wait for" state — rely on Playwright's auto-waiting.

### Native dialogs / alerts (critical)

Many house-style expected results are native browser alerts (`window.alert`) —
e.g. `"Please fill out Username and Password."`, `"Sign up successful."`,
`"Wrong password."`, `"Product added."`. Playwright auto-dismisses dialogs, so
register a handler **before** the action and assert on `dialog.message()`:

```ts
const [dialog] = await Promise.all([
  page.waitForEvent('dialog'),
  page.getByRole('button', { name: 'Log in' }).click(),
]);
expect(dialog.message()).toBe('Please fill out Username and Password.');
await dialog.accept();
```

### Test data

Generate unique data for create flows so reruns don't collide:
`const username = 'user_' + Date.now();`. Keep valid/invalid/boundary inputs in
one place (a fixture or a `data/` module) mirroring the manual **Test Data**.

### Reuse at scale

For larger suites use the **Page Object Model** — a class per page holding its
locators and actions — and Playwright **fixtures** for shared setup (e.g. a
logged-in `storageState` so authenticated tests skip the login UI). Keep it light
for small suites; don't over-engineer.

### Worked example — `login.spec.ts`

Implements the manual Login cases (valid login, empty-field validation,
wrong-password) for demoblaze:

```ts
import { test, expect } from '@playwright/test';

test.describe('Login', () => {
  test.beforeEach(async ({ page }) => {
    await page.goto('/');                         // baseURL = https://www.demoblaze.com/
    await page.getByRole('link', { name: 'Log in' }).click();
    await expect(page.locator('#logInModal')).toBeVisible();
  });

  test('TestCases_001 - Valid login', async ({ page }) => {
    await page.locator('#loginusername').fill('test_user');   // no accessible name → id
    await page.locator('#loginpassword').fill('Correct123!');
    await page.getByRole('button', { name: 'Log in' }).click();
    // Expected: modal closes and "Welcome <user>" with Log out is shown
    await expect(page.locator('#nameofuser')).toHaveText('Welcome test_user');
    await expect(page.getByRole('link', { name: 'Log out' })).toBeVisible();
  });

  test('TestCases_002 - Empty fields validation', async ({ page }) => {
    const [dialog] = await Promise.all([
      page.waitForEvent('dialog'),
      page.getByRole('button', { name: 'Log in' }).click(),
    ]);
    expect(dialog.message()).toBe('Please fill out Username and Password.');
    await dialog.accept();
  });

  test('TestCases_003 - Wrong password', async ({ page }) => {
    await page.locator('#loginusername').fill('test_user');
    await page.locator('#loginpassword').fill('definitely-wrong');
    const [dialog] = await Promise.all([
      page.waitForEvent('dialog'),
      page.getByRole('button', { name: 'Log in' }).click(),
    ]);
    expect(dialog.message()).toBe('Wrong password.');
    await dialog.accept();
  });
});
```

Minimal config:

```ts
// playwright.config.ts
import { defineConfig } from '@playwright/test';
export default defineConfig({
  use: { baseURL: 'https://www.demoblaze.com/', headless: true, trace: 'on-first-retry' },
  testDir: './tests',
});
```

### Deliverable

When generating automation, save real files (`playwright.config.ts`, specs under
`tests/`, any page objects/fixtures) and present them, so the QA can run
`npx playwright test` directly. Keep selectors realistic to the actual app rather
than inventing IDs; if the live markup is unknown, use role-based locators and
flag the assumptions.

## Output format

Plain text is the default and matches the house style. If the user asks for a
downloadable file:
- A **spreadsheet (.xlsx)** suits the tabular layout (ID | Scenario |
  Preconditions | Steps | Test Data | Expected Result | Priority) — read the xlsx
  skill first, then present the file.
- A **Word document (.docx)** suits a full report with the analysis sections —
  read the docx skill first, then present the file.
- For **Playwright automation**, write actual `*.spec.ts`/`*.spec.js` files plus
  `playwright.config.ts` (and any page objects/fixtures) and present them so the
  suite is runnable with `npx playwright test`.
- Otherwise keep the exact plain-text layout shown above.

## Style summary (quick reference)

- Open with Requirement Summary → Test Scenarios → Test Cases → Test Data →
  Requirement Gaps → Risks → Regression Areas (scale down for small asks).
- Header block with Project / Application / Tester for standalone documents.
- Modules separated by `=` lines; heading `MODULE N — NAME` with an em dash.
- `TestCases_NNN:-` IDs, three digits, continuous numbering, with optional
  Preconditions and Priority lines.
- Imperative steps; start with `Go to <URL>` / `Click on "<label>"`; last step is
  always a `Verify …`.
- Quote all UI labels and alert messages verbatim.
- Cover positive, negative, boundary, and edge cases using standard test design
  techniques; bake in defect-hunting cases.
- Produce one consolidated final set — no separate passes, no origin tags.
- For automation, generate Playwright (JS/TS) tests that trace 1:1 to
  `TestCases_NNN`: `describe` per module, role-based locators, web-first
  assertions, and `dialog` handling for native alerts.


