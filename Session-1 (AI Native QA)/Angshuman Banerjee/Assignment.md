# QA MANUAL TEST CASES

**Member:** Angshuman Banerjee

**Application Under Test:** https://eventhub.rahulshettyacademy.com/login

---

## TABLE OF CONTENTS

1. [Section 1: Human-Created Test Cases](#section-1-human-created-test-cases)
   - [Scenario 1: Old User Login](#scenario-1-old-user-login)
   - [Scenario 2: Manage Event in Admin Section](#scenario-2-manage-event-in-admin-section)
   - [Scenario 3: Create New Event](#scenario-3-create-new-event)
   - [Scenario 4: New User Creation](#scenario-4-new-user-creation)
   - [Scenario 5: Verify Event Appears in List](#scenario-5-verify-event-appears-in-list)

2. [Section 2: AI-Created Test Cases](#section-2-ai-created-test-cases)

3. [Analysis and Recommendations](#analysis-and-recommendations)

4. [Final Automation-Ready Test Suite](#final-automation-ready-test-suite)

---

# SECTION 1: HUMAN-CREATED TEST CASES

## Scenario 1: Old User Login

### Testcase_ID: LOGIN_BLANK_CREDENTIALS_001

**Test Scenario:** Verify login with blank email and password.

**Test Steps:**
1. Open the login page.
2. Leave Email and Password blank.
3. Click Sign In.

**Expected Result:**
- Validation errors displayed
- Login blocked

---

### Testcase_ID: LOGIN_VALID_CREDENTIALS_002

**Test Scenario:** Verify login with valid credentials.

**Test Steps:**
1. Enter valid registered email and password.
2. Click Sign In.

**Expected Result:**
- User redirected to dashboard

---

### Testcase_ID: LOGIN_INVALID_EMAIL_003

**Test Scenario:** Verify login with invalid email and valid password.

**Test Steps:**
1. Enter invalid email and valid password.
2. Click Sign In.

**Expected Result:**
- Error message for invalid credentials displayed

---

### Testcase_ID: LOGIN_INVALID_PASSWORD_004

**Test Scenario:** Verify login with valid email and invalid password.

**Test Steps:**
1. Enter valid email and invalid password.
2. Click Sign In.

**Expected Result:**
- Error message for invalid credentials displayed

---

### Testcase_ID: LOGIN_INVALID_CREDENTIALS_005

**Test Scenario:** Verify login with invalid email and invalid password.

**Test Steps:**
1. Enter invalid email and invalid password.
2. Click Sign In.

**Expected Result:**
- Login denied with error message

---

## Scenario 2: Manage Event in Admin Section

### Testcase_ID: ADMIN_EVENT_PAGE_ACCESS_001

**Test Scenario:** Verify event management page access.

**Test Steps:**
1. Login as admin.
2. Navigate to Events page.

**Expected Result:**
- Events page displayed

---

### Testcase_ID: ADMIN_EVENT_ACTION_BUTTONS_VISIBLE_002

**Test Scenario:** Verify action buttons visibility.

**Test Steps:**
1. Locate All Events table.

**Expected Result:**
- Edit and Delete buttons visible

---

### Testcase_ID: ADMIN_EVENT_ACTION_BUTTONS_CLICKABLE_003

**Test Scenario:** Verify action buttons are clickable.

**Test Steps:**
1. Click Edit button.
2. Click Delete button.

**Expected Result:**
- Buttons respond appropriately

---

### Testcase_ID: ADMIN_EVENT_EDIT_NAVIGATION_004

**Test Scenario:** Verify edit event navigation.

**Test Steps:**
1. Click Edit on an event.

**Expected Result:**
- Event form opens with existing data

---

### Testcase_ID: ADMIN_CANCEL_EDIT_VISIBLE_005

**Test Scenario:** Verify Cancel Edit button visibility.

**Test Steps:**
1. Open event in edit mode.

**Expected Result:**
- Cancel Edit button displayed

---

### Testcase_ID: ADMIN_CANCEL_EDIT_FUNCTIONALITY_006

**Test Scenario:** Verify Cancel Edit functionality.

**Test Steps:**
1. Click Cancel Edit.

**Expected Result:**
- Changes discarded and form reset

---

### Testcase_ID: ADMIN_DELETE_EVENT_007

**Test Scenario:** Verify event deletion.

**Test Steps:**
1. Click Delete for an event.

**Expected Result:**
- Event removed successfully

---

### Testcase_ID: ADMIN_UPDATE_EVENT_008

**Test Scenario:** Verify event update.

**Test Steps:**
1. Modify event details.
2. Click Update.

**Expected Result:**
- Changes saved successfully

---

### Testcase_ID: ADMIN_EMPTY_EVENTS_TABLE_009

**Test Scenario:** Verify empty events table.

**Test Steps:**
1. Ensure no events exist.

**Expected Result:**
- Blank state displayed

---

### Testcase_ID: ADMIN_UPDATED_EVENT_DATA_DISPLAY_010

**Test Scenario:** Verify updated event data in table.

**Test Steps:**
1. Edit event.
2. Save event.

**Expected Result:**
- Updated values displayed

---

### Testcase_ID: ADMIN_DELETED_EVENT_NOT_VISIBLE_011

**Test Scenario:** Verify deleted event not displayed.

**Test Steps:**
1. Delete event.
2. Refresh page.

**Expected Result:**
- Deleted event absent

---

### Testcase_ID: ADMIN_NO_ACTION_BUTTONS_EMPTY_TABLE_012

**Test Scenario:** Verify action buttons hidden when no events.

**Test Steps:**
1. View empty table.

**Expected Result:**
- No Edit/Delete buttons shown

---

## Scenario 3: Create New Event

### Testcase_ID: EVENT_USER_LOGIN_PRECHECK_001

**Test Scenario:** Verify user login before event creation.

**Test Steps:**
1. Login to application.

**Expected Result:**
- User authenticated

---

### Testcase_ID: EVENT_DASHBOARD_VISIBILITY_002

**Test Scenario:** Verify dashboard visibility.

**Test Steps:**
1. Login successfully.

**Expected Result:**
- Dashboard displayed

---

### Testcase_ID: EVENT_NAVIGATION_TO_EVENTS_PAGE_003

**Test Scenario:** Verify navigation to Events page.

**Test Steps:**
1. Click Events menu.

**Expected Result:**
- Events page opens

---

### Testcase_ID: EVENT_ADD_NEW_BUTTON_VISIBLE_004

**Test Scenario:** Verify Add New Event button visibility.

**Test Steps:**
1. Open Events page.

**Expected Result:**
- Add New Event button visible

---

### Testcase_ID: EVENT_ADD_NEW_BUTTON_FUNCTIONALITY_005

**Test Scenario:** Verify Add New Event button functionality.

**Test Steps:**
1. Click Add New Event.

**Expected Result:**
- Event form opens

---

### Testcase_ID: EVENT_REDIRECT_TO_FORM_006

**Test Scenario:** Verify redirect to event form.

**Test Steps:**
1. Click Add button.

**Expected Result:**
- Manage Event form displayed

---

### Testcase_ID: EVENT_MANDATORY_FIELD_VALIDATION_007

**Test Scenario:** Verify mandatory field validation.

**Test Steps:**
1. Leave required fields blank.
2. Submit form.

**Expected Result:**
- Validation errors shown

---

### Testcase_ID: EVENT_OPTIONAL_FIELDS_BLANK_008

**Test Scenario:** Verify optional fields can be blank.

**Test Steps:**
1. Leave optional fields empty.
2. Submit valid form.

**Expected Result:**
- Event creation allowed

---

### Testcase_ID: EVENT_CURRENT_DATE_RESTRICTION_009

**Test Scenario:** Verify current date restriction.

**Test Steps:**
1. Enter current date as event date.

**Expected Result:**
- Creation blocked if future date required

---

### Testcase_ID: EVENT_ZERO_SEATS_VALIDATION_010

**Test Scenario:** Verify total seats cannot be zero.

**Test Steps:**
1. Enter 0 seats.
2. Submit form.

**Expected Result:**
- Validation error displayed

---

### Testcase_ID: EVENT_ZERO_PRICE_VALIDATION_011

**Test Scenario:** Verify event price cannot be zero.

**Test Steps:**
1. Enter 0 price.
2. Submit form.

**Expected Result:**
- Validation error displayed

---

### Testcase_ID: EVENT_CITY_VENUE_VALIDATION_012

**Test Scenario:** Verify city and venue validation.

**Test Steps:**
1. Enter invalid city value.
2. Enter invalid venue value.

**Expected Result:**
- Validation error displayed

---

### Testcase_ID: EVENT_SUCCESSFUL_CREATION_013

**Test Scenario:** Verify successful event creation.

**Test Steps:**
1. Enter valid event data.
2. Submit form.

**Expected Result:**
- Success notification displayed

---

## Scenario 4: New User Creation

### Testcase_ID: USER_REGISTRATION_PAGE_ACCESS_001

**Test Scenario:** Verify registration page access.

**Test Steps:**
1. Click Register link.

**Expected Result:**
- Registration form displayed

---

### Testcase_ID: USER_DUPLICATE_EMAIL_VALIDATION_002

**Test Scenario:** Verify duplicate email validation.

**Test Steps:**
1. Register using existing email.

**Expected Result:**
- Email already registered error

---

### Testcase_ID: USER_PASSWORD_POLICY_VALIDATION_003

**Test Scenario:** Verify password policy.

**Test Steps:**
1. Enter invalid password format (such as all consecutive numbers).

**Expected Result:**
- Validation error displayed

---

### Testcase_ID: USER_NEW_ACCOUNT_REGISTRATION_004

**Test Scenario:** Verify registration with new email.

**Test Steps:**
1. Enter valid new user data.

**Expected Result:**
- Account created successfully

---

### Testcase_ID: USER_CONFIRM_PASSWORD_REQUIRED_005

**Test Scenario:** Verify confirm password requirement.

**Test Steps:**
1. Leave confirm password blank.

**Expected Result:**
- Validation error displayed

---

### Testcase_ID: USER_REGISTRATION_SUCCESS_MESSAGE_006

**Test Scenario:** Verify registration success message.

**Test Steps:**
1. Complete registration.

**Expected Result:**
- Success message displayed

---

### Testcase_ID: USER_DASHBOARD_ACCESS_AFTER_REGISTRATION_007

**Test Scenario:** Verify dashboard access after registration.

**Test Steps:**
1. Register successfully.

**Expected Result:**
- User redirected to dashboard

---

## Scenario 5: Verify Event Appears in List

### Testcase_ID: EVENT_LIST_NEW_EVENT_VISIBLE_001

**Test Scenario:** Verify newly created event in All Events table.

**Test Steps:**
1. Create event.
2. Open All Events table.

**Expected Result:**
- Event appears in list

---

### Testcase_ID: EVENT_LIST_DATA_ACCURACY_002

**Test Scenario:** Verify event data accuracy in the table.

**Test Steps:**
1. Compare created event data with table values.

**Expected Result:**
- Displayed data matches created data

---

# SECTION 2: AI-CREATED TEST CASES

## AI Prompt Given

**Context:** Act as a senior test engineer specialized with functional testing and UI/UX testing for web applications.

**URL to Test:** https://eventhub.rahulshettyacademy.com/

**Application Context:**
- EventHub is an event booking platform with the following core functionality
- Users can register/create a profile and log in
- Logged-in users can browse listed events and book them
- A "My Bookings" section lets users view events they have booked
- An Admin section allows authorized users to create and manage new events

**Scenarios to Cover (End-to-End Flow):**
- New user registration/account creation
- Admin login and navigation to the event management section
- Admin creates a new event (with all required event details)
- Verification that the newly created event appears in that user's event listing
- Manage Event in Admin Section
- Old User Login

**Task:** Generate a complete manual test suite for the above scenarios on the Eventhub website. Do not duplicate the same test cases.

---

## New User Registration / Account Creation

### Testcase_ID: AI_REG_001

**Test Scenario:** Verify successful new user registration with valid data

**Test Steps:**
1. Navigate to EventHub website.
2. Click on Register/Sign Up.
3. Enter valid First Name, Last Name, Email, Password, and required fields.
4. Click Register/Create Account.

**Expected Result:**
- Account is created successfully
- Success message is displayed
- User is redirected to login/dashboard page

---

### Testcase_ID: AI_REG_002

**Test Scenario:** Verify mandatory field validation during registration

**Test Steps:**
1. Open Registration page.
2. Leave all mandatory fields blank.
3. Click Register.

**Expected Result:**
- Appropriate validation messages are displayed for all required fields
- Registration is not completed

---

### Testcase_ID: AI_REG_003

**Test Scenario:** Verify registration with already registered email address

**Test Steps:**
1. Open Registration page.
2. Enter an email already registered in the system.
3. Fill remaining fields with valid data.
4. Submit registration.

**Expected Result:**
- Registration is blocked
- Message indicates email already exists

---

### Testcase_ID: AI_REG_004

**Test Scenario:** Verify email format validation

**Test Steps:**
1. Open Registration page.
2. Enter invalid email format (e.g., testgmail.com).
3. Complete remaining fields.
4. Submit registration.

**Expected Result:**
- Invalid email validation message is displayed
- Registration is prevented

---

### Testcase_ID: AI_REG_005

**Test Scenario:** Verify password policy validation

**Test Steps:**
1. Open Registration page.
2. Enter password not meeting required criteria.
3. Fill remaining details.
4. Submit registration.

**Expected Result:**
- Password policy error message is displayed
- User cannot register until valid password is entered

---

### Testcase_ID: AI_REG_006

**Test Scenario:** Verify UI alignment and usability of registration page

**Test Steps:**
1. Open Registration page.
2. Inspect labels, input fields, buttons, placeholders, and page layout.

**Expected Result:**
- All UI elements are properly aligned
- Labels are readable
- No overlapping or broken components are visible

---

## Admin Login and Navigation

### Testcase_ID: AI_ADMIN_LOGIN_001

**Test Scenario:** Verify successful admin login

**Test Steps:**
1. Open Login page.
2. Enter valid admin credentials.
3. Click Login.

**Expected Result:**
- Admin is logged in successfully
- Admin dashboard is displayed

---

### Testcase_ID: AI_ADMIN_LOGIN_002

**Test Scenario:** Verify login with invalid admin credentials

**Test Steps:**
1. Open Login page.
2. Enter invalid username/password.
3. Click Login.

**Expected Result:**
- Login fails
- Appropriate error message is displayed

---

### Testcase_ID: AI_ADMIN_NAV_003

**Test Scenario:** Verify navigation to Event Management section

**Test Steps:**
1. Login as Admin.
2. Navigate through dashboard menu.
3. Select Event Management section.

**Expected Result:**
- Event Management page opens successfully
- Existing events are displayed

---

### Testcase_ID: AI_ADMIN_NAV_004

**Test Scenario:** Verify admin menu accessibility

**Test Steps:**
1. Login as Admin.
2. Verify all available menu options.

**Expected Result:**
- All admin functions are visible and accessible
- Navigation works correctly

---

## Admin Creates New Event

### Testcase_ID: AI_EVENT_CREATE_001

**Test Scenario:** Verify successful event creation with valid details

**Test Steps:**
1. Login as Admin.
2. Navigate to Event Management.
3. Click Create Event.
4. Enter all mandatory event details.
5. Save event.

**Expected Result:**
- Event is created successfully
- Success confirmation message is displayed

---

### Testcase_ID: AI_EVENT_CREATE_002

**Test Scenario:** Verify mandatory field validation during event creation

**Test Steps:**
1. Open Create Event page.
2. Leave required fields empty.
3. Click Save.

**Expected Result:**
- Validation messages appear
- Event is not created

---

### Testcase_ID: AI_EVENT_CREATE_003

**Test Scenario:** Verify event creation with past event date

**Test Steps:**
1. Create a new event.
2. Select a date in the past.
3. Save event.

**Expected Result:**
- System prevents creation
- Appropriate validation message is displayed

---

### Testcase_ID: AI_EVENT_CREATE_004

**Test Scenario:** Verify event image upload functionality

**Test Steps:**
1. Open Create Event page.
2. Upload valid image file.
3. Save event.

**Expected Result:**
- Image uploads successfully
- Event is created with image attached

---

### Testcase_ID: AI_EVENT_CREATE_005

**Test Scenario:** Verify event details are saved correctly

**Test Steps:**
1. Create event with title, description, venue, date, and capacity.
2. Save event.
3. Reopen created event.

**Expected Result:**
- All entered details are stored accurately

---

### Testcase_ID: AI_EVENT_CREATE_006

**Test Scenario:** Verify UI/UX of event creation page

**Test Steps:**
1. Open Create Event page.
2. Verify form design, field alignment, button visibility, and responsiveness.

**Expected Result:**
- Form is user-friendly
- Fields and buttons are properly aligned and accessible

---

## Verify Newly Created Event Appears in User Event Listing

### Testcase_ID: AI_EVENT_LIST_001

**Test Scenario:** Verify newly created event is visible in event listing

**Test Steps:**
1. Login as normal user.
2. Navigate to Events page.
3. Search for newly created event.

**Expected Result:**
- Newly created event appears in listing

---

### Testcase_ID: AI_EVENT_LIST_002

**Test Scenario:** Verify event details displayed correctly in listing

**Test Steps:**
1. Open event listing.
2. Locate newly created event.
3. Verify displayed information.

**Expected Result:**
- Event title, date, venue, and image match admin-created data

---

### Testcase_ID: AI_EVENT_LIST_003

**Test Scenario:** Verify event search functionality

**Test Steps:**
1. Navigate to event listing.
2. Search using event name.
3. Execute search.

**Expected Result:**
- Matching event appears in search results

---

### Testcase_ID: AI_EVENT_LIST_004

**Test Scenario:** Verify event detail page accessibility

**Test Steps:**
1. Click newly created event.
2. Open event detail page.

**Expected Result:**
- Event detail page loads successfully
- Complete event information is displayed

---

## Manage Event in Admin Section

### Testcase_ID: AI_ADMIN_MANAGE_001

**Test Scenario:** Verify admin can edit event details

**Test Steps:**
1. Login as Admin.
2. Navigate to Event Management.
3. Select created event.
4. Edit event information.
5. Save changes.

**Expected Result:**
- Event details are updated successfully

---

### Testcase_ID: AI_ADMIN_MANAGE_002

**Test Scenario:** Verify edited event information reflects in user listing

**Test Steps:**
1. Modify event details as Admin.
2. Login as User.
3. View event listing.

**Expected Result:**
- Updated event information is displayed

---

### Testcase_ID: AI_ADMIN_MANAGE_003

**Test Scenario:** Verify admin can deactivate/cancel event

**Test Steps:**
1. Login as Admin.
2. Open Event Management.
3. Select event.
4. Mark event as inactive/cancelled.

**Expected Result:**
- Event status changes successfully
- Appropriate confirmation message appears

---

### Testcase_ID: AI_ADMIN_MANAGE_004

**Test Scenario:** Verify inactive event visibility behavior

**Test Steps:**
1. Deactivate event.
2. Login as User.
3. Check event listing.

**Expected Result:**
- Event follows defined business rule (hidden or marked inactive)

---

### Testcase_ID: AI_ADMIN_MANAGE_005

**Test Scenario:** Verify event deletion functionality

**Test Steps:**
1. Login as Admin.
2. Select event.
3. Click Delete.
4. Confirm deletion.

**Expected Result:**
- Event is deleted successfully
- Event no longer appears in management list

---

### Testcase_ID: AI_ADMIN_MANAGE_006

**Test Scenario:** Verify delete confirmation popup behavior

**Test Steps:**
1. Attempt to delete event.
2. Observe confirmation popup.
3. Click Cancel.

**Expected Result:**
- Event remains unchanged
- Deletion is not executed

---

## Old User Login and Event Booking

### Testcase_ID: AI_BOOK_LOGIN_001

**Test Scenario:** Verify existing user login

**Test Steps:**
1. Open Login page.
2. Enter valid existing user credentials.
3. Click Login.

**Expected Result:**
- User logs in successfully
- User dashboard is displayed

---

### Testcase_ID: AI_BOOK_EVENT_002

**Test Scenario:** Verify booking newly created event

**Test Steps:**
1. Login as existing user.
2. Open newly created event.
3. Click Book Event.
4. Complete booking process.

**Expected Result:**
- Booking is successful
- Confirmation message is displayed

---

### Testcase_ID: AI_BOOK_VERIFY_003

**Test Scenario:** Verify booked event appears in My Bookings

**Test Steps:**
1. Complete event booking.
2. Navigate to My Bookings.

**Expected Result:**
- Newly booked event is displayed in My Bookings section

---

### Testcase_ID: AI_BOOK_DETAILS_004

**Test Scenario:** Verify booking details accuracy

**Test Steps:**
1. Open My Bookings.
2. Select booked event.

**Expected Result:**
- Event name, date, venue, and booking information are correct

---

### Testcase_ID: AI_BOOK_DUPLICATE_005

**Test Scenario:** Verify booking duplicate event behavior

**Test Steps:**
1. Book an event.
2. Attempt booking same event again.

**Expected Result:**
- System follows business rule: prevents duplicate booking OR displays duplicate booking warning

---

### Testcase_ID: AI_BOOK_UI_006

**Test Scenario:** Verify My Bookings page UI/UX

**Test Steps:**
1. Navigate to My Bookings.
2. Review page layout and booking cards.

**Expected Result:**
- Bookings are clearly displayed
- Page is responsive and easy to navigate

---

## End-to-End Validation

### Testcase_ID: AI_E2E_001

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
- Entire workflow executes successfully without functional or UI issues
- Data consistency is maintained across Admin and User modules

---

# ANALYSIS AND RECOMMENDATIONS

## What Was Effective (Compared to Industry Standards)

✅ **Strengths:**

- **Comprehensive Coverage:** Covers complete end-to-end business flow from Registration → Admin Event Creation → Event Management → User Booking → My Bookings
- **Balanced Testing:** Includes both positive and negative scenarios (valid/invalid registration, login validation, mandatory field checks)
- **Well-Structured Format:** Clear Test Case IDs, Steps, and Expected Results with consistent organization
- **Logical Separation:** Scenarios are organized by user journey stage without major duplication
- **UI/UX Inclusion:** Includes basic UI/UX validation alongside functional testing
- **User-Friendly:** Easy to understand, review, and execute for manual testers
- **Baseline Quality:** Provides solid foundation for smoke testing, UAT, and initial regression coverage

## Areas for Improvement

❌ **Gaps Identified:**

- **Missing Metadata:** Lacks preconditions, test data, priority, severity, and requirement traceability
- **Limited Edge Cases:** Boundary value testing (field lengths, capacity limits, date validations) is insufficient
- **Security Gaps:** Missing security and authorization scenarios (role access, session timeout, URL manipulation)
- **Deep Event Management:** Event management coverage lacks detail (capacity updates, booked-event deletion impacts, status transitions)
- **Search/Filter Testing:** Minimal search, filter, sorting, and booking edge-case coverage
- **Generic UI/UX:** UI/UX checks are generic rather than detailed and measurable
- **No Advanced Testing:** Missing cross-browser, responsive, accessibility, performance, and concurrency testing

---

# FINAL AUTOMATION-READY TEST SUITE

## Registration Module

### Testcase_ID: FINAL_REG_001

**Test Scenario:** Verify successful registration with valid user details

**Priority:** High | **Severity:** Critical

**Test Steps:**
1. Navigate to Registration page.
2. Enter unique email address.
3. Enter password meeting policy requirements.
4. Enter matching Confirm Password.
5. Click Create Account button.

**Expected Result:**
- User account is created successfully
- Success message is displayed
- User is redirected to Login/Home page

---

### Testcase_ID: FINAL_REG_002

**Test Scenario:** Verify mandatory field validation on registration form

**Priority:** High | **Severity:** Critical

**Test Steps:**
1. Open Registration page.
2. Leave all fields blank.
3. Click Create Account button.

**Expected Result:**
- Validation messages appear for all mandatory fields
- Registration is blocked

---

### Testcase_ID: FINAL_REG_003

**Test Scenario:** Verify registration with existing email

**Priority:** High | **Severity:** Major

**Test Steps:**
1. Open Registration page.
2. Enter an already registered email.
3. Enter valid password and confirm password.
4. Submit form.

**Expected Result:**
- Registration is rejected
- Duplicate email message is displayed

---

### Testcase_ID: FINAL_REG_004

**Test Scenario:** Verify password policy enforcement

**Priority:** High | **Severity:** Major

**Test Steps:**
1. Enter password without uppercase, special character, or required length.
2. Submit registration.

**Expected Result:**
- Password policy validation is displayed
- Account is not created

---

### Testcase_ID: FINAL_REG_005

**Test Scenario:** Verify password and confirm password mismatch validation

**Priority:** Medium | **Severity:** Major

**Test Steps:**
1. Enter valid password.
2. Enter different Confirm Password.
3. Submit registration.

**Expected Result:**
- Password mismatch error is displayed
- Registration is prevented

---

## Login Module

### Testcase_ID: FINAL_LOGIN_001

**Test Scenario:** Verify successful login for registered user

**Priority:** High | **Severity:** Critical

**Test Steps:**
1. Open Login page.
2. Enter valid email and password.
3. Click Sign In button.

**Expected Result:**
- User is successfully logged in
- Dashboard/Home page loads

---

### Testcase_ID: FINAL_LOGIN_002

**Test Scenario:** Verify login with invalid credentials

**Priority:** High | **Severity:** Major

**Test Steps:**
1. Enter invalid email/password.
2. Click Sign In button.

**Expected Result:**
- Login fails
- Error message is displayed

---

### Testcase_ID: FINAL_LOGIN_003

**Test Scenario:** Verify logout functionality

**Priority:** High | **Severity:** Major

**Test Steps:**
1. Login successfully.
2. Click Logout button.
3. Try navigating back using browser Back button.

**Expected Result:**
- User remains logged out
- Protected pages are inaccessible

---

## Admin Event Management

### Testcase_ID: FINAL_ADMIN_001

**Test Scenario:** Verify admin can access Event Management module

**Priority:** High | **Severity:** Critical

**Test Steps:**
1. Login as Admin.
2. Navigate to Event Management.

**Expected Result:**
- Event Management page loads successfully

---

### Testcase_ID: FINAL_ADMIN_002

**Test Scenario:** Verify event creation using valid data

**Priority:** High | **Severity:** Critical

**Test Steps:**
1. Open Create Event page.
2. Enter event title.
3. Enter description.
4. Select future date.
5. Enter venue.
6. Enter capacity.
7. Save event.

**Expected Result:**
- Event is created successfully
- Event appears in Event Management list

---

### Testcase_ID: FINAL_ADMIN_003

**Test Scenario:** Verify mandatory field validation during event creation

**Priority:** High | **Severity:** Major

**Test Steps:**
1. Open Create Event page.
2. Leave required fields blank.
3. Save event.

**Expected Result:**
- Validation messages are displayed
- Event creation is blocked

---

### Testcase_ID: FINAL_ADMIN_004

**Test Scenario:** Verify event creation with past date

**Priority:** Medium | **Severity:** Major

**Test Steps:**
1. Create event using a past date.
2. Save event.

**Expected Result:**
- Event is not created
- Date validation message is displayed

---

### Testcase_ID: FINAL_ADMIN_005

**Test Scenario:** Verify admin can update existing event

**Priority:** High | **Severity:** Major

**Test Steps:**
1. Open existing event.
2. Modify title, venue, or date.
3. Save changes.

**Expected Result:**
- Event updates successfully
- Modified details are persisted

---

### Testcase_ID: FINAL_ADMIN_006

**Test Scenario:** Verify admin can delete event

**Priority:** High | **Severity:** Major

**Test Steps:**
1. Open Event Management.
2. Select event.
3. Click Delete button.
4. Confirm deletion.

**Expected Result:**
- Event is removed from event list

---

### Testcase_ID: FINAL_ADMIN_007

**Test Scenario:** Verify delete confirmation behavior

**Priority:** Medium | **Severity:** Minor

**Test Steps:**
1. Click Delete Event button.
2. Click Cancel on confirmation dialog.

**Expected Result:**
- Event remains unchanged
- No deletion occurs

---

## Event Listing

### Testcase_ID: FINAL_EVENT_001

**Test Scenario:** Verify newly created event appears in event listing

**Priority:** High | **Severity:** Critical

**Test Steps:**
1. Create event as Admin.
2. Login as User.
3. Navigate to Events page.

**Expected Result:**
- Newly created event is visible

---

### Testcase_ID: FINAL_EVENT_002

**Test Scenario:** Verify event information displayed correctly

**Priority:** High | **Severity:** Major

**Test Steps:**
1. Open event card.
2. Compare displayed details with admin-created data.

**Expected Result:**
- Event title, venue, date, and description match stored data

---

### Testcase_ID: FINAL_EVENT_003

**Test Scenario:** Verify search functionality

**Priority:** High | **Severity:** Major

**Test Steps:**
1. Enter event name in search field.
2. Execute search.

**Expected Result:**
- Matching event is returned

---

### Testcase_ID: FINAL_EVENT_004

**Test Scenario:** Verify search behavior for invalid event name

**Priority:** Medium | **Severity:** Minor

**Test Steps:**
1. Search using non-existing event name.

**Expected Result:**
- No results message is displayed

---

## Booking Module

### Testcase_ID: FINAL_BOOK_001

**Test Scenario:** Verify successful event booking

**Priority:** High | **Severity:** Critical

**Test Steps:**
1. Login as User.
2. Open available event.
3. Click Book Event button.
4. Confirm booking.

**Expected Result:**
- Booking is successful
- Confirmation message appears

---

### Testcase_ID: FINAL_BOOK_002

**Test Scenario:** Verify booked event appears in My Bookings

**Priority:** High | **Severity:** Critical

**Test Steps:**
1. Book an event.
2. Open My Bookings section.

**Expected Result:**
- Booked event is listed

---

### Testcase_ID: FINAL_BOOK_003

**Test Scenario:** Verify booking information accuracy

**Priority:** High | **Severity:** Major

**Test Steps:**
1. Open My Bookings.
2. Open booked event.

**Expected Result:**
- Event name, venue, date, and booking status are correct

---

### Testcase_ID: FINAL_BOOK_004

**Test Scenario:** Verify duplicate booking handling

**Priority:** Medium | **Severity:** Major

**Test Steps:**
1. Book an event.
2. Attempt booking same event again.

**Expected Result:**
- Duplicate booking is prevented or warning message is displayed

---

### Testcase_ID: FINAL_BOOK_005

**Test Scenario:** Verify booking restriction for expired events

**Priority:** Medium | **Severity:** Major

**Test Steps:**
1. Open expired event.
2. Attempt booking.

**Expected Result:**
- Booking is blocked

---

## Authorization & Security

### Testcase_ID: FINAL_SEC_001

**Test Scenario:** Verify normal user cannot access admin pages

**Priority:** High | **Severity:** Critical

**Test Steps:**
1. Login as normal user.
2. Enter Admin URL directly.

**Expected Result:**
- Access denied or redirected

---

### Testcase_ID: FINAL_SEC_002

**Test Scenario:** Verify protected pages require authentication

**Priority:** High | **Severity:** Critical

**Test Steps:**
1. Do not login.
2. Open My Bookings URL.
3. Open Admin URL.

**Expected Result:**
- User is redirected to Login page

---

## UI/UX Validation

### Testcase_ID: FINAL_UI_001

**Test Scenario:** Verify registration page UI consistency

**Priority:** Medium | **Severity:** Minor

**Test Steps:**
1. Open Registration page.
2. Verify labels, input fields, buttons, and alignment.

**Expected Result:**
- UI elements are properly aligned and usable

---

### Testcase_ID: FINAL_UI_002

**Test Scenario:** Verify event listing responsiveness

**Priority:** Medium | **Severity:** Minor

**Test Steps:**
1. Open Events page.
2. Test on Desktop, Tablet, and Mobile viewport.

**Expected Result:**
- Layout adjusts correctly without overlap or truncation

---

### Testcase_ID: FINAL_UI_003

**Test Scenario:** Verify validation messages are user-friendly

**Priority:** Medium | **Severity:** Minor

**Test Steps:**
1. Trigger validation errors on Registration/Login/Event forms.

**Expected Result:**
- Error messages are clearly visible and understandable

---

## End-to-End Workflow

### Testcase_ID: FINAL_E2E_001

**Test Scenario:** Verify complete EventHub business workflow

**Priority:** High | **Severity:** Critical

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
- Entire workflow executes successfully with consistent data across all modules

---

## Document Summary

- **Total Test Cases (Section 1):** 37 test cases
- **Total Test Cases (Section 2):** 34 test cases
- **Total Test Cases (Final Suite):** 43 test cases
- **Coverage Areas:** Registration, Login, Event Management, Booking, Security, UI/UX
- **Last Updated:** 2026-06-20
- **Format:** Markdown (GitHub-compatible)
