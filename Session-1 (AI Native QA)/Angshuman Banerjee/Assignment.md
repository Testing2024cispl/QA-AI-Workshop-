QA MANUAL TEST CASES
Member : Angshuman Banerjee
Target Application : https://eventhub.rahulshettyacademy.com/login
------------------------------------------------
SECTION 1 : TEST CASES MADE BY HUMAN THINKING -
=================================================
### Scenario 1: Old User Login

**Testcase_ID:** LOGIN_BLANK_CREDENTIALS_001
**Test Scenario:** Verify login with blank email and password.

**Test Steps:**

1. Open the login page.
2. Leave Email and Password blank.
3. Click Sign In.

**Expected Result:**
Validation errors displayed; login blocked.

---

**Testcase_ID:** LOGIN_VALID_CREDENTIALS_002
**Test Scenario:** Verify login with valid credentials.

**Test Steps:**

1. Enter valid registered email and password.
2. Click Sign In.

**Expected Result:**
User redirected to dashboard.

---

**Testcase_ID:** LOGIN_INVALID_EMAIL_003
**Test Scenario:** Verify login with invalid email and valid password.

**Test Steps:**

1. Enter invalid email and valid password.
2. Click Sign In.

**Expected Result:**
Error message for invalid credentials.

---

**Testcase_ID:** LOGIN_INVALID_PASSWORD_004
**Test Scenario:** Verify login with valid email and invalid password.

**Test Steps:**

1. Enter valid email and invalid password.
2. Click Sign In.

**Expected Result:**
Error message for invalid credentials.

---

**Testcase_ID:** LOGIN_INVALID_CREDENTIALS_005
**Test Scenario:** Verify login with invalid email and invalid password.

**Test Steps:**

1. Enter invalid email and invalid password.
2. Click Sign In.

**Expected Result:**
Login denied with error message.

---

## Scenario 2: Manage Event in Admin Section

**Testcase_ID:** ADMIN_EVENT_PAGE_ACCESS_001
**Test Scenario:** Verify event management page access.

**Test Steps:**

1. Login as admin.
2. Navigate to Events page.

**Expected Result:**
Events page displayed.

---

**Testcase_ID:** ADMIN_EVENT_ACTION_BUTTONS_VISIBLE_002
**Test Scenario:** Verify action buttons visibility.

**Test Steps:**

1. Locate All Events table.

**Expected Result:**
Edit and Delete buttons visible.

---

**Testcase_ID:** ADMIN_EVENT_ACTION_BUTTONS_CLICKABLE_003
**Test Scenario:** Verify action buttons are clickable.

**Test Steps:**

1. Click Edit button.
2. Click Delete button.

**Expected Result:**
Buttons respond appropriately.

---

**Testcase_ID:** ADMIN_EVENT_EDIT_NAVIGATION_004
**Test Scenario:** Verify edit event navigation.

**Test Steps:**

1. Click Edit on an event.

**Expected Result:**
Event form opens with existing data.

---

**Testcase_ID:** ADMIN_CANCEL_EDIT_VISIBLE_005
**Test Scenario:** Verify Cancel Edit button visibility.

**Test Steps:**

1. Open event in edit mode.

**Expected Result:**
Cancel Edit button displayed.

---

**Testcase_ID:** ADMIN_CANCEL_EDIT_FUNCTIONALITY_006
**Test Scenario:** Verify Cancel Edit functionality.

**Test Steps:**

1. Click Cancel Edit.

**Expected Result:**
Changes discarded and form reset.

---

**Testcase_ID:** ADMIN_DELETE_EVENT_007
**Test Scenario:** Verify event deletion.

**Test Steps:**

1. Click Delete for an event.

**Expected Result:**
Event removed successfully.

---

**Testcase_ID:** ADMIN_UPDATE_EVENT_008
**Test Scenario:** Verify event update.

**Test Steps:**

1. Modify event details.
2. Click Update.

**Expected Result:**
Changes saved successfully.

---

**Testcase_ID:** ADMIN_EMPTY_EVENTS_TABLE_009
**Test Scenario:** Verify empty events table.

**Test Steps:**

1. Ensure no events exist.

**Expected Result:**
Blank state displayed.

---

**Testcase_ID:** ADMIN_UPDATED_EVENT_DATA_DISPLAY_010
**Test Scenario:** Verify updated event data in table.

**Test Steps:**

1. Edit event.
2. Save event.

**Expected Result:**
Updated values displayed.

---

**Testcase_ID:** ADMIN_DELETED_EVENT_NOT_VISIBLE_011
**Test Scenario:** Verify deleted event not displayed.

**Test Steps:**

1. Delete event.
2. Refresh page.

**Expected Result:**
Deleted event absent.

---

**Testcase_ID:** ADMIN_NO_ACTION_BUTTONS_EMPTY_TABLE_012
**Test Scenario:** Verify action buttons hidden when no events.

**Test Steps:**

1. View empty table.

**Expected Result:**
No Edit/Delete buttons shown.

---

## Scenario 3: Create New Event

**Testcase_ID:** EVENT_USER_LOGIN_PRECHECK_001
**Test Scenario:** Verify user login before event creation.

**Test Steps:**

1. Login to application.

**Expected Result:**
User authenticated.

---

**Testcase_ID:** EVENT_DASHBOARD_VISIBILITY_002
**Test Scenario:** Verify dashboard visibility.

**Test Steps:**

1. Login successfully.

**Expected Result:**
Dashboard displayed.

---

**Testcase_ID:** EVENT_NAVIGATION_TO_EVENTS_PAGE_003
**Test Scenario:** Verify navigation to Events page.

**Test Steps:**

1. Click Events menu.

**Expected Result:**
Events page opens.

---

**Testcase_ID:** EVENT_ADD_NEW_BUTTON_VISIBLE_004
**Test Scenario:** Verify Add New Event button visibility.

**Test Steps:**

1. Open Events page.

**Expected Result:**
Add New Event button visible.

---

**Testcase_ID:** EVENT_ADD_NEW_BUTTON_FUNCTIONALITY_005
**Test Scenario:** Verify Add New Event button functionality.

**Test Steps:**

1. Click Add New Event.

**Expected Result:**
Event form opens.

---

**Testcase_ID:** EVENT_REDIRECT_TO_FORM_006
**Test Scenario:** Verify redirect to event form.

**Test Steps:**

1. Click Add button.

**Expected Result:**
Manage Event form displayed.

---

**Testcase_ID:** EVENT_MANDATORY_FIELD_VALIDATION_007
**Test Scenario:** Verify mandatory field validation.

**Test Steps:**

1. Leave required fields blank.
2. Submit form.

**Expected Result:**
Validation errors shown.

---

**Testcase_ID:** EVENT_OPTIONAL_FIELDS_BLANK_008
**Test Scenario:** Verify optional fields can be blank.

**Test Steps:**

1. Leave optional fields empty.
2. Submit valid form.

**Expected Result:**
Event creation allowed.

---

**Testcase_ID:** EVENT_CURRENT_DATE_RESTRICTION_009
**Test Scenario:** Verify current date restriction.

**Test Steps:**

1. Enter current date as event date.

**Expected Result:**
Creation blocked if future date required.

---

**Testcase_ID:** EVENT_ZERO_SEATS_VALIDATION_010
**Test Scenario:** Verify total seats cannot be zero.

**Test Steps:**

1. Enter 0 seats.
2. Submit form.

**Expected Result:**
Validation error displayed.

---

**Testcase_ID:** EVENT_ZERO_PRICE_VALIDATION_011
**Test Scenario:** Verify event price cannot be zero.

**Test Steps:**

1. Enter 0 price.
2. Submit form.

**Expected Result:**
Validation error displayed.

---

**Testcase_ID:** EVENT_CITY_VENUE_VALIDATION_012
**Test Scenario:** Verify city and venue validation.

**Test Steps:**

1. Enter invalid city value.
2. Enter invalid venue value.

**Expected Result:**
Validation error displayed.

---

**Testcase_ID:** EVENT_SUCCESSFUL_CREATION_013
**Test Scenario:** Verify successful event creation.

**Test Steps:**

1. Enter valid event data.
2. Submit form.

**Expected Result:**
Success notification displayed.

---

## Scenario 4: New User Creation

**Testcase_ID:** USER_REGISTRATION_PAGE_ACCESS_001
**Test Scenario:** Verify registration page access.

**Test Steps:**

1. Click Register link.

**Expected Result:**
Registration form displayed.

---

**Testcase_ID:** USER_DUPLICATE_EMAIL_VALIDATION_002
**Test Scenario:** Verify duplicate email validation.

**Test Steps:**

1. Register using existing email.

**Expected Result:**
Email already registered error.

---

**Testcase_ID:** USER_PASSWORD_POLICY_VALIDATION_003
**Test Scenario:** Verify password policy.

**Test Steps:**

1. Enter invalid password format (such as all consecutive numbers).

**Expected Result:**
Validation error displayed.

---

**Testcase_ID:** USER_NEW_ACCOUNT_REGISTRATION_004
**Test Scenario:** Verify registration with new email.

**Test Steps:**

1. Enter valid new user data.

**Expected Result:**
Account created successfully.

---

**Testcase_ID:** USER_CONFIRM_PASSWORD_REQUIRED_005
**Test Scenario:** Verify confirm password requirement.

**Test Steps:**

1. Leave confirm password blank.

**Expected Result:**
Validation error displayed.

---

**Testcase_ID:** USER_REGISTRATION_SUCCESS_MESSAGE_006
**Test Scenario:** Verify registration success message.

**Test Steps:**

1. Complete registration.

**Expected Result:**
Success message displayed.

---

**Testcase_ID:** USER_DASHBOARD_ACCESS_AFTER_REGISTRATION_007
**Test Scenario:** Verify dashboard access after registration.

**Test Steps:**

1. Register successfully.

**Expected Result:**
User redirected to dashboard.

---

## Scenario 5: Verify Event Appears in List

**Testcase_ID:** EVENT_LIST_NEW_EVENT_VISIBLE_001
**Test Scenario:** Verify newly created event in All Events table.

**Test Steps:**

1. Create event.
2. Open All Events table.

**Expected Result:**
Event appears in list.

---

**Testcase_ID:** EVENT_LIST_DATA_ACCURACY_002
**Test Scenario:** Verify event data accuracy in the table.

**Test Steps:**

1. Compare created event data with table values.

**Expected Result:**
Displayed data matches created data.

==========================================
SECTION 2 : AI CREATED MANUAL TEST CASES
------------------------------------------
PROMPT GIVEN: 
------------------------------------------
Act as a senior test engineer specialized with functional testing and UI/UX testing for web applications.
URL TO BE TESTED: https://eventhub.rahulshettyacademy.com/.
APPLICATION CONTEXT:
a. EventHub is an event booking platform with the following core functionality:
b. Users can register/create a profile and log in.
c. Logged-in users can browse listed events and book them.
d. A "My Bookings" section lets users view events they have booked.
e. An Admin section allows authorized users to create and manage new events.

SCENARIO TO BE COVERED (END-TO-END FLOW) Write test cases covering this user journey, broken down into its individual stages:
a. New user registration/account creation.
b. Admin login and navigation to the event management section.
c. Admin creates a new event (with all required event details).
d. Verification that the newly created event appears in that user's event listing.
e. Manage Event in Admin Section.
f. Old User Login.

TASK: Generate a complete manual test suite for the above scenarios on the Eventhub website. Do not duplicate the same test cases.
NOTE: Show the result in the below format-
TESTCASE_ID:
Test Scenario:
Test Steps:
Expected Result:
-------------------------
RESULT OF THE PROMPT:
-------------------------
Below is a comprehensive **Manual Functional & UI/UX Test Suite** for the requested **EventHub End-to-End User Journey**. Test cases are organized by stage and avoid duplication.

---

# New User Registration / Account Creation

### TESTCASE_ID:001

**Test Scenario:** Verify successful new user registration with valid data

**Test Steps:**

1. Navigate to EventHub website.
2. Click on Register/Sign Up.
3. Enter valid First Name, Last Name, Email, Password, and required fields.
4. Click Register/Create Account.

**Expected Result:**

* Account is created successfully.
* Success message is displayed.
* User is redirected to login/dashboard page.

---

### TESTCASE_ID:002

**Test Scenario:** Verify mandatory field validation during registration

**Test Steps:**

1. Open Registration page.
2. Leave all mandatory fields blank.
3. Click Register.

**Expected Result:**

* Appropriate validation messages are displayed for all required fields.
* Registration is not completed.

---

### TESTCASE_ID:003

**Test Scenario:** Verify registration with already registered email address

**Test Steps:**

1. Open Registration page.
2. Enter an email already registered in the system.
3. Fill remaining fields with valid data.
4. Submit registration.

**Expected Result:**

* Registration is blocked.
* Message indicates email already exists.

---

### TESTCASE_ID:004

**Test Scenario:** Verify email format validation

**Test Steps:**

1. Open Registration page.
2. Enter invalid email format (e.g., testgmail.com).
3. Complete remaining fields.
4. Submit registration.

**Expected Result:**

* Invalid email validation message is displayed.
* Registration is prevented.

---

### TESTCASE_ID:005

**Test Scenario:** Verify password policy validation

**Test Steps:**

1. Open Registration page.
2. Enter password not meeting required criteria.
3. Fill remaining details.
4. Submit registration.

**Expected Result:**

* Password policy error message is displayed.
* User cannot register until valid password is entered.

---

### TESTCASE_ID:006

**Test Scenario:** Verify UI alignment and usability of registration page

**Test Steps:**

1. Open Registration page.
2. Inspect labels, input fields, buttons, placeholders, and page layout.

**Expected Result:**

* All UI elements are properly aligned.
* Labels are readable.
* No overlapping or broken components are visible.

---

# Admin Login and Navigation

### TESTCASE_ID: 001

**Test Scenario:** Verify successful admin login

**Test Steps:**

1. Open Login page.
2. Enter valid admin credentials.
3. Click Login.

**Expected Result:**

* Admin is logged in successfully.
* Admin dashboard is displayed.

---

### TESTCASE_ID:002

**Test Scenario:** Verify login with invalid admin credentials

**Test Steps:**

1. Open Login page.
2. Enter invalid username/password.
3. Click Login.

**Expected Result:**

* Login fails.
* Appropriate error message is displayed.

---

### TESTCASE_ID:003

**Test Scenario:** Verify navigation to Event Management section

**Test Steps:**

1. Login as Admin.
2. Navigate through dashboard menu.
3. Select Event Management section.

**Expected Result:**

* Event Management page opens successfully.
* Existing events are displayed.

---

### TESTCASE_ID:004

**Test Scenario:** Verify admin menu accessibility

**Test Steps:**

1. Login as Admin.
2. Verify all available menu options.

**Expected Result:**

* All admin functions are visible and accessible.
* Navigation works correctly.

---

# Admin Creates New Event

### TESTCASE_ID:001

**Test Scenario:** Verify successful event creation with valid details

**Test Steps:**

1. Login as Admin.
2. Navigate to Event Management.
3. Click Create Event.
4. Enter all mandatory event details.
5. Save event.

**Expected Result:**

* Event is created successfully.
* Success confirmation message is displayed.

---

### TESTCASE_ID:002

**Test Scenario:** Verify mandatory field validation during event creation

**Test Steps:**

1. Open Create Event page.
2. Leave required fields empty.
3. Click Save.

**Expected Result:**

* Validation messages appear.
* Event is not created.

---

### TESTCASE_ID:003

**Test Scenario:** Verify event creation with past event date

**Test Steps:**

1. Create a new event.
2. Select a date in the past.
3. Save event.

**Expected Result:**

* System prevents creation.
* Appropriate validation message is displayed.

---

### TESTCASE_ID:004

**Test Scenario:** Verify event image upload functionality

**Test Steps:**

1. Open Create Event page.
2. Upload valid image file.
3. Save event.

**Expected Result:**

* Image uploads successfully.
* Event is created with image attached.

---

### TESTCASE_ID:005

**Test Scenario:** Verify event details are saved correctly

**Test Steps:**

1. Create event with title, description, venue, date, and capacity.
2. Save event.
3. Reopen created event.

**Expected Result:**

* All entered details are stored accurately.

---

### TESTCASE_ID:006

**Test Scenario:** Verify UI/UX of event creation page

**Test Steps:**

1. Open Create Event page.
2. Verify form design, field alignment, button visibility, and responsiveness.

**Expected Result:**

* Form is user-friendly.
* Fields and buttons are properly aligned and accessible.

---

# Verify Newly Created Event Appears in User Event Listing

### TESTCASE_ID: 001

**Test Scenario:** Verify newly created event is visible in event listing

**Test Steps:**

1. Login as normal user.
2. Navigate to Events page.
3. Search for newly created event.

**Expected Result:**

* Newly created event appears in listing.

---

### TESTCASE_ID:002

**Test Scenario:** Verify event details displayed correctly in listing

**Test Steps:**

1. Open event listing.
2. Locate newly created event.
3. Verify displayed information.

**Expected Result:**

* Event title, date, venue, and image match admin-created data.

---

### TESTCASE_ID:003

**Test Scenario:** Verify event search functionality

**Test Steps:**

1. Navigate to event listing.
2. Search using event name.
3. Execute search.

**Expected Result:**

* Matching event appears in search results.

---

### TESTCASE_ID:004

**Test Scenario:** Verify event detail page accessibility

**Test Steps:**

1. Click newly created event.
2. Open event detail page.

**Expected Result:**

* Event detail page loads successfully.
* Complete event information is displayed.

---

# Manage Event in Admin Section

### TESTCASE_ID:001

**Test Scenario:** Verify admin can edit event details

**Test Steps:**

1. Login as Admin.
2. Navigate to Event Management.
3. Select created event.
4. Edit event information.
5. Save changes.

**Expected Result:**

* Event details are updated successfully.

---

### TESTCASE_ID:002

**Test Scenario:** Verify edited event information reflects in user listing

**Test Steps:**

1. Modify event details as Admin.
2. Login as User.
3. View event listing.

**Expected Result:**

* Updated event information is displayed.

---

### TESTCASE_ID:003

**Test Scenario:** Verify admin can deactivate/cancel event

**Test Steps:**

1. Login as Admin.
2. Open Event Management.
3. Select event.
4. Mark event as inactive/cancelled.

**Expected Result:**

* Event status changes successfully.
* Appropriate confirmation message appears.

---

### TESTCASE_ID:004

**Test Scenario:** Verify inactive event visibility behavior

**Test Steps:**

1. Deactivate event.
2. Login as User.
3. Check event listing.

**Expected Result:**

* Event follows defined business rule (hidden or marked inactive).

---

### TESTCASE_ID:005

**Test Scenario:** Verify event deletion functionality

**Test Steps:**

1. Login as Admin.
2. Select event.
3. Click Delete.
4. Confirm deletion.

**Expected Result:**

* Event is deleted successfully.
* Event no longer appears in management list.

---

### TESTCASE_ID:006

**Test Scenario:** Verify delete confirmation popup behavior

**Test Steps:**

1. Attempt to delete event.
2. Observe confirmation popup.
3. Click Cancel.

**Expected Result:**

* Event remains unchanged.
* Deletion is not executed.

---
# Old User Login and Event Booking

### TESTCASE_ID:001

**Test Scenario:** Verify existing user login

**Test Steps:**

1. Open Login page.
2. Enter valid existing user credentials.
3. Click Login.

**Expected Result:**

* User logs in successfully.
* User dashboard is displayed.

---

### TESTCASE_ID:002

**Test Scenario:** Verify booking newly created event

**Test Steps:**

1. Login as existing user.
2. Open newly created event.
3. Click Book Event.
4. Complete booking process.

**Expected Result:**

* Booking is successful.
* Confirmation message is displayed.

---

### TESTCASE_ID:003

**Test Scenario:** Verify booked event appears in My Bookings

**Test Steps:**

1. Complete event booking.
2. Navigate to My Bookings.

**Expected Result:**

* Newly booked event is displayed in My Bookings section.

---

### TESTCASE_ID:004

**Test Scenario:** Verify booking details accuracy

**Test Steps:**

1. Open My Bookings.
2. Select booked event.

**Expected Result:**

* Event name, date, venue, and booking information are correct.

---

### TESTCASE_ID:005

**Test Scenario:** Verify booking duplicate event behavior

**Test Steps:**

1. Book an event.
2. Attempt booking same event again.

**Expected Result:**

* System follows business rule:

  * Prevents duplicate booking OR
  * Displays duplicate booking warning.

---

### TESTCASE_ID:006

**Test Scenario:** Verify My Bookings page UI/UX

**Test Steps:**

1. Navigate to My Bookings.
2. Review page layout and booking cards.

**Expected Result:**

* Bookings are clearly displayed.
* Page is responsive and easy to navigate.

---

# End-to-End Validation

### TESTCASE_ID:001

**Test Scenario:** Verify complete end-to-end EventHub workflow

**Test Steps:**

1. Register a new user account.
2. Login as Admin.
3. Create a new event.
4. Logout Admin.
5. Login as existing user.
6. Verify event appears in event listing.
7. Book the event.
8. Open My Bookings.
9. Verify booking details.
10. Login as Admin and edit event.
11. Verify updates are reflected for user.

**Expected Result:**

* Entire workflow executes successfully without functional or UI issues.
* Data consistency is maintained across Admin and User modules.
  
-------------------------------------------------------------------
MY THOUGHTS ON BOTH USER [HUMAN AND AI] CREATED TEST CASE DOCUMENT:
-------------------------------------------------------------------
###  What I felt suitable:- (Compared to a Human-Created Test Suite)

* Covers the complete end-to-end business flow: Registration → Admin Event Creation → Event Management → User Booking → My Bookings.
* Includes both positive and negative scenarios (valid/invalid registration, login validation, mandatory field checks).
* Well-structured format with clear Test Case IDs, Steps, and Expected Results.
* Avoids major duplication and keeps scenarios logically separated.
* Includes basic UI/UX validation alongside functional testing.
* Easy to understand, review, and execute for manual testers.
* Provides a solid baseline for smoke testing, UAT, and initial regression coverage.

### What I felt not suitable:- (Compared to a Human-Created Test Suite)

* Lacks preconditions, test data, priority, severity, and requirement traceability.
* Limited boundary value and edge-case testing (field lengths, capacity limits, date validations).
* Missing security and authorization scenarios (role access, session timeout, URL manipulation).
* Event management coverage is not deep enough (capacity updates, booked-event deletion impacts, status transitions).
* Minimal search, filter, sorting, and booking edge-case coverage.
* UI/UX checks are generic rather than detailed and measurable.
* No cross-browser, responsive, accessibility, performance, or concurrency testing.
* A human QA would typically expand this into a more comprehensive, production-ready regression suite.
---------------------------------------------------------
FINAL TEST CASES (AI+HUMAN) COMBINED - AUTOMATION READY:
---------------------------------------------------------
# Final Automation-Ready Test Suite – EventHub

The following test cases combine **AI-generated coverage + Senior QA best practices**, making them suitable for **manual execution, Selenium, Playwright, Cypress, or API automation frameworks**.

---

## Registration Module

### Testcase_ID: REG_001_VALID_REGISTRATION

**Test Scenario:** Verify successful registration with valid user details

**Test Steps:**

1. Navigate to Registration page.
2. Enter unique email.
3. Enter password meeting policy requirements.
4. Enter matching Confirm Password.
5. Click Create Account.

**Expected Result:**

* User account is created successfully.
* Success message is displayed.
* User is redirected to Login/Home page.

---

### Testcase_ID: REG_002_REQUIRED_FIELD_VALIDATION

**Test Scenario:** Verify mandatory field validation on registration form

**Test Steps:**

1. Open Registration page.
2. Leave all fields blank.
3. Click Create Account.

**Expected Result:**

* Validation messages appear for all mandatory fields.
* Registration is blocked.

---

### Testcase_ID: REG_003_DUPLICATE_EMAIL

**Test Scenario:** Verify registration with existing email

**Test Steps:**

1. Open Registration page.
2. Enter an already registered email.
3. Enter valid password and confirm password.
4. Submit form.

**Expected Result:**

* Registration is rejected.
* Appropriate duplicate email message is displayed.

---

### Testcase_ID: REG_004_PASSWORD_POLICY

**Test Scenario:** Verify password policy enforcement

**Test Steps:**

1. Enter password without uppercase, special character, or required length.
2. Submit registration.

**Expected Result:**

* Password policy validation is displayed.
* Account is not created. ([EventHub][1])

---

### Testcase_ID: REG_005_PASSWORD_CONFIRMATION

**Test Scenario:** Verify password and confirm password mismatch validation

**Test Steps:**

1. Enter valid password.
2. Enter different Confirm Password.
3. Submit registration.

**Expected Result:**

* Password mismatch error is displayed.
* Registration is prevented.

---

## Login Module

### Testcase_ID: LOGIN_001_VALID_USER_LOGIN

**Test Scenario:** Verify successful login for registered user

**Test Steps:**

1. Open Login page.
2. Enter valid email and password.
3. Click Sign In.

**Expected Result:**

* User is successfully logged in.
* Dashboard/Home page loads. ([EventHub][2])

---

### Testcase_ID: LOGIN_002_INVALID_CREDENTIALS

**Test Scenario:** Verify login with invalid credentials

**Test Steps:**

1. Enter invalid email/password.
2. Click Sign In.

**Expected Result:**

* Login fails.
* Error message is displayed.

---

### Testcase_ID: LOGIN_003_SESSION_LOGOUT

**Test Scenario:** Verify logout functionality

**Test Steps:**

1. Login successfully.
2. Click Logout.
3. Try navigating back using browser Back button.

**Expected Result:**

* User remains logged out.
* Protected pages are inaccessible.

---

## Admin Event Management

### Testcase_ID: ADMIN_001_ACCESS_EVENT_MANAGEMENT

**Test Scenario:** Verify admin can access Event Management module

**Test Steps:**

1. Login as Admin.
2. Navigate to Event Management.

**Expected Result:**

* Event Management page loads successfully.

---

### Testcase_ID: ADMIN_002_CREATE_EVENT_VALID_DATA

**Test Scenario:** Verify event creation using valid data

**Test Steps:**

1. Open Create Event page.
2. Enter event title.
3. Enter description.
4. Select future date.
5. Enter venue.
6. Enter capacity.
7. Save event.

**Expected Result:**

* Event is created successfully.
* Event appears in Event Management list.

---

### Testcase_ID: ADMIN_003_CREATE_EVENT_REQUIRED_FIELDS

**Test Scenario:** Verify mandatory field validation during event creation

**Test Steps:**

1. Open Create Event page.
2. Leave required fields blank.
3. Save event.

**Expected Result:**

* Validation messages are displayed.
* Event creation is blocked.

---

### Testcase_ID: ADMIN_004_CREATE_EVENT_PAST_DATE

**Test Scenario:** Verify event creation with past date

**Test Steps:**

1. Create event using a past date.
2. Save event.

**Expected Result:**

* Event is not created.
* Date validation message is displayed.

---

### Testcase_ID: ADMIN_005_EDIT_EVENT

**Test Scenario:** Verify admin can update existing event

**Test Steps:**

1. Open existing event.
2. Modify title, venue, or date.
3. Save changes.

**Expected Result:**

* Event updates successfully.
* Modified details are persisted.

---

### Testcase_ID: ADMIN_006_DELETE_EVENT

**Test Scenario:** Verify admin can delete event

**Test Steps:**

1. Open Event Management.
2. Select event.
3. Click Delete.
4. Confirm deletion.

**Expected Result:**

* Event is removed from event list.

---

### Testcase_ID: ADMIN_007_DELETE_CONFIRMATION_POPUP

**Test Scenario:** Verify delete confirmation behavior

**Test Steps:**

1. Click Delete Event.
2. Click Cancel on confirmation dialog.

**Expected Result:**

* Event remains unchanged.
* No deletion occurs.

---

## Event Listing

### Testcase_ID: EVENT_001_EVENT_VISIBLE_TO_USERS

**Test Scenario:** Verify newly created event appears in event listing

**Test Steps:**

1. Create event as Admin.
2. Login as User.
3. Navigate to Events page.

**Expected Result:**

* Newly created event is visible.

---

### Testcase_ID: EVENT_002_EVENT_DETAILS_ACCURACY

**Test Scenario:** Verify event information displayed correctly

**Test Steps:**

1. Open event card.
2. Compare displayed details with admin-created data.

**Expected Result:**

* Event title, venue, date, and description match stored data.

---

### Testcase_ID: EVENT_003_SEARCH_EVENT_BY_NAME

**Test Scenario:** Verify search functionality

**Test Steps:**

1. Enter event name in search field.
2. Execute search.

**Expected Result:**

* Matching event is returned.

---

### Testcase_ID: EVENT_004_SEARCH_NON_EXISTING_EVENT

**Test Scenario:** Verify search behavior for invalid event name

**Test Steps:**

1. Search using non-existing event name.

**Expected Result:**

* No results message is displayed.

---

## Booking Module

### Testcase_ID: BOOK_001_SUCCESSFUL_EVENT_BOOKING

**Test Scenario:** Verify successful event booking

**Test Steps:**

1. Login as User.
2. Open available event.
3. Click Book Event.
4. Confirm booking.

**Expected Result:**

* Booking is successful.
* Confirmation message appears.

---

### Testcase_ID: BOOK_002_BOOKING_REFLECTS_IN_MY_BOOKINGS

**Test Scenario:** Verify booked event appears in My Bookings

**Test Steps:**

1. Book an event.
2. Open My Bookings.

**Expected Result:**

* Booked event is listed.

---

### Testcase_ID: BOOK_003_BOOKING_DETAILS_VERIFICATION

**Test Scenario:** Verify booking information accuracy

**Test Steps:**

1. Open My Bookings.
2. Open booked event.

**Expected Result:**

* Event name, venue, date, and booking status are correct.

---

### Testcase_ID: BOOK_004_DUPLICATE_BOOKING_VALIDATION

**Test Scenario:** Verify duplicate booking handling

**Test Steps:**

1. Book an event.
2. Attempt booking same event again.

**Expected Result:**

* Duplicate booking is prevented or warning message is displayed.

---

### Testcase_ID: BOOK_005_BOOK_EXPIRED_EVENT

**Test Scenario:** Verify booking restriction for expired events

**Test Steps:**

1. Open expired event.
2. Attempt booking.

**Expected Result:**

* Booking is blocked.

---

## Authorization & Security

### Testcase_ID: SEC_001_USER_ADMIN_URL_ACCESS

**Test Scenario:** Verify normal user cannot access admin pages

**Test Steps:**

1. Login as normal user.
2. Enter Admin URL directly.

**Expected Result:**

* Access denied or redirected.

---

### Testcase_ID: SEC_002_UNAUTHENTICATED_ACCESS

**Test Scenario:** Verify protected pages require authentication

**Test Steps:**

1. Do not login.
2. Open My Bookings URL.
3. Open Admin URL.

**Expected Result:**

* User is redirected to Login page.

---

## UI/UX Validation

### Testcase_ID: UI_001_REGISTRATION_PAGE_LAYOUT

**Test Scenario:** Verify registration page UI consistency

**Test Steps:**

1. Open Registration page.
2. Verify labels, input fields, buttons, and alignment.

**Expected Result:**

* UI elements are properly aligned and usable.

---

### Testcase_ID: UI_002_RESPONSIVE_EVENT_LISTING

**Test Scenario:** Verify event listing responsiveness

**Test Steps:**

1. Open Events page.
2. Test on Desktop, Tablet, and Mobile viewport.

**Expected Result:**

* Layout adjusts correctly without overlap or truncation.

---

### Testcase_ID: UI_003_ERROR_MESSAGE_USABILITY

**Test Scenario:** Verify validation messages are user-friendly

**Test Steps:**

1. Trigger validation errors on Registration/Login/Event forms.

**Expected Result:**

* Error messages are clearly visible and understandable.
---
## End-to-End Workflow

### Testcase_ID: E2E_001_COMPLETE_EVENT_LIFECYCLE

**Test Scenario:** Verify complete EventHub business workflow

**Test Steps:**

1. Register new user.
2. Login as Admin.
3. Create new event.
4. Verify event appears in listing.
5. Login as User.
6. Book event.
7. Verify booking in My Bookings.
8. Login as Admin.
9. Edit event.
10. Verify updates are reflected for user.

**Expected Result:**
* Entire workflow executes successfully with consistent data across all modules.





