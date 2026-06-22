---
name: functional-test-cases
description: Generate a comprehensive, exhaustive list of manual functional test cases for a web application or URL, formatted as numbered, step-by-step test scripts with explicit verification steps. Use this skill whenever the user asks to "create test cases", "list functional test cases", "write test cases for this URL", "explore all possible routes/flows", or otherwise wants QA-style test scenarios for a website, web page, or app — even if they don't say the words "functional test cases" exactly. Trigger this for any request that boils down to "what should I test on this site and how", including login flows, forms, navigation, cart/checkout, search, and error/validation handling.
---

# Functional Test Cases

This skill produces manual functional test cases for a web application: the concrete, repeatable scripts a QA tester (or an automation engineer writing scripts) would follow to verify that the application behaves correctly. Each test case is a self-contained sequence of actions followed by explicit verifications.

The goal is **coverage**: identify every meaningful functional route through the application and write a test case for each, including happy paths, validation/error paths, and edge cases.

## Workflow

1. **Understand the target.** Identify the URL or feature the user wants tested. If a URL is given, fetch it (use `web_fetch` / `web_search`) to inspect the page structure — form fields, buttons, links, expected text, error messages, and navigation targets. If the page can't be fetched, rely on knowledge of how that kind of app typically works and state any assumptions briefly at the top.

2. **Enumerate the routes.** Before writing, mentally map every functional flow the feature supports. For a given feature, systematically walk through these categories so nothing is missed:
   - **Happy path** — valid inputs, successful outcome.
   - **Invalid input** — wrong values for each individual field, one at a time.
   - **Empty / required-field** — each required field left blank, one at a time.
   - **Boundary / format** — too long, too short, special characters, whitespace, case sensitivity.
   - **State-specific** — locked accounts, expired sessions, already-existing records, permission-restricted users.
   - **Navigation & UI** — links, redirects, presence of key elements (titles, icons, buttons).
   - **Negative / abuse** — SQL-ish strings, repeated submissions, back-button behavior, direct URL access to protected pages.

3. **Write one test case per distinct route.** Don't fold several checks into one case if they exercise different conditions. Prefer many small, focused cases over a few large ones.

4. **Be specific.** Use the actual field names, button labels, valid/invalid values, and exact expected messages. When real example values exist (e.g., known demo credentials or the page's literal error strings), use them verbatim inside double quotes.

## Output format

ALWAYS use this exact structure. Start with the literal heading `TestCases`, then list each case with a zero-padded three-digit ID, a `:-` suffix, an underscore separator line, the action steps, and the verification step(s).

```
TestCases
001:-
_
<action step>
<action step>
<action step>
Verify that <expected outcome stated explicitly>
Verify that <additional expected outcome, if any>
002:-
_
<action step>
...
```

Rules for the format:
- IDs are zero-padded and sequential: `001:-`, `002:-`, `003:-`, …
- The `_` on its own line separates the ID from the steps for every case.
- Action steps are plain imperative lines (`Go to …`, `Enter …`, `Click on …`, `Leave … empty`).
- Quote literal values and messages exactly: `Enter valid username "standard_user"`, `Verify that an error message is displayed: "Epic sadface: Username is required"`.
- Every test case ends with one or more `Verify that …` lines that state the expected result explicitly — never leave a case without a verification.
- Output the test cases as plain text exactly in this shape (not a table, not bullets), so it can be copied directly into a test plan or handed to an automation engineer.

## Example

This is the expected output for the prompt: *"Create a list of all the functional test cases for this URL https://www.saucedemo.com/ — explore all the possible routes"* (login feature). Note the exhaustive coverage of one happy path plus every invalid/empty/locked variant:

```
TestCases
001:-
_
Go to https://www.saucedemo.com/
Enter valid username "standard_user"
Enter valid password "secret_sauce"
Click on the Login button
Verify that the user is logged in successfully and redirected to the Inventory page ("/inventory.html")
Verify that the header title "Swag Labs" and the shopping cart icon are visible
002:-
_
Go to https://www.saucedemo.com/
Enter an invalid username "invalid_user"
Enter a valid password "secret_sauce"
Click on the Login button
Verify that an error message is displayed: "Epic sadface: Username and password do not match any user in this service"
003:-
_
Go to https://www.saucedemo.com/
Enter valid username "standard_user"
Enter an invalid password "wrong_password"
Click on the Login button
Verify that an error message is displayed: "Epic sadface: Username and password do not match any user in this service"
004:-
_
Go to https://www.saucedemo.com/
Leave the username field empty
Enter a valid password "secret_sauce"
Click on the Login button
Verify that an error message is displayed: "Epic sadface: Username is required"
005:-
_
Go to https://www.saucedemo.com/
Enter valid username "standard_user"
Leave the password field empty
Click on the Login button
Verify that an error message is displayed: "Epic sadface: Password is required"
006:-
_
Go to https://www.saucedemo.com/
Enter the locked-out username "locked_out_user"
Enter valid password "secret_sauce"
Click on the Login button
Verify that an error message is displayed: "Epic sadface: Sorry, this user has been locked out."
```

## Coverage reminders

- When the app has more than one feature area (login, inventory, cart, checkout, etc.), generate cases for each area, continuing the same numbering scheme. Group implicitly by ordering related cases together.
- If the user names a specific feature ("just the login page"), scope to that feature but still exhaust its routes.
- Don't stop at the happy path. A login feature with only one or two test cases is incomplete — the example above shows the minimum expected thoroughness for a single feature.
- Prefer real, observed values (field names, labels, error text) over invented ones. Only invent placeholders when the real values genuinely can't be determined, and say so.
