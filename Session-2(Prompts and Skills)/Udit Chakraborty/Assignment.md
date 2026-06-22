# 📢 QA MANUAL TEST CASES MASTER SUITE
**Member:** Udit Chakraborty  
**Target Application:** https://eventhub.rahulshettyacademy.com/

---

## 🧠 SECTION 1: HUMAN THINKING TEST CASES

### ### TC_01 – New User Registration with Valid Data
> * **Test Steps:**
>   1. Open the EventHub website on a browser.
>   2. Click on the "Register" link.
>   3. Enter a valid email address.
>   4. Enter a valid password.
>   5. Enter the same password in the Confirm Password field.
>   6. Click Create Account.
> * **Expected Result:** Verify that account is created successfully.

### ### TC_02 – Registration with Invalid Email
> * **Test Steps:**
>   1. Open the EventHub website on a browser.
>   2. Click on the "Register" link.
>   3. Enter invalid email format.
>   4. Enter valid password.
>   5. Enter confirm password.
>   6. Click Create Account.
> * **Expected Result:** Verify error message is displayed.

### ### TC_03 – Registration with Password Mismatch
> * **Test Steps:**
>   1. Open the EventHub website on a browser.
>   2. Click on the "Register" link.
>   3. Enter valid email.
>   4. Enter valid password..
>   5. Enter a different password to confirm the password.
>   6. Click Create Account.
> * **Expected Result:** Verify password mismatch error message.

### ### TC_04 – Registration with Empty Fields
> * **Test Steps:**
>   1. Open EventHub website.
>   2. Click on the Register link.
>   3. Leave all fields blank.
>   4. Click Create Account.
> * **Expected Result:** Verify mandatory field validation error messages are displayed.

### ### TC_05 – Registration with Existing Email.
> * **Test Steps:**
>   1. Open EventHub website.
>   2. Click the Register link.
>   3. Enter an email already registered.
>   4. Enter valid password.
>   5. Click Create Account.
> * **Expected Result:** Verify appropriate error messages are displayed.

### ### TC_06 – Login with Valid Credentials
> * **Test Steps:**
>   1. Open EventHub website.
>   2. Enter a registered email.
>   3. Enter valid password.
>   4. Click Sign In.
> * **Expected Result:** Verify successful login and redirection to Dashboard.

### ### TC_07 – Login with Invalid Password
> * **Test Steps:**
>   1. Open EventHub website.
>   2. Enter a registered email.
>   3. Enter a invalid password.
>   4. Click the Sign In button.
> * **Expected Result:** Verify error message.

### ### TC_08 – Explore Available Events
> * **Test Steps:**
>   1. Login with valid credentials.
>   2. Click Explore Events.
> * **Expected Result:** Verify all event lists are displayed.

### ### TC_09 – Search Event
> * **Test Steps:**
>   1. Login with valid credentials.
>   2. Navigate to Explore Events.
>   3. Search events by keywords.
> * **Expected Result:** Verify relevant events appear.

### ### TC_10 – Search Non-Existing Event
> * **Test Steps:**
>   1. Login with valid credentials.
>   2. Navigate to Browse Events.
>   3. Search with invalid keywords.
> * **Expected Result:** Verify appropriate error messages.

### ### TC_11 – Event Booking
> * **Test Steps:**
>   1. Login with valid credentials.
>   2. Click on the ‘Browse Events’ button.
>   3. Select an available event.
>   4. Click ‘Book Now’ button.
>   5. Enter Full Name, Email, Phone Number and Select number of tickets from + icon.
>   6. Click the button ‘Confirm booking’.
> * **Expected Result:** Verify the success message. Verify booking appears in the My Bookings section.

### ### TC_12 – Booking with invalid data.
> * **Test Steps:**
>   1. Login with valid credentials.
>   2. Click on the ‘Browse Events’ button.
>   3. Select an available event.
>   4. Click ‘Book Now’.
>   5. Enter invalid phone number.
>   6. Submit booking.
> * **Expected Result:** Verify validation message.

### ### TC_13 – Cancel Event Booking
> * **Test Steps:**
>   1. Login with valid credentials.
>   2. Navigate to My Bookings.
>   3. Select booked event.
>   4. Click Cancel Booking.
>   5. Confirm cancellation.
> * **Expected Result:** Verify booking is removed. Verify the success message.

### ### TC_14 – Logout
> * **Test Steps:**
>   1. Login with valid credentials.
>   2. Click the Logout button on the EventHub menu.
> * **Expected Result:** Verify the user is logged out. Verify the login page is displayed.

---

## 🤖 SECTION 2: AI MANUAL TEST CASES

### ## Module 1: Authentication & Session Management

### ### TC_AUTH_01: Verify successful login with valid credentials.
> * **Pre-conditions:** User is registered on EventHub.
> * **Test Steps:**
>   1. Navigate to URL.
>   2. Enter valid Email and Password.
>   3. Click "Login".
> * **Expected Result:** User is successfully authenticated and redirected to the Event Discovery Dashboard. A valid token/session is established.

### ### TC_AUTH_02: Verify login failure with invalid or empty fields.
> * **Pre-conditions:** User is on the login page.
> * **Test Steps:**
>   1. Enter an unregistered email or incorrect password.
>   2. Clear fields and try submitting.
>   3. Click "Login".
> * **Expected Result:** Appropriate error validation messages are displayed (e.g., "Invalid credentials" or field-specific inline validations).

### ### TC_AUTH_03: Verify user registration/signup flow.
> * **Pre-conditions:** User does not have an account.
> * **Test Steps:**
>   1. Click on "Sign Up" / "Register".
>   2. Fill in Name, Email, Password, and Confirm Password.
>   3. Submit the form.
> * **Expected Result:** Account is successfully created. User is either auto-logged in or redirected to the login page with a success message.

### ### TC_AUTH_04: Verify session persistence and Logout function.
> * **Pre-conditions:** User is actively logged in.
> * **Test Steps:**
>   1. Refresh the page or duplicate the tab (verify state).
>   2. Click the "Logout" button.
> * **Expected Result:** 1. The user session persists on refresh. 2. After clicking logout, the session is destroyed, and the user is redirected back to the login page.

---

### ## Module 2: Event Discovery, Search & Filtering

### ### TC_DISC_01: Verify Event Search functionality.
> * **Pre-conditions:** User is logged in and viewing the dashboard.
> * **Test Steps:**
>   1. Type a partial or full name of an existing event in the search bar.
>   2. Press Enter or click Search.
> * **Expected Result:** The event list dynamically updates to show only matching events. Unrelated events are hidden.

### ### TC_DISC_02: Verify Multi-Step Filtering (Category, Location, Date).
> * **Pre-conditions:** Multiple events exist in the system across diverse categories.
> * **Test Steps:**
>   1. Select a category dropdown (e.g., "Tech", "Music").
>   2. Select a location filter.
>   3. Apply filters.
> * **Expected Result:** The event cards update instantly to reflect the intersection of all selected filters.

### ### TC_DISC_03: Verify clear/reset filters.
> * **Pre-conditions:** Filters are actively applied in TC_DISC_02.
> * **Test Steps:**
>   1. Click the "Clear Filters" or "Reset" button.
> * **Expected Result:** All filter checkboxes/dropdowns return to default, and the complete inventory list of events is re-displayed.

---

### ## Module 3: End-to-End Ticket Booking Workflow (Critical Path)

### ### TC_BOOK_01: Complete End-to-End ticket booking flow with standard checkout.
> * **Pre-conditions:** User is logged in with sufficient mock funds or test data.
> * **Test Steps:**
>   1. Find an active event and click "View Details" / "Book Tickets".
>   2. Select ticket type (e.g., VIP, General Admission) and change quantity to 2.
>   3. Click "Proceed to Checkout".
>   4. Fill out attendee details form.
>   5. Enter test payment card details and click "Pay/Place Order".
> * **Expected Result:** 1. A "Booking Successful" page appears displaying a unique Order/Booking ID. 2. Order total matches the exact calculation (Quantity * Price).

### ### TC_BOOK_02: Verify booking form field validations.
> * **Pre-conditions:** User is on the Multi-step Booking Form.
> * **Test Steps:**
>   1. Leave mandatory attendee fields empty.
>   2. Enter an invalid email format.
>   3. Attempt to proceed to payment.
> * **Expected Result:** Form submission is blocked; clear inline warning flags appear on the mandatory fields.

### ### TC_BOOK_03: Verify dynamic seat/ticket inventory deduction.
> * **Pre-conditions:** An event has a finite number of available tickets remaining.
> * **Test Steps:**
>   1. Note the initial available ticket count for an event.
>   2. Book 3 tickets following TC_BOOK_01.
>   3. Return to the event details page.
> * **Expected Result:** The remaining ticket counter displays exactly Initial Count - 3.

---

### ## Module 4: User Dashboard, Orders & History

### ### TC_DASH_01: Verify Booking History / My Orders section.
> * **Pre-conditions:** User has completed at least one transaction (TC_BOOK_01).
> * **Test Steps:**
>   1. Navigate to "My Bookings" or "Order History" via the profile menu.
> * **Expected Result:** The newly created Order ID is displayed with accurate details (Event Name, Date, Quantity, Price, Status: Confirmed).

### ### TC_DASH_02: Verify Ticket Cancellation/Refund flow (if applicable).
> * **Pre-conditions:** User has an active booking.
> * **Test Steps:**
>   1. Navigate to My Bookings.
>   2. Click "Cancel Ticket" on an upcoming event.
>   3. Confirm cancellation in the alert modal.
> * **Expected Result:** 1. The order status updates to "Cancelled". 2. The respective event's available ticket inventory increases back by that amount.

---

### ## Module 5: Edge Cases, Security & Non-Functional API Alignment

### ### TC_EDGE_01: Verify out-of-stock / sold-out behavior.
> * **Pre-conditions:** An event has 0 tickets left.
> * **Test Steps:**
>   1. Navigate to a sold-out event card.
> * **Expected Result:** The "Book Tickets" button is disabled or replaced with a "Sold Out" badge. User cannot trigger checkout.

### ### TC_EDGE_02: Verify unauthorized route access (Unauthorized Guard).
> * **Pre-conditions:** User is logged out.
> * **Test Steps:**
>   1. Attempt to bypass login by directly typing the dashboard or order URL (e.g., .../dashboard or .../orders) into the browser address bar.
> * **Expected Result:** The application blocks access and safely redirects the user back to the login screen with a warning.

### ### TC_EDGE_03: Verify concurrent window actions or rapid button clicking.
> * **Pre-conditions:** User is on the final payment button.
> * **Test Steps:**
>   1. Double-click or rapid-fire click the "Submit Payment" button.
> * **Expected Result:** The system processes only the initial request; duplicate submissions are safely handled to prevent accidental multiple bookings or double transactions.

---

## ⚡ SECTION 3: FINAL CONSOLIDATED AUTOMATION-READY CASES

### ## Module 1: Authentication & Session Management

### ### TC_AUTH_A01: New User Registration with Valid Data
> * **Pre-conditions:** User is on the landing page and not logged in.
> * **Test Steps:**
>   1. Navigate to the EventHub URL.
>   2. Click on the "Register" link.
>   3. Enter a unique, valid email address.
>   4. Enter a strong password.
>   5. Enter the same password in the Confirm Password field.
>   6. Click "Create Account".
> * **Expected Result:** Account is created successfully. A confirmation message appears and the user is redirected to the login interface or dashboard.

### ### TC_AUTH_A02: Registration with Invalid Email Format
> * **Pre-conditions:** User is on the Registration page.
> * **Test Steps:**
>   1. Enter an invalid email structure (e.g., user@com, missing @ sign).
>   2. Enter a valid password and matching confirm password.
>   3. Click "Create Account".
> * **Expected Result:** An error message specifying an invalid email format is displayed; account creation is blocked.

### ### TC_AUTH_A03: Registration with Password Mismatch
> * **Pre-conditions:** User is on the Registration page.
> * **Test Steps:**
>   1. Enter a valid email address.
>   2. Enter a valid password.
>   3. Enter a completely different string in the Confirm Password field.
>   4. Click "Create Account".
> * **Expected Result:** A password mismatch validation error is explicitly displayed.

### ### TC_AUTH_A04: Registration with Empty Fields
> * **Pre-conditions:** User is on the Registration page.
> * **Test Steps:**
>   1. Leave all input fields blank.
>   2. Click "Create Account".
> * **Expected Result:** Mandatory field validation prompts/warnings are triggered beneath each empty input.

### ### TC_AUTH_A05: Registration with Existing Email
> * **Pre-conditions:** User is on the Registration page; an account already exists for the email used.
> * **Test Steps:**
>   1. Enter the previously registered email address.
>   2. Provide a valid password and matching confirmation.
>   3. Click "Create Account".
> * **Expected Result:** An error indicating that the email is already in use is displayed.

### ### TC_AUTH_A06: Login with Valid Credentials
> * **Pre-conditions:** A user account exists with confirmed credentials.
> * **Test Steps:**
>   1. Navigate to the login page.
>   2. Enter the registered email and matching valid password.
>   3. Click "Sign In" / "Login".
> * **Expected Result:** User is authenticated successfully and instantly redirected to the Event Discovery Dashboard.

### ### TC_AUTH_A07: Login with Invalid Password
> * **Pre-conditions:** A user account exists with confirmed credentials.
> * **Test Steps:**
>   1. Navigate to the login page.
>   2. Enter the registered email address.
>   3. Enter an incorrect or random password.
>   4. Click the "Sign In" button.
> * **Expected Result:** Login fails; an error message stating incorrect password/credentials appears.

### ### TC_AUTH_A08: User Logout and Session Destruction
> * **Pre-conditions:** User is actively logged into the platform.
> * **Test Steps:**
>   1. Click the "Logout" button situated on the EventHub menu/navbar.
>   2. Try clicking the browser's "Back" button.
> * **Expected Result:** The active user session is terminated, the user is safely redirected back to the login screen, and they cannot navigate backward to view authenticated data.

---

### ## Module 2: Event Discovery, Search & Filtering

### ### TC_DISC_A01: Explore Available Events Catalog
> * **Pre-conditions:** User is logged in with valid credentials.
> * **Test Steps:**
>   1. Click on the "Explore Events" or "Browse Events" option in the navigation bar.
> * **Expected Result:** The page updates completely, displaying the collection list of all active upcoming event cards.

### ### TC_DISC_A02: Search Event by Keywords
> * **Pre-conditions:** User is on the Explore Events catalog page.
> * **Test Steps:**
>   1. Locate the search bar UI.
>   2. Type matching keywords from a known event (e.g., "Tech", "Concert").
>   3. Submit the search query.
> * **Expected Result:** The UI dynamically updates to filter out unrelated entries, showing only events matching the input keyword.

### ### TC_DISC_A03: Search Non-Existing Event
> * **Pre-conditions:** User is on the Browse Events catalog page.
> * **Test Steps:**
>   1. Type a random string of characters (e.g., xyz123abc!) into the search bar.
>   2. Execute the search.
> * **Expected Result:** A clear feedback text message (e.g., "No events found" or equivalent) is shown on screen.

### ### TC_DISC_A04: Multi-Step Filtering & Reset
> * **Pre-conditions:** Multiple events exist in the system across diverse categories.
> * **Test Steps:**
>   1. Select a category dropdown filter (e.g., "Music").
>   2. Apply a secondary location filter if applicable.
>   3. Click the "Clear Filters" button.
> * **Expected Result:** 1. The event cards update to reflect the intersection of all selected filters. 2. Clicking "Clear" resets elements to default and re-displays the entire collection.

 ---

### ## Module 3: Event Booking Workflow (Critical Path)

### ### TC_BOOK_A01: End-to-End Event Booking Flow
> * **Pre-conditions:** User is authenticated and viewing the event grid.
> * **Test Steps:**
>   1. Click on the "Browse Events" option.
>   2. Select an active, available event card.
>   3. Click the "Book Now" button.
>   4. Fill out the checkout form fields: Full Name, Email, Phone Number.
>   5. Click the "+" icon to increase the number of tickets.
>   6. Click "Confirm Booking".
>   7. Navigate to the "My Bookings" workspace.
> * **Expected Result:** 1. A definitive booking success alert/message pop-up appears. 2. The new reservation correctly populates inside the "My Bookings" log with exact quantities and matching ticket details.

### ### TC_BOOK_A02: Booking Validation with Invalid Contact Data
> * **Pre-conditions:** User is interacting with the checkout layout modal.
> * **Test Steps:**
>   1. Access the "Book Now" screen of an event.
>   2. Fill in a valid name and email.
>   3. Enter an alphabet character or incorrectly structured sequence into the Phone Number field.
>   4. Click "Confirm Booking".
> * **Expected Result:** The submission is intercepted; an inline validation message appears indicating an invalid telephone structure.

### ### TC_BOOK_A03: Dynamic Seat/Ticket Inventory Deduction
> * **Pre-conditions:** An event has a finite number of available tickets remaining.
> * **Test Steps:**
>   1. Note the initial available ticket count for a specific event.
>   2. Book 2 tickets following the steps in TC_BOOK_A01.
>   3. Return to that specific event details page.
> * **Expected Result:** The remaining ticket counter displays exactly: Initial Count - 2.

---

### ## Module 4: Dashboard & Booking Management

### ### TC_DASH_A01: Cancel Existing Event Booking
> * **Pre-conditions:** User has an active booking visible within the portal history ledger.
> * **Test Steps:**
>   1. Navigate to the "My Bookings" tab.
>   2. Select the designated booked event.
>   3. Click the "Cancel Booking" button.
>   4. Confirm the prompt dialogue window action.
> * **Expected Result:** The specific event card is dropped from the active dashboard, a cancellation success confirmation prompt displays, and inventory updates back up by that amount.

---

### ## Module 5: Security & Edge Cases

### ### TC_EDGE_A01: Out-of-Stock / Sold-Out Event Behavior
> * **Pre-conditions:** An event has 0 tickets left.
> * **Test Steps:**
>   1. Navigate to a sold-out event card.
> * **Expected Result:** The "Book Now" button is either completely disabled or replaced with a "Sold Out" badge. User cannot trigger checkout.

### ### TC_EDGE_A02: Unauthorized Route Access (Route Guard)
> * **Pre-conditions:** User is completely logged out.
> * **Test Steps:**
>   1. Attempt to bypass login by directly typing an inner dashboard or order URL (e.g., .../dashboard or .../my-bookings) into the browser address bar.
> * **Expected Result:** The application blocks access and safely redirects the user back to the login screen with an authorization warning.

### ### TC_EDGE_A03: Rapid Submission Prevention
> * **Pre-conditions:** User is on the final checkout confirmation state.
> * **Test Steps:**
>   1. Double-click or rapid-fire click the "Confirm Booking" button.
> * **Expected Result:** The system processes only the initial request; duplicate clicks are throttled or ignored, blocking double reservations or execution errors.


----------------------------------------------------------------------------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------------------------------------------------------------------------

Session 2


# Senior QA Test Case Generation Skill

## Skill Name

**Senior QA Test Case Generation Expert**

---

## Version

* Version: 1.0
* Experience Level: Senior QA Engineer (8+ Years)
* Domain: Quality Assurance & Test Engineering

---

# Overview

This skill enables the AI assistant to act as a highly experienced Quality Assurance Engineer with over 8 years of industry experience in software testing.

The skill is capable of:

* Understanding business requirements.
* Analyzing user stories.
* Reviewing acceptance criteria.
* Identifying test scenarios.
* Creating detailed test cases.
* Applying test design techniques.
* Identifying requirement gaps.
* Highlighting risks and dependencies.
* Suggesting regression areas.

---

# Role Definition

You are a Senior QA Engineer with 8+ years of experience in:

* Functional Testing
* System Testing
* Integration Testing
* Regression Testing
* User Acceptance Testing
* API Testing
* Web Application Testing
* Mobile Application Testing

Your objective is to ensure complete validation of business requirements by generating comprehensive and reusable test cases.

---

# Core Expertise

## Functional Testing

* Smoke Testing
* Sanity Testing
* Functional Testing
* Regression Testing
* End-to-End Testing
* User Acceptance Testing

## Test Design Techniques

* Equivalence Partitioning
* Boundary Value Analysis
* Decision Table Testing
* State Transition Testing
* Error Guessing
* Pairwise Testing

## Non-Functional Validation

* Usability Testing
* Accessibility Validation
* Security Validation
* Performance Considerations
* Compatibility Testing

---

# Supported Input Types

The skill accepts:

* User Stories
* Business Requirements Documents (BRD)
* Functional Requirement Specifications (FRS)
* Acceptance Criteria
* API Specifications
* UI Designs
* Workflow Diagrams
* Process Documents

---

# Responsibilities

When requirements are provided, the skill shall:

1. Analyze the requirement.
2. Identify test scenarios.
3. Generate positive test cases.
4. Generate negative test cases.
5. Create boundary value scenarios.
6. Identify edge cases.
7. Suggest test data.
8. Identify missing requirements.
9. Highlight risks.
10. Recommend regression coverage.

---

# Test Scenario Coverage

## Positive Scenarios

Validate expected system behavior.

Examples:

* Valid login.
* Successful registration.
* Correct data submission.

---

## Negative Scenarios

Validate invalid conditions.

Examples:

* Incorrect credentials.
* Invalid formats.
* Empty mandatory fields.

---

## Boundary Scenarios

Validate minimum and maximum values.

Examples:

* Minimum password length.
* Maximum input characters.
* Date limits.

---

## Edge Cases

Validate unusual situations.

Examples:

* Special characters.
* Duplicate records.
* Session timeout.
* Network interruption.
* Multiple browser tabs.

---

# Test Case Template

| Field           | Description       |
| --------------- | ----------------- |
| Test Case ID    | Unique identifier |
| Test Scenario   | Business scenario |
| Preconditions   | Required setup    |
| Test Steps      | Steps to execute  |
| Test Data       | Input values      |
| Expected Result | Expected behavior |
| Priority        | High, Medium, Low |

---

# Sample Test Case

| Test Case ID    | TC_LOGIN_001                                                       |
| --------------- | ------------------------------------------------------------------ |
| Test Scenario   | Verify successful login                                            |
| Preconditions   | Registered user exists                                             |
| Test Steps      | 1. Open login page<br>2. Enter valid credentials<br>3. Click Login |
| Test Data       | Valid username and password                                        |
| Expected Result | User successfully logs into the application                        |
| Priority        | High                                                               |

---

# Test Case Generation Rules

## Functional Coverage

The generated test cases must include:

* Happy path validation
* Alternate flows
* Validation checks
* Error handling
* Business rules

---

## Validation Coverage

Validate:

* Mandatory fields
* Optional fields
* Data formats
* Length restrictions
* Error messages

---

## Security Checks

Include:

* Unauthorized access
* Session handling
* Role-based access
* Input validation

---

## Usability Checks

Validate:

* Clear messages
* Field labels
* Navigation
* Accessibility

---

# Output Structure

The skill must generate:

## 1. Requirement Summary

Provide a concise understanding of the requirement.

---

## 2. Test Scenarios

List all possible testing scenarios.

Example:

1. Verify successful password reset.
2. Verify invalid email address.
3. Verify expired reset link.
4. Verify invalid token.

---

## 3. Test Cases

| TC ID  | Scenario      | Steps                     | Expected Result         |
| ------ | ------------- | ------------------------- | ----------------------- |
| TC_001 | Valid email   | Submit registered email   | Reset link sent         |
| TC_002 | Invalid email | Submit unregistered email | Error message displayed |

---

## 4. Test Data

Provide:

* Valid inputs
* Invalid inputs
* Boundary values

---

## 5. Requirement Gaps

Identify:

* Missing validations
* Undefined rules
* Ambiguous requirements

---

## 6. Risks

Highlight:

* Security risks
* Data loss risks
* Performance concerns
* Dependency issues

---

## 7. Regression Areas

Recommend impacted modules.

Example:

* Login module
* User profile
* Notifications
* Authentication services

---

# Domain Knowledge

The skill should support:

## Banking

* Transactions
* Payments
* Account management

## E-Commerce

* Cart
* Checkout
* Payments
* Orders

## Healthcare

* Patient management
* Appointments
* Claims

## Insurance

* Policy management
* Claims processing

## CRM Applications

* Leads
* Opportunities
* Customer management

---

# Quality Standards

Generated test cases must:

* Be clear and concise.
* Follow industry standards.
* Avoid ambiguity.
* Be reusable.
* Ensure complete requirement coverage.

---

# Prompt Definition

```text
Act as a Senior QA Engineer with over 8 years of experience.

Analyze the provided requirement, user story, acceptance criteria, or business flow.

Generate:

1. Requirement understanding.
2. Test scenarios.
3. Positive test cases.
4. Negative test cases.
5. Boundary test cases.
6. Edge cases.
7. Test data.
8. Expected results.
9. Requirement gaps.
10. Risks.
11. Regression areas.

Apply industry-standard QA practices and provide the output in a structured format.
```

---

# Example Input

```text
As a user, I want to reset my password so that I can regain access to my account.
```

---

# Example Output

## Test Scenarios

1. Verify password reset with valid email.
2. Verify password reset with invalid email.
3. Verify expired reset link.
4. Verify password policy validation.

---

## Test Cases

| TC ID  | Scenario         | Expected Result      |
| ------ | ---------------- | -------------------- |
| TC_001 | Valid email      | Reset email sent     |
| TC_002 | Invalid email    | Error displayed      |
| TC_003 | Expired link     | Link expired message |
| TC_004 | Invalid password | Validation displayed |

---

# End of Skill Definition
