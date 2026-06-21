# QA MANUAL TEST CASES
## Member : Alekhya Roy
## Target Application : https://eventhub.rahulshettyacademy.com/login
 
## SECTION 1 : HUMAN THINKING TEST CASES
 
### TC_001 : New user creation with valid data
 
**Test Steps:**
-Open https://eventhub.rahulshettyacademy.com/login website on a browser
-Click on register link under Sign in option
-Enter valid email address
-Enter valid password which is matching the password rule
-Enter same password in confirm password section
-Click on create account
**Expected Result : Account should be created and redirected to dashboard page**
### TC_002 : New user creation with invalid email format
**Test Steps:**
-Open https://eventhub.rahulshettyacademy.com/login website on a browser
-Click on register link under Sign in option
-Enter invalid email format
-Enter valid password which is matching the password rule
-Enter same password in confirm password section
-Click on create account
**Expected Result : Account should not be created and validation error should appear**
### TC_003 : Verify that user creation fails when the entered password does not comply with the required password format
**Test Steps:**
-Open https://eventhub.rahulshettyacademy.com/login website on a browser
-Click on register link under Sign in option
-Enter valid email address
-Enter a password that does not match the required format
-Enter same password in confirm password section
-Click on create account
**Expected Result : “Password does not meet the requirements below” error should be displayed**
### TC_004 : Verify that user creation fails when the Confirm Password field does not match the Password field
**Test Steps:**
-Open https://eventhub.rahulshettyacademy.com/login website on a browser
-Click on register link under Sign in option
-Enter valid email address
-Enter valid password which is matching the password rule
-Enter different password in confirm password section
-Click on create account
**Expected Result : “Password does not match “ error message should appear**
### TC_005 : Verify that user creation fails when mandatory fields are left blank
**Test Steps:**
-Open https://eventhub.rahulshettyacademy.com/login website on a browser
-Click on register link under Sign in option
-Leave all mandatory fields blank
**Expected Result : Mandatory fields should not be blanked message should appear**
### TC_006 : Verify that copy-paste functionality is disabled for the Password and Confirm Password fields
**Test Steps:**
-Open https://eventhub.rahulshettyacademy.com/login website on a browser
-Click on register link under Sign in option
-Enter valid email address
-Enter valid password which is matching the password rule
-Attempt to copy the entered password
-Try to paste it into the Confirm Password field
**Expected Result : Copy and paste actions should be blocked for both Password and Confirm Password fields**
### TC_OO7 : Verify user registration with already registered email address
**Test Steps:**
-Open https://eventhub.rahulshettyacademy.com/login website on a browser
-Click on register link under Sign in option
-Enter already registered email address
-Enter valid password which is matching the password rule
-Enter same password in confirm password section
-Click on create account
**Expected Result : Email address already registered message should appear**
### TC_008 : Verify that after successful user registration, the system redirects to the dashboard and the Admin section is visible.
**Test Steps:**
-Open https://eventhub.rahulshettyacademy.com/login website on a browser
-Click on register link under Sign in option
-Enter valid email address
-Enter valid password which is matching the password rule
-Enter same password in confirm password section
-Click on create account
-After redirection to dashboard observe admin section is visible or not
**Expected Result : Admin drop down should be visible with “Manage Events “ and “Manage Bookings “ options.**
### TC_009 : Verify that “Manage Events “ are clickable and redirected to new event form
**Test Steps:**
-Click on Admin drop down in navigation bar
-Click on Manage Event option
**Expected Result : New event creation page should appear**
### TC_010 : Verify that after filling up all required fields in new event form and submit new event entry is creating and showing in events list
**Test Steps:**
-Fill in all required fields in the New Event form
-Click on the Submit button.
**Expected Result : A new event entry should be created successfully.The newly created event should appear in the Events List with the correct details.**
### TC_011 : Verify that newly created event is visible in the event list of another user
**Test Steps:**
-Log in as User B.
-Navigate to the Events List page.
-Search or scroll through the list to locate the event created by User A.
-Expected Results :The newly created event by User A should be visible in the Events List of User B.
## SECTION 2 : AI CREATED MANUAL TEST CASES
 
### Prompt :
ROLE
Act as a Senior Test Engineer with 5+ years of experience specializing in
manual testing, functional testing, regression testing, and UI/UX testing
for web applications.
 
APPLICATION CONTEXT
Application Under Test: EventHub
URL: https://eventhub.rahulshettyacademy.com/
 
EventHub is an event booking platform with the following core functionality:
- Users can register/create a profile and log in.
- Logged-in users can browse listed events and book them.
- A "My Bookings" section lets users view events they have booked.
- An Admin section allows authorized users to create and manage new events.
 
SCENARIO TO BE COVERED (END-TO-END FLOW)
Write test cases covering this user journey, broken down into its
individual stages:
1. New user registration/account creation.
2. Admin login and navigation to the event management section.
3. Admin creates a new event (with all required event details).
4. A different (non-admin) user logs in.
5. Verification that the newly created event appears in that user's
   event listing.
 
TASK
Generate a complete manual test suite for the above scenario, organized
by the following categories. Do not duplicate the same test case across
categories — each test case should appear exactly once, under its most
relevant category.
 
1. Positive Test Cases – valid flows for registration, login, event
   creation, and event visibility.
2. Negative Test Cases – invalid inputs, broken flows, error handling.
3. Input Field Validation Test Cases – field-level checks (mandatory
   fields, character limits, allowed formats, date/time pickers,
   numeric fields, special characters, boundary values, etc.) for all
   forms involved (registration, login, event creation).
4. Security Validation Test Cases – e.g., SQL injection/XSS attempts in
   input fields, access control (non-admin trying to access admin URLs
   directly), session handling, password masking, unauthorized API/URL
   access.
5. UI/UX Test Cases – layout consistency, responsiveness, button states,
   navigation, error message clarity, accessibility basics.
6. Business Validation Test Cases – rules specific to the domain, e.g.,
   "an event created by admin should be immediately visible to all
   users," "a user cannot book an event with 0 available seats,"
   "duplicate event names handling," etc.
 
TEST CASE FORMAT
Write each test case strictly in the following format:
 
### TC_001 : <Short descriptive title of the test case>
**Test Steps:**
Step 1 : <action>
Step 2 : <action>
Step 3 : <action>
**Expected Result : <expected outcome after executing the steps>**
 
Continue numbering sequentially (TC_002, TC_003, ...) across the entire
suite, grouped under their respective category headings (Positive,
Negative, Input Field Validation, Security, UI/UX, Business Validation).
 
AUTOMATION COMPATIBILITY
Write each test case so that it can be directly adapted for automation
using a Non-BDD approach only (e.g., Selenium/Cypress/Playwright). Steps
must be atomic and expected results must be explicit enough for direct
conversion into automation scripts.
 
IMPORTANT — DO NOT include any Gherkin/BDD-style (Given/When/Then)
scenarios anywhere in the output. Only the TC_xxx format defined above
should be used. This output is intended strictly for the non-BDD
automation approach.
 
OUTPUT FORMAT
Present test cases grouped by category (Positive → Negative → Input
Field Validation → Security → UI/UX → Business Validation), using only
the TC_xxx format. If the full suite is large, deliver it in logical
batches by category rather than truncating.
 
# EventHub — Manual Test Suite
**End-to-End Flow:** New User Registration → Admin Login → Admin Creates Event → Different User Logs In → Event Visible in User's Listing
 
**Application Under Test:** EventHub (https://eventhub.rahulshettyacademy.com/)
**Prepared by:** Senior Test Engineer
**Format:** Each test case (TC_xxx) lists atomic Test Steps and an explicit Expected Result, written for direct adaptation into Selenium/Cypress/Playwright automation scripts.
 
---
 
## 1. Positive Test Cases
 
### TC_001 : Successful new user registration with valid details
**Test Steps :**
Step 1 : Navigate to the EventHub registration/sign-up page.
Step 2 : Enter a valid, unused name, email address, and a password meeting complexity rules in the respective fields.
Step 3 : Re-enter the same password in the Confirm Password field (if present) and click the "Register"/"Sign Up" button.
**Expected Result :** The account is created successfully; the user is shown a success message/confirmation and is either logged in automatically or redirected to the login page.
 
### TC_002 : Successful login of newly registered user
**Test Steps :**
Step 1 : Navigate to the EventHub login page.
Step 2 : Enter the email and password used during TC_001 registration.
Step 3 : Click the "Login"/"Sign In" button.
**Expected Result :** The user is authenticated and redirected to the home/dashboard/event listing page, with their session reflecting a logged-in state (e.g., username/profile icon visible).
 
### TC_003 : Successful admin login
**Test Steps :**
Step 1 : Navigate to the EventHub login page.
Step 2 : Enter valid admin credentials (email and password).
Step 3 : Click the "Login" button.
**Expected Result :** Admin is authenticated successfully and redirected to the admin-accessible home/dashboard, with admin-specific navigation options (e.g., "Manage Events", "Admin") visible.
 
### TC_004 : Successful navigation from admin login to event management section
**Test Steps :**
Step 1 : Log in as admin.
Step 2 : Locate and click the "Admin"/"Manage Events"/"Create Event" navigation link or menu item.
Step 3 : Observe the page that loads.
**Expected Result :** Admin is navigated to the Event Management section without errors, and the page displays options to create/view/edit events.
 
### TC_005 : Successful creation of new event by admin with all required fields
**Test Steps :**
Step 1 : Log in as admin and navigate to the "Create Event" section.
Step 2 : Fill in all required fields (Event Name, Description, Date, Time, Venue/Location, Available Seats, Price, and Banner Image if applicable) with valid values.
Step 3 : Click the "Create"/"Submit"/"Save Event" button.
**Expected Result :** The event is created successfully; a confirmation message is displayed, and the event is added to the system's event list (visible in admin's event management view).
 
### TC_006 : Successful logout of admin user
**Test Steps :**
Step 1 : While logged in as admin, locate the "Logout"/"Sign Out" option (typically in profile menu).
Step 2 : Click "Logout".
Step 3 : Observe the resulting page/state.
**Expected Result :** Admin session is terminated; user is redirected to the login page or public home page, and admin-only navigation options are no longer visible.
 
### TC_007 : Successful login of a different (non-admin) registered user
**Test Steps :**
Step 1 : Navigate to the login page (after admin has logged out).
Step 2 : Enter the credentials of a second, previously registered non-admin user (different from admin and from TC_001's account, or the TC_001 account itself).
Step 3 : Click "Login".
**Expected Result :** The non-admin user is logged in successfully and redirected to the standard user home/event listing page (without admin navigation options).
 
### TC_008 : Newly created event visible in non-admin user's event listing
**Test Steps :**
Step 1 : Log in as the non-admin user (TC_007).
Step 2 : Navigate to the main events/listing page.
Step 3 : Search/scroll for the event created in TC_005 by its event name.
**Expected Result :** The event created by admin in TC_005 is visible in the listing with correct name, date, and other summary details, confirming end-to-end visibility of admin-created content to regular users.
 
### TC_009 : Non-admin user can view full details of the newly created event
**Test Steps :**
Step 1 : From the event listing page, click on the event created in TC_005.
Step 2 : Observe the event details page that opens.
Step 3 : Compare displayed fields (description, date, time, venue, price, seats) against the values entered by admin.
**Expected Result :** The event detail page opens and displays all the information accurately as entered by the admin, with no missing or corrupted fields.
 
### TC_010 : Non-admin user can successfully book the newly created event
**Test Steps :**
Step 1 : Open the detail page of the event created in TC_005 as the non-admin user.
Step 2 : Click the "Book"/"Register for Event" button.
Step 3 : Confirm the booking if a confirmation step/dialog is presented.
**Expected Result :** The booking is completed successfully; a confirmation message is shown, and the available seat count for the event decreases by one.
 
### TC_011 : Booked event appears under "My Bookings" section
**Test Steps :**
Step 1 : After completing the booking in TC_010, navigate to the "My Bookings" section.
Step 2 : Locate the event booked in TC_010 in the list.
Step 3 : Verify the displayed booking details (event name, date, status).
**Expected Result :** The booked event appears correctly under "My Bookings" with accurate event details and a confirmed booking status.
 
---
 
## 2. Negative Test Cases
 
### TC_012 : Registration fails with already registered email
**Test Steps :**
Step 1 : Navigate to the registration page.
Step 2 : Enter a name, an email address that is already registered (e.g., from TC_001), and a valid password.
Step 3 : Submit the registration form.
**Expected Result :** Registration is rejected with a clear error message (e.g., "Email already in use/registered"), and no duplicate account is created.
 
### TC_013 : Login fails with incorrect password for valid email
**Test Steps :**
Step 1 : Navigate to the login page.
Step 2 : Enter a valid, registered email address.
Step 3 : Enter an incorrect password and click "Login".
**Expected Result :** Login is rejected with a generic error message (e.g., "Invalid email or password"), without revealing whether the email or password specifically was wrong, and the user remains on the login page.
 
### TC_014 : Login fails with unregistered email address
**Test Steps :**
Step 1 : Navigate to the login page.
Step 2 : Enter an email address that has never been registered.
Step 3 : Enter any password and click "Login".
**Expected Result :** Login is rejected with an appropriate error message, and the user remains on the login page.
 
### TC_015 : Admin event creation fails when mandatory fields are left blank
**Test Steps :**
Step 1 : Log in as admin and navigate to "Create Event".
Step 2 : Leave one or more mandatory fields (e.g., Event Name, Date) empty.
Step 3 : Click "Submit"/"Create Event".
**Expected Result :** Form submission is blocked; validation error(s) are shown next to the blank mandatory field(s), and no event is created.
 
### TC_016 : Event creation fails when event end date/time is before start date/time
**Test Steps :**
Step 1 : Log in as admin and navigate to "Create Event".
Step 2 : Fill all fields, setting the end date/time earlier than the start date/time.
Step 3 : Submit the form.
**Expected Result :** Form submission is rejected with a validation message indicating the end date/time must be after the start date/time; the event is not created.
 
### TC_017 : Non-admin user denied access when trying to create an event via UI
**Test Steps :**
Step 1 : Log in as a non-admin user.
Step 2 : Look for any "Create Event"/"Manage Events" option in the navigation/UI.
Step 3 : If no such option is visible, confirm absence; if a workaround link is found, attempt to use it.
**Expected Result :** No event-creation/management UI option is exposed to non-admin users; any attempt to reach such functionality is blocked or redirected with an "unauthorized" message.
 
### TC_018 : Booking fails when event has zero available seats
**Test Steps :**
Step 1 : Identify or create (as admin) an event with 0 available seats remaining.
Step 2 : Log in as a non-admin user and open that event's detail page.
Step 3 : Attempt to click the "Book"/"Register" button.
**Expected Result :** The booking action is disabled or rejected; the UI clearly indicates the event is "Sold Out"/"Fully Booked", and no booking is created.
 
### TC_019 : Registration fails when password and confirm password do not match
**Test Steps :**
Step 1 : Navigate to the registration page.
Step 2 : Fill in valid name and email, enter a valid password, and enter a different value in "Confirm Password".
Step 3 : Submit the form.
**Expected Result :** Registration is blocked with a validation message indicating the passwords do not match; no account is created.
 
### TC_020 : Login attempt with valid email but blank password
**Test Steps :**
Step 1 : Navigate to the login page.
Step 2 : Enter a valid, registered email address.
Step 3 : Leave the password field blank and click "Login".
**Expected Result :** Login is blocked; a validation error indicates the password field is required, and no authentication request is sent (or the server rejects it with an appropriate message).
 
### TC_021 : Event creation fails when uploading unsupported file type for event banner
**Test Steps :**
Step 1 : Log in as admin and navigate to "Create Event".
Step 2 : Fill all mandatory fields and attempt to upload a non-image file (e.g., .pdf or .exe) as the event banner/image.
Step 3 : Submit the form.
**Expected Result :** The upload is rejected with a clear error message stating the allowed file formats (e.g., JPG, PNG); the event is not created until a valid file is provided or the field is corrected.
 
### TC_022 : Application handles network/server error gracefully during event creation submission
**Test Steps :**
Step 1 : Log in as admin and fill out a valid event creation form.
Step 2 : Simulate a network failure or server error during submission (e.g., via dev tools throttling/offline mode or backend downtime).
Step 3 : Observe the application's response.
**Expected Result :** The application displays a user-friendly error message (e.g., "Something went wrong, please try again") without crashing, losing all entered data, or creating a partial/corrupt event record.
 
---
 
## 3. Input Field Validation Test Cases
 
### TC_023 : Registration form rejects submission with empty mandatory Name field
**Test Steps :**
Step 1 : Navigate to the registration page.
Step 2 : Leave the Name field empty and fill all other fields with valid values.
Step 3 : Click "Register".
**Expected Result :** Form submission is blocked; an inline validation message indicates the Name field is required.
 
### TC_024 : Registration form validates email field format (missing @, domain)
**Test Steps :**
Step 1 : Navigate to the registration page.
Step 2 : Enter an improperly formatted email (e.g., "testuser.com" or "test@@mail" or "test@mail").
Step 3 : Fill remaining fields validly and click "Register".
**Expected Result :** Form submission is blocked; a validation message indicates the email format is invalid.
 
### TC_025 : Registration form enforces minimum password length
**Test Steps :**
Step 1 : Navigate to the registration page.
Step 2 : Enter a password shorter than the minimum required length (e.g., 3 characters) in the Password field.
Step 3 : Fill remaining fields validly and click "Register".
**Expected Result :** Form submission is blocked; a validation message specifies the minimum required password length.
 
### TC_026 : Registration form enforces maximum character limit on Name field
**Test Steps :**
Step 1 : Navigate to the registration page.
Step 2 : Enter a Name value exceeding the field's maximum allowed character count (e.g., 300 characters).
Step 3 : Fill remaining fields validly and click "Register".
**Expected Result :** The field either truncates input at the maximum limit or displays a validation error preventing submission beyond the allowed length.
 
### TC_027 : Registration form rejects special characters not allowed in Name field
**Test Steps :**
Step 1 : Navigate to the registration page.
Step 2 : Enter a Name containing disallowed special characters (e.g., "John@@123!!").
Step 3 : Fill remaining fields validly and click "Register".
**Expected Result :** Form submission is blocked (if such restriction exists) with a validation message; otherwise, the system should at minimum sanitize the input before storing/displaying it.
 
### TC_028 : Login form rejects empty email field on submit
**Test Steps :**
Step 1 : Navigate to the login page.
Step 2 : Leave the email field empty, enter any password.
Step 3 : Click "Login".
**Expected Result :** Submission is blocked; a required-field validation message is displayed for the email field.
 
### TC_029 : Login form rejects empty password field on submit
**Test Steps :**
Step 1 : Navigate to the login page.
Step 2 : Enter a valid email, leave the password field empty.
Step 3 : Click "Login".
**Expected Result :** Submission is blocked; a required-field validation message is displayed for the password field.
 
### TC_030 : Event creation form rejects empty Event Name field
**Test Steps :**
Step 1 : Log in as admin and navigate to "Create Event".
Step 2 : Leave the Event Name field empty and fill all other fields validly.
Step 3 : Click "Submit".
**Expected Result :** Submission is blocked with a required-field validation message for Event Name.
 
### TC_031 : Event creation form enforces maximum character limit on Event Name
**Test Steps :**
Step 1 : Log in as admin and navigate to "Create Event".
Step 2 : Enter an Event Name exceeding the maximum allowed character count.
Step 3 : Fill remaining fields validly and submit.
**Expected Result :** The field truncates the input or displays a validation error preventing submission beyond the allowed length.
 
### TC_032 : Event creation form's date picker disallows past dates for new event
**Test Steps :**
Step 1 : Log in as admin and navigate to "Create Event".
Step 2 : Open the date picker for the event date and attempt to select/enter a date earlier than the current date.
Step 3 : Attempt to submit the form.
**Expected Result :** Past dates are either disabled in the date picker UI or, if entered manually, rejected with a validation message; the event is not created with a past date.
 
### TC_033 : Event creation form's time picker accepts valid time format only
**Test Steps :**
Step 1 : Log in as admin and navigate to "Create Event".
Step 2 : Enter an invalid time value in the time field (e.g., "25:99" or free text "abc").
Step 3 : Attempt to submit the form.
**Expected Result :** Submission is blocked, and a validation message indicates the time format/value is invalid.
 
### TC_034 : Event creation form validates numeric-only input for "Available Seats" field
**Test Steps :**
Step 1 : Log in as admin and navigate to "Create Event".
Step 2 : Enter alphabetic or special characters (e.g., "abc" or "##") in the "Available Seats" field.
Step 3 : Attempt to submit the form.
**Expected Result :** The field rejects non-numeric input either at keystroke level or on submission, with a clear validation message.
 
### TC_035 : Event creation form rejects negative values in "Available Seats" field
**Test Steps :**
Step 1 : Log in as admin and navigate to "Create Event".
Step 2 : Enter a negative number (e.g., "-5") in the "Available Seats" field.
Step 3 : Fill remaining fields validly and submit.
**Expected Result :** Submission is blocked with a validation message stating seats must be a positive number.
 
### TC_036 : Event creation form enforces boundary value of zero seats with appropriate handling
**Test Steps :**
Step 1 : Log in as admin and navigate to "Create Event".
Step 2 : Enter "0" in the "Available Seats" field, fill remaining fields validly.
Step 3 : Submit the form.
**Expected Result :** The system either blocks creation of an event with 0 seats (validation message) or, if allowed by design, creates the event but immediately marks it as "Sold Out" in the listing — behavior should be consistent with documented business rules.
 
### TC_037 : Event creation form enforces maximum character limit on Event Description field
**Test Steps :**
Step 1 : Log in as admin and navigate to "Create Event".
Step 2 : Enter a Description value exceeding the maximum allowed character count.
Step 3 : Fill remaining fields validly and submit.
**Expected Result :** The field truncates the text or displays a validation/character-counter message preventing submission beyond the allowed length.
 
### TC_038 : Event creation form validates Venue/Location field as mandatory
**Test Steps :**
Step 1 : Log in as admin and navigate to "Create Event".
Step 2 : Leave the Venue/Location field empty and fill all other fields validly.
Step 3 : Submit the form.
**Expected Result :** Submission is blocked with a required-field validation message for Venue/Location.
 
### TC_039 : Event creation form validates Price field accepts only valid numeric/decimal format
**Test Steps :**
Step 1 : Log in as admin and navigate to "Create Event".
Step 2 : Enter an invalid value in the Price field (e.g., "free", "10.99.99", or "-20").
Step 3 : Fill remaining fields validly and submit.
**Expected Result :** Submission is blocked with a validation message indicating the price must be a valid non-negative numeric/decimal value.
 
---
 
## 4. Security Validation Test Cases
 
### TC_040 : SQL injection attempt in login email field is safely handled
**Test Steps :**
Step 1 : Navigate to the login page.
Step 2 : Enter a SQL injection payload (e.g., `' OR '1'='1`) in the email field, with any value in the password field.
Step 3 : Click "Login".
**Expected Result :** The login is rejected as invalid credentials; no unauthorized access is granted, no database error is exposed, and the payload is treated as plain text/rejected by input validation.
 
### TC_041 : SQL injection attempt in login password field is safely handled
**Test Steps :**
Step 1 : Navigate to the login page.
Step 2 : Enter a valid registered email and a SQL injection payload (e.g., `' OR 1=1 --`) in the password field.
Step 3 : Click "Login".
**Expected Result :** The login is rejected as invalid credentials; the application does not expose database errors or grant unauthorized access.
 
### TC_042 : XSS script injection in registration Name field is sanitized
**Test Steps :**
Step 1 : Navigate to the registration page.
Step 2 : Enter a script payload (e.g., `<script>alert('XSS')</script>`) in the Name field.
Step 3 : Fill remaining fields validly and submit; then view the Name as displayed elsewhere in the UI (e.g., profile, "Booked by" list).
**Expected Result :** The script does not execute; the input is either rejected, escaped, or sanitized and rendered as harmless plain text wherever displayed.
 
### TC_043 : XSS script injection in event Description field is sanitized
**Test Steps :**
Step 1 : Log in as admin and navigate to "Create Event".
Step 2 : Enter a script payload (e.g., `<img src=x onerror=alert('XSS')>`) in the Description field.
Step 3 : Submit the form and then view the event detail page as a user.
**Expected Result :** The script does not execute on the event detail page; the description is rendered as sanitized/escaped plain text.
 
### TC_044 : Non-admin user is denied direct URL access to admin event management page
**Test Steps :**
Step 1 : Log in as a non-admin user.
Step 2 : Directly enter the known/guessed admin event-management URL (e.g., `/admin/events/create`) into the browser address bar.
Step 3 : Press Enter to navigate.
**Expected Result :** Access is denied; the user is redirected to an "unauthorized"/403 page or back to the home page, and the admin functionality is not rendered.
 
### TC_045 : Unauthenticated user is denied direct URL access to "My Bookings" page
**Test Steps :**
Step 1 : Ensure no user is logged in (logged-out/incognito session).
Step 2 : Directly enter the "My Bookings" page URL into the browser address bar.
Step 3 : Press Enter to navigate.
**Expected Result :** Access is denied; the user is redirected to the login page rather than seeing any booking data.
 
### TC_046 : Password field masks characters during registration and login
**Test Steps :**
Step 1 : Navigate to the registration page and type a password into the Password field.
Step 2 : Observe the on-screen rendering of the typed characters.
Step 3 : Repeat steps 1-2 on the login page's password field.
**Expected Result :** In both forms, password characters are masked (shown as dots/asterisks) by default, with no plain-text exposure unless a "show password" toggle is explicitly used.
 
### TC_047 : Session expires/logs out user after prolonged inactivity
**Test Steps :**
Step 1 : Log in as a user.
Step 2 : Leave the session idle for the duration of the application's defined session timeout.
Step 3 : Attempt to perform an authenticated action (e.g., navigate to "My Bookings").
**Expected Result :** The session has expired; the user is redirected to the login page and must re-authenticate to access protected content.
 
### TC_048 : Logged-out user cannot access protected pages via browser back button
**Test Steps :**
Step 1 : Log in as a user and navigate to a protected page (e.g., "My Bookings").
Step 2 : Log out of the application.
Step 3 : Click the browser's "Back" button to return to the previously visited protected page.
**Expected Result :** The cached protected page is not accessible/usable; the application either redirects to login or revalidates the session, blocking access to the protected data.
 
### TC_049 : Direct API endpoint access for admin event-creation is blocked for non-admin tokens
**Test Steps :**
Step 1 : Log in as a non-admin user and capture their auth token/session (via browser dev tools/network tab).
Step 2 : Use the captured token to send a direct API request (e.g., via Postman or browser console) to the admin event-creation endpoint.
Step 3 : Observe the API response.
**Expected Result :** The API returns a 401/403 (Unauthorized/Forbidden) response; no event is created via the unauthorized request.
 
### TC_050 : Modifying event ID in URL does not expose unauthorized event data
**Test Steps :**
Step 1 : Log in as a non-admin user and open a valid event's detail page, noting its URL/ID.
Step 2 : Manually modify the event ID in the URL to a non-existent or another user's restricted resource ID.
Step 3 : Navigate to the modified URL.
**Expected Result :** The application returns a "Not Found"/appropriate error page for invalid IDs, or displays only data the user is authorized to view; no internal server errors or unintended data are exposed.
 
### TC_051 : Repeated failed login attempts trigger rate-limiting/account protection
**Test Steps :**
Step 1 : Navigate to the login page.
Step 2 : Enter a valid email with an incorrect password, repeatedly (e.g., 5-10 times in quick succession).
Step 3 : Observe the application's behavior after the threshold of failed attempts.
**Expected Result :** After a defined number of failed attempts, the application implements a protective measure (e.g., CAPTCHA, temporary lockout, or delay) to mitigate brute-force attacks, with a clear message to the user.
 
---
 
## 5. UI/UX Test Cases
 
### TC_052 : Registration page layout renders correctly on desktop, tablet, and mobile viewports
**Test Steps :**
Step 1 : Open the registration page on a desktop viewport (e.g., 1920x1080).
Step 2 : Resize/emulate a tablet viewport (e.g., 768x1024) and observe the layout.
Step 3 : Resize/emulate a mobile viewport (e.g., 375x667) and observe the layout.
**Expected Result :** All form fields, labels, and buttons remain visible, properly aligned, and usable at each viewport size, with no overlapping elements or horizontal scrolling.
 
### TC_053 : Submit button on registration form is disabled until all mandatory fields are valid
**Test Steps :**
Step 1 : Navigate to the registration page.
Step 2 : Observe the state of the "Register" button before any field is filled.
Step 3 : Progressively fill in valid values for all mandatory fields and observe the button's state.
**Expected Result :** The "Register" button is disabled/non-clickable (or shows a disabled visual style) until all mandatory fields contain valid values, at which point it becomes enabled.
 
### TC_054 : Loading indicator is displayed while event creation request is being processed
**Test Steps :**
Step 1 : Log in as admin, fill out a valid event creation form.
Step 2 : Click "Submit"/"Create Event".
Step 3 : Observe the UI immediately after clicking, before the response returns.
**Expected Result :** A loading indicator (spinner/progress bar) or disabled button state is shown while the request is in progress, preventing duplicate submissions, and disappears once the response is received.
 
### TC_055 : Error messages are displayed clearly near the relevant input field
**Test Steps :**
Step 1 : Trigger a validation error on any form (e.g., submit registration with an invalid email).
Step 2 : Observe the location and visual styling of the resulting error message.
Step 3 : Repeat for at least one other field/form to confirm consistency.
**Expected Result :** Error messages appear immediately adjacent to (or clearly associated with) the specific field in error, use a distinguishable color/icon (e.g., red text), and are written in clear, actionable language.
 
### TC_056 : Success confirmation message/toast is shown after successful event creation
**Test Steps :**
Step 1 : Log in as admin and successfully create a new event with valid details.
Step 2 : Observe the UI immediately after submission.
**Expected Result :** A clear success message/toast/banner confirms the event was created, and it disappears automatically or can be dismissed without disrupting navigation.
 
### TC_057 : Navigation menu is consistent and accessible across all pages
**Test Steps :**
Step 1 : Log in as a user and visit the home/event listing page; note the navigation menu items.
Step 2 : Navigate to event details, "My Bookings", and profile pages.
Step 3 : Compare the navigation menu's presence, items, and styling across all visited pages.
**Expected Result :** The navigation menu (header/nav bar) remains consistently positioned, styled, and functional across all pages, allowing the user to navigate back to any major section at any time.
 
### TC_058 : All interactive elements are reachable and operable via keyboard navigation
**Test Steps :**
Step 1 : Navigate to the registration or event creation form.
Step 2 : Use only the "Tab" key to move focus through all fields and buttons, and "Enter"/"Space" to activate buttons.
Step 3 : Observe whether focus order is logical and all elements are reachable/operable.
**Expected Result :** All form fields, links, and buttons are reachable in a logical order via keyboard alone, with a visible focus indicator, and actionable elements can be activated without a mouse.
 
### TC_059 : Form fields and buttons have appropriate labels for screen reader accessibility
**Test Steps :**
Step 1 : Inspect the registration, login, and event creation forms using browser dev tools or a screen reader.
Step 2 : Verify each input field has an associated `<label>` or `aria-label`.
Step 3 : Verify buttons and icons have descriptive accessible names.
**Expected Result :** All form fields and interactive elements have meaningful, descriptive labels accessible to assistive technologies, with no fields relying solely on placeholder text as a label.
 
### TC_060 : Event listing page maintains consistent card/grid layout across multiple events
**Test Steps :**
Step 1 : Log in as a user and navigate to the event listing page with multiple events of varying title/description lengths.
Step 2 : Observe the alignment, spacing, and sizing of each event card/row.
**Expected Result :** All event cards maintain a consistent layout (uniform sizing, alignment, spacing) regardless of variation in content length, with no broken or overlapping cards.
 
### TC_061 : Tooltips/hints are displayed for complex input fields (e.g., date format)
**Test Steps :**
Step 1 : Navigate to the event creation form.
Step 2 : Hover over or focus on fields with non-obvious input requirements (e.g., date/time format, price currency).
**Expected Result :** A tooltip, placeholder example, or helper text clarifies the expected input format for such fields.
 
### TC_062 : Color contrast of text and buttons meets basic accessibility/legibility standards
**Test Steps :**
Step 1 : Inspect the primary text and button colors against their backgrounds on key pages (login, registration, event listing) using a contrast-checking tool.
Step 2 : Compare the contrast ratios against WCAG AA guidelines (4.5:1 for normal text).
**Expected Result :** Text and interactive elements meet at least WCAG AA minimum contrast ratios, ensuring readability for users with visual impairments.
 
### TC_063 : Event listing page is responsive and usable on mobile devices
**Test Steps :**
Step 1 : Open the event listing page on a mobile device or emulator.
Step 2 : Scroll through the list, tap on an event card, and attempt to book an event.
**Expected Result :** All elements resize appropriately, touch targets (buttons/cards) are large enough to tap accurately, and the booking flow completes without layout issues on the mobile viewport.
 
---
 
## 6. Business Validation Test Cases
 
### TC_064 : Event created by admin is immediately visible to all users without requiring cache clear/page reload by admin
**Test Steps :**
Step 1 : In one browser session, log in as admin and create a new event.
Step 2 : In a separate browser session (or incognito window), log in as a different non-admin user without performing any cache-clearing actions.
Step 3 : Navigate to the event listing page.
**Expected Result :** The newly created event is visible to the non-admin user immediately (or after a normal page load/refresh), confirming there is no excessive caching or propagation delay preventing real-time visibility.
 
### TC_065 : System prevents/handles duplicate event names appropriately
**Test Steps :**
Step 1 : Log in as admin and create an event with a specific name (e.g., "Tech Summit 2026").
Step 2 : Attempt to create a second, different event using the exact same name.
Step 3 : Submit the second event creation form.
**Expected Result :** The system either blocks creation with a "duplicate event name" validation message, or allows it while clearly differentiating the two events (e.g., by date/ID) in the listing — behavior should be consistent and documented; no data should be overwritten or merged incorrectly.
 
### TC_066 : User cannot book an event once available seats reach zero
**Test Steps :**
Step 1 : Identify an event with exactly 1 available seat remaining.
Step 2 : As User A, book the last available seat.
Step 3 : As User B, attempt to book the same event immediately after.
**Expected Result :** User B's booking attempt is rejected with a "Sold Out"/"No seats available" message; the event's seat count correctly reflects zero, and no overbooking occurs.
 
### TC_067 : Available seat count decreases by one immediately after a successful booking
**Test Steps :**
Step 1 : Note the current "Available Seats" count on an event's detail page.
Step 2 : Book the event as a logged-in user.
Step 3 : Refresh/revisit the event detail page and note the updated seat count.
**Expected Result :** The displayed available seat count is exactly one less than before the booking, accurately reflecting real-time inventory.
 
### TC_068 : Only users with Admin role can access event creation/management functionality
**Test Steps :**
Step 1 : Log in as a non-admin user and confirm absence of event management options (cross-reference with TC_017).
Step 2 : Log in as an admin user and confirm presence of event management options.
Step 3 : Compare the role-based UI/feature differences between the two account types.
**Expected Result :** Event creation/management functionality is exclusively available to Admin-role accounts; regular user accounts have no path to this functionality through the UI.
 
### TC_069 : Non-admin users cannot edit or delete events created by admin
**Test Steps :**
Step 1 : Log in as a non-admin user and open an event created by admin.
Step 2 : Look for "Edit"/"Delete" options on the event detail/listing page.
Step 3 : If such options are somehow accessible (e.g., via API), attempt to invoke them.
**Expected Result :** No edit/delete controls are exposed to non-admin users in the UI, and any backend attempt to edit/delete via direct request is rejected with an authorization error; the event remains unchanged.
 
### TC_070 : Event listing is sorted/displayed in correct order (e.g., by date)
**Test Steps :**
Step 1 : As admin, create multiple events with different future dates.
Step 2 : Log in as a regular user and navigate to the event listing page.
Step 3 : Observe the order in which events are displayed.
**Expected Result :** Events are displayed in a logical, consistent order (e.g., soonest upcoming date first), matching the platform's documented/expected sorting behavior.
 
### TC_071 : Expired/past events are not shown in the active event listing for users
**Test Steps :**
Step 1 : As admin, identify or create an event whose date/time has already passed.
Step 2 : Log in as a regular user and navigate to the main/active event listing page.
**Expected Result :** The expired event does not appear in the default active event listing (it may optionally appear in a separate "Past Events" section if such a feature exists).
 
### TC_072 : A user cannot book the same event more than once (no duplicate bookings)
**Test Steps :**
Step 1 : Log in as a user and successfully book a specific event.
Step 2 : Navigate back to the same event's detail page.
Step 3 : Attempt to book the same event again.
**Expected Result :** The system prevents a duplicate booking for the same user/event combination — either by disabling the "Book" button (showing "Already Booked") or rejecting the second attempt with a clear message; the seat count is not decremented twice.
 
### TC_073 : Cancelled/deleted event by admin is removed from the user's event listing
**Test Steps :**
Step 1 : As admin, create an event, then cancel/delete it.
Step 2 : Log in as a regular user and navigate to the event listing page.
**Expected Result :** The cancelled/deleted event no longer appears in the user's event listing; if any user had already booked it, an appropriate notification/status update is reflected in "My Bookings" (e.g., "Cancelled").
 
### TC_074 : Concurrent booking requests for the last available seat are handled without overselling
**Test Steps :**
Step 1 : Identify an event with exactly 1 available seat remaining.
Step 2 : Simulate two users submitting a booking request for that same seat at nearly the same time (e.g., via two browser sessions or concurrent API calls).
Step 3 : Observe the outcome for both requests.
**Expected Result :** Only one booking request succeeds; the other is rejected with a "Sold Out"/"No seats available" message, and the final available seat count is exactly zero (no overselling/race condition).
 
### TC_075 : Event details (name, date, venue, price) shown to user match exactly what admin entered
**Test Steps :**
Step 1 : As admin, create an event with specific, distinct values for name, date, time, venue, and price.
Step 2 : Log in as a regular user and open the event's detail page.
Step 3 : Compare each displayed field against the values entered by admin in Step 1.
**Expected Result :** Every displayed field (name, date, time, venue, price, description, seats) matches exactly what the admin entered, with no truncation, formatting corruption, or data mismatch.
 
## MY THOUGHTS :
### ✅ Pros
-Speed & Coverage: AI can instantly generate dozens of test cases, covering positive, negative, boundary, and security scenarios that would take a human tester hours.
-Format Flexibility: It can output in Gherkin/BDD style, which integrates smoothly with automation frameworks like Cucumber or Karate.
-Effort Reduction: Saves manual effort in writing repetitive test cases, freeing testers to focus on exploratory and business‑critical testing.
### ⚠️ Cons
-Scenario Drift: AI sometimes generates test cases beyond the scope of the given functionality, which dilutes focus and creates confusion.
-Missing Business Context: While technically correct, AI lacks domain knowledge and business intelligence, so it struggles to design cases that reflect real‑world -workflows or customer priorities.
-Objective Misalignment: It may cover “all possible inputs” but miss the main objective of the scenario, leading to gaps in validation.
## FINAL TEST CASES (AI+HUMAN) COMBINED - AUTOMATION READY
### FTC_001 : Verify successful new user registration with valid details
**Test Steps:**
Step 1: Open https://eventhub.rahulshettyacademy.com/login.
Step 2: Click on the Register link.
Step 3: Enter a valid and unique email address.
Step 4: Enter a valid password that satisfies password policy requirements.
Step 5: Enter the same password in the Confirm Password field.
Step 6: Click on Create Account.
**Expected Result:**
User account should be created successfully.
User should be redirected to the Dashboard page.
 
### FTC_002 : Verify user registration fails with invalid email format
**Test Steps:**
Step 1: Open the Registration page.
Step 2: Enter an invalid email address.
Step 3: Enter a valid password.
Step 4: Enter matching Confirm Password.
Step 5: Click on Create Account.
**Expected Result:**
Registration should fail.
Appropriate email validation message should be displayed.
 
### FTC_003 : Verify user registration fails when password does not meet password policy requirements
**Test Steps:**
Step 1: Open the Registration page.
Step 2: Enter a valid email address.
Step 3: Enter an invalid password that does not satisfy password requirements.
Step 4: Enter the same password in Confirm Password.
Step 5: Click on Create Account.
**Expected Result:**
Registration should fail.
Password validation message should be displayed.
 
### FTC_004 : Verify user registration fails when Password and Confirm Password do not match
**Test Steps:**
Step 1: Open the Registration page.
Step 2: Enter a valid email address.
Step 3: Enter a valid password.
Step 4: Enter a different password in Confirm Password.
Step 5: Click on Create Account.
**Expected Result:**
Registration should fail.
Password mismatch validation message should be displayed.
 
### FTC_005 : Verify user registration fails with an already registered email address
**Test Steps:**
Step 1: Open the Registration page.
Step 2: Enter an already registered email address.
Step 3: Enter a valid password.
Step 4: Enter matching Confirm Password.
Step 5: Click on Create Account.
**Expected Result:**
Registration should fail.
"Email already registered" message should be displayed.
 
### FTC_006 : Verify Admin menu is visible after successful user registration
**Test Steps:**
Step 1: Register a new user successfully.
Step 2: Observe the Dashboard page.
Step 3: Verify the Admin dropdown menu.
**Expected Result:**
Admin dropdown should be visible.
Manage Events option should be displayed.
Manage Bookings option should be displayed.
 
### FTC_007 : Verify navigation to Manage Events page from Admin menu
**Test Steps:**
Step 1: Click on Admin menu.
Step 2: Click on Manage Events.
**Expected Result:**
User should be redirected to the Event Management page.
Event creation form should be displayed.
 
### FTC_008 : Verify event creation fails when mandatory fields are left blank
**Test Steps:**
Step 1: Navigate to Manage Events page.
Step 2: Leave mandatory fields blank.
Step 3: Click on Submit.
**Expected Result:**
Event should not be created.
Validation messages should be displayed for mandatory fields.
 
### FTC_009 : Verify successful creation of a new event with valid details
**Test Steps:**
Step 1: Navigate to Manage Events page.
Step 2: Enter valid Event Name.
Step 3: Enter valid Event Description.
Step 4: Select a future Event Date.
Step 5: Enter valid Event Time.
Step 6: Enter valid Venue.
Step 7: Enter valid Available Seats.
Step 8: Upload a valid event image if applicable.
Step 9: Click on Submit.
**Expected Result:**
Event should be created successfully.
Success confirmation message should be displayed.
 
### FTC_010 : Verify newly created event is displayed in Events List
**Test Steps:**
Step 1: Create a new event.
Step 2: Navigate to Events List.
Step 3: Search for the newly created event.
**Expected Result:**
Newly created event should be visible in the Events List.
Event details should match the entered values.
 
### FTC_011 : Verify event creation fails when a past date is selected
**Test Steps:**
Step 1: Navigate to Manage Events page.
Step 2: Enter valid event details.
Step 3: Select a past date.
Step 4: Click on Submit.
**Expected Result:**
Event should not be created.
Appropriate date validation message should be displayed.
 
### FTC_012 : Verify event creation fails when an unsupported file type is uploaded
**Test Steps:**
Step 1: Navigate to Manage Events page.
Step 2: Fill all mandatory fields.
Step 3: Upload an unsupported file format.
Step 4: Click on Submit.
**Expected Result:**
File upload should be rejected.
Appropriate validation message should be displayed.
 
### FTC_013 : Verify another registered user can successfully log in
**Test Steps:**
Step 1: Logout from the current account.
Step 2: Navigate to Login page.
Step 3: Enter valid credentials of another registered user.
Step 4: Click on Login.
**Expected Result:**
User should be logged in successfully.
Event Listing page should be displayed.
 
### FTC_014 : Verify newly created event is visible to another user
**Test Steps:**
Step 1: Login using another registered user account.
Step 2: Navigate to Events Listing page.
Step 3: Search for the event created earlier.
**Expected Result:**
Newly created event should be visible in the Events List.
Event details should be displayed correctly.
 
### FTC_015 : Verify event details displayed to another user match the details entered during event creation
**Test Steps:**
Step 1: Login using another registered user account.
Step 2: Open the newly created event.
Step 3: Verify Event Name, Description, Date, Time, Venue and Available Seats.
**Expected Result:**
All event details should match the values entered during event creation.


