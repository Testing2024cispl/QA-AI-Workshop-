# BlazeDemo Test Cases – Full Document

---

## Section 1: Original Manual Test Cases

### Test Case 1 – User Login with Valid Credentials
**Scenario:** Verify that a user can successfully log in to the application using a valid email address and password.

Open Browser , Enter the Urls , Landing page will get display , Click on Home it will redirect to Login page , Enter valid Email , Valid Password , Click on login button

**Expected result >** User should created confirmation message should get display

### Test Case 2 – Login Attempt with an Existing User Account
**Scenario:** Verify the system behavior when an existing user attempts to log in using valid credentials and ensure the appropriate confirmation message is displayed.

Open Browser , Enter the Urls , Landing page will get display , Click on Home it will redirect to Login page , Enter Existing  Email , Valid Password , Click on login button

**Expected result >** User is existed already , confirmation popup should get display

### Test Case 3 – Login Attempt with Blank Mandatory Fields
**Scenario:** Verify that the application validates mandatory login fields and highlights them when the user attempts to log in without providing any data.

Open Browser , Enter the Urls , Landing page will get display , Click on Home it will redirect to Login page , Dont enter any data , Click on login button, mandatory fields should get highlighted

**Expected result >** User should created confirmation message should get display

### Test Case 4 – Forgot Password with Valid Email Address
**Scenario:** Verify that a password reset request can be successfully initiated using a valid registered email address and that the user receives a confirmation email.

Open Browser , Enter the Urls , Landing page will get display , Click on Home it will redirect to Login page , Click on forget password link , Enter valid Email click on send invitation button and check user should get confirmation mail

**Expected result >** User should get confirmation mail

### Test Case 5 – Forgot Password with Invalid Email Address
**Scenario:** Verify that the application displays an appropriate validation message when an invalid email address is entered during the password reset process.

Open Browser , Enter the Urls , Landing page will get display , Click on Home it will redirect to Login page , Click on forget password link , Enter Invalid valid Email click on send invitation button

**Expected result >** Its should display Please enter valid email address

### Test Case 6 – Forgot Password with Empty Email Field
**Scenario:** Verify that the email field is mandatory on the forgot password page and that validation messages are displayed when the field is left blank.

Open Browser , Enter the Urls , Landing page will get display , Click on Home it will redirect to Login page , Click on forget password link , Dont Enter any email click on send invitation button Expected result > Mandatory Field should get Highlighted

### Test Case 7 – New User Registration with Valid Details
**Scenario:** Verify that a new user can successfully register by providing all required valid information.

Open Browser , Enter the Urls , Landing page will get display , Click on Home it will redirect to Login page , Click on register , Enter valid name , valid company , Valid Email, Valid password and confirm password click on Register button

**Expected result >** New User get created confirmation should get display

### Test Case 8 – User Registration with Mismatched Passwords
**Scenario:** Verify that the application prevents user registration when the password and confirm password fields do not match.

Open Browser , Enter the Urls , Landing page will get display , Click on Home it will redirect to Login page , Click on register , Enter valid name , valid company , Valid Email, Valid password and enter invalid  confirm password click on Register button

**Expected result >** Password not matched , popup will get display

### Test Case 9 – User Registration with Blank Mandatory Fields
**Scenario:** Verify that all mandatory fields on the registration page are validated and highlighted when the user attempts to register without entering any information.

Open Browser , Enter the Urls , Landing page will get display , Click on Home it will redirect to Login page , Click on register , Dont enter any data , Click on Register button , Mandatory fields should get highlighted

**Expected result >** New User get created confirmation should get display

### Test Case 10 – Flight Booking with Valid Details
**Scenario:** Verify that a user can successfully search for flights, select a flight, complete the booking process with valid information, and view the booking confirmation details on the confirmation page.

Open Browser , Enter the Urls , Landing page will get display , Chose Departure city  , choose destination , click on Find Flights , Check reserve.php page  is getting display with all Details , click on Choose flight , Enter all the Valid data , and click on Purchase flights

**Expected result >** All the data , is getting display in Thankyou page with confirmation popup

---

## PROMPT
**Act as senior Employee with have 5+ years of experience in software testing and give me the testcase of the following**

# AI MANUAL Test Cases – BlazeDemo

**Application Name:** BlazeDemo
**Application URL:** https://blazedemo.com/
**Module:** Authentication & Flight Booking
**Prepared By:** QA Team
**Document Version:** 1.0

---

## Section 2: AI Structured Test Cases

### Test Case ID: TC_001
**Test Case Name:** User Login with Valid Credentials

**Scenario:** Verify that a user can successfully log in to the application using valid credentials.

**Preconditions:**
- User must be registered in the application.
- Application URL should be accessible.

**Test Steps:**
- Launch the browser.
- Navigate to the application URL.
- Verify that the landing page is displayed.
- Click on the Home link.
- Verify that the Login page is displayed.
- Enter a valid email address.
- Enter a valid password.
- Click the Login button.

**Expected Result:**
- User should be logged in successfully.
- A successful login confirmation message should be displayed.
- User should be redirected to the dashboard/home page.

### Test Case ID: TC_002
**Test Case Name:** Login Attempt with Existing User Account

**Scenario:** Verify the system behavior when an existing user attempts to log in using valid credentials.

**Preconditions:**
- User account must already exist.

**Test Steps:**
- Launch the browser.
- Navigate to the application URL.
- Verify that the landing page is displayed.
- Click on the Home link.
- Verify that the Login page is displayed.
- Enter an existing email address.
- Enter a valid password.
- Click the Login button.

**Expected Result:**
- User should be logged in successfully.
- Appropriate confirmation message should be displayed.

### Test Case ID: TC_003
**Test Case Name:** Login with Blank Mandatory Fields

**Scenario:** Verify that mandatory fields are validated when no data is entered.

**Preconditions:**
- User should be on the Login page.

**Test Steps:**
- Launch the browser.
- Navigate to the application URL.
- Verify that the landing page is displayed.
- Click on the Home link.
- Verify that the Login page is displayed.
- Leave all fields blank.
- Click the Login button.

**Expected Result:**
- Mandatory fields should be highlighted.
- Appropriate validation messages should be displayed.
- User should not be able to log in.

### Test Case ID: TC_004
**Test Case Name:** Forgot Password with Valid Email Address

**Scenario:** Verify that a password reset request can be initiated using a valid email address.

**Preconditions:**
- User email address must be registered.

**Test Steps:**
- Launch the browser.
- Navigate to the application URL.
- Verify that the landing page is displayed.
- Click on the Home link.
- Navigate to the Login page.
- Click the Forgot Password link.
- Enter a valid email address.
- Click the Send Invitation button.

**Expected Result:**
- Password reset request should be submitted successfully.
- User should receive a confirmation email.
- Success message should be displayed.

### Test Case ID: TC_005
**Test Case Name:** Forgot Password with Invalid Email Address

**Scenario:** Verify validation when an invalid email address is entered.

**Preconditions:**
- User should be on the Forgot Password page.

**Test Steps:**
- Launch the browser.
- Navigate to the application URL.
- Verify that the landing page is displayed.
- Click on the Home link.
- Navigate to the Login page.
- Click the Forgot Password link.
- Enter an invalid email address.
- Click the Send Invitation button.

**Expected Result:**
- Appropriate validation message should be displayed.
- Error message: "Please enter a valid email address."
- Password reset request should not be submitted.

### Test Case ID: TC_006
**Test Case Name:** Forgot Password with Empty Email Field

**Scenario:** Verify that the email field is mandatory on the Forgot Password page.

**Preconditions:**
- User should be on the Forgot Password page.

**Test Steps:**
- Launch the browser.
- Navigate to the application URL.
- Verify that the landing page is displayed.
- Click on the Home link.
- Navigate to the Login page.
- Click the Forgot Password link.
- Leave the email field blank.
- Click the Send Invitation button.

**Expected Result:**
- Mandatory field should be highlighted.
- Appropriate validation message should be displayed.
- Password reset request should not be submitted.

### Test Case ID: TC_007
**Test Case Name:** New User Registration with Valid Details

**Scenario:** Verify that a new user can register successfully using valid details.

**Preconditions:**
- User account should not already exist.

**Test Steps:**
- Launch the browser.
- Navigate to the application URL.
- Verify that the landing page is displayed.
- Click on the Home link.
- Navigate to the Login page.
- Click the Register link.
- Enter a valid name.
- Enter a valid company name.
- Enter a valid email address.
- Enter a valid password.
- Enter the same password in the Confirm Password field.
- Click the Register button.

**Expected Result:**
- New user account should be created successfully.
- Registration confirmation message should be displayed.

### Test Case ID: TC_008
**Test Case Name:** User Registration with Mismatched Passwords

**Scenario:** Verify that the application prevents registration when passwords do not match.

**Preconditions:**
- User should be on the Registration page.

**Test Steps:**
- Launch the browser.
- Navigate to the application URL.
- Verify that the landing page is displayed.
- Click on the Home link.
- Navigate to the Login page.
- Click the Register link.
- Enter valid user details.
- Enter a valid password.
- Enter a different value in the Confirm Password field.
- Click the Register button.

**Expected Result:**
- Registration should fail.
- Error message: "Passwords do not match" should be displayed.
- User account should not be created.

### Test Case ID: TC_009
**Test Case Name:** User Registration with Blank Mandatory Fields

**Scenario:** Verify validation for mandatory registration fields.

**Preconditions:**
- User should be on the Registration page.

**Test Steps:**
- Launch the browser.
- Navigate to the application URL.
- Verify that the landing page is displayed.
- Click on the Home link.
- Navigate to the Login page.
- Click the Register link.
- Leave all fields blank.
- Click the Register button.

**Expected Result:**
- Mandatory fields should be highlighted.
- Appropriate validation messages should be displayed.
- User account should not be created.

### Test Case ID: TC_010
**Test Case Name:** Flight Booking with Valid Details

**Scenario:** Verify that a user can successfully search, select, and book a flight using valid details.

**Preconditions:**
- Application URL should be accessible.

**Test Steps:**
- Launch the browser.
- Navigate to the application URL.
- Verify that the landing page is displayed.
- Select the departure city.
- Select the destination city.
- Click the Find Flights button.
- Verify that the flight results page is displayed.
- Verify that available flight details are displayed.
- Click the Choose This Flight button.
- Enter valid passenger details.
- Enter valid payment details.
- Click the Purchase Flight button.

**Expected Result:**
- Booking should be completed successfully.
- Thank You page should be displayed.
- Booking confirmation message should be displayed.
- All entered booking details should be displayed correctly.

---

## Section 3: AI + Manual Combined Test Cases – BlazeDemo

### Test Case ID: TC_001
**Test Case Name:** User Login with Valid Credentials

**Scenario:** Verify that a user can successfully log in to the application using a valid email address and password.

**Preconditions:**
- User must be registered in the application.
- Application URL should be accessible.

**Test Steps:**
- Launch the browser.
- Navigate to https://blazedemo.com/.
- Verify that the landing page is displayed.
- Click on the Home link; verify redirection to the Login page.
- Enter a valid email address.
- Enter a valid password.
- Click the Login button.

**Expected Result:**
- User should be logged in successfully.
- A "User created/login successful" confirmation message should be displayed.
- User should be redirected to the dashboard/home page.

### Test Case ID: TC_002
**Test Case Name:** Login Attempt with an Existing User Account

**Scenario:** Verify the system behavior when an existing user attempts to log in using valid credentials, and ensure the appropriate confirmation message is displayed.

**Preconditions:**
- User account must already exist in the system.

**Test Steps:**
- Launch the browser.
- Navigate to https://blazedemo.com/.
- Verify that the landing page is displayed.
- Click on the Home link; verify redirection to the Login page.
- Enter an existing/registered email address.
- Enter the valid password.
- Click the Login button.

**Expected Result:**
- System should recognize the user as already existing.
- A confirmation popup ("User already exists / Login successful") should be displayed.

### Test Case ID: TC_003
**Test Case Name:** Login Attempt with Blank Mandatory Fields

**Scenario:** Verify that the application validates mandatory login fields and highlights them when the user attempts to log in without providing any data.

**Preconditions:**
- User should be on the Login page.

**Test Steps:**
- Launch the browser.
- Navigate to https://blazedemo.com/.
- Verify that the landing page is displayed.
- Click on the Home link; verify redirection to the Login page.
- Leave the email and password fields blank.
- Click the Login button.

**Expected Result:**
- Mandatory fields (Email, Password) should be highlighted in red/error state.
- Appropriate validation message should be displayed.
- User should not be logged in and no confirmation message should appear.

**Note (Human review):** Original notes listed the expected result as a "User created confirmation message" — this was corrected, since blank mandatory fields should block login, not confirm it.

### Test Case ID: TC_004
**Test Case Name:** Forgot Password with Valid Email Address

**Scenario:** Verify that a password reset request can be successfully initiated using a valid registered email address and that the user receives a confirmation email.

**Preconditions:**
- User's email address must already be registered.

**Test Steps:**
- Launch the browser.
- Navigate to https://blazedemo.com/.
- Verify that the landing page is displayed.
- Click on the Home link; verify redirection to the Login page.
- Click the Forgot Password link.
- Enter a valid registered email address.
- Click the Send Invitation button.
- Check the registered inbox for a confirmation email.

**Expected Result:**
- Password reset request should be submitted successfully.
- User should receive a confirmation email.
- A success message should be displayed on screen.

### Test Case ID: TC_005
**Test Case Name:** Forgot Password with Invalid Email Address

**Scenario:** Verify that the application displays an appropriate validation message when an invalid email address is entered during the password reset process.

**Preconditions:**
- User should be on the Forgot Password page.

**Test Steps:**
- Launch the browser.
- Navigate to https://blazedemo.com/.
- Verify that the landing page is displayed.
- Click on the Home link; verify redirection to the Login page.
- Click the Forgot Password link.
- Enter an invalid email address (e.g., wrong format).
- Click the Send Invitation button.

**Expected Result:**
- Validation message "Please enter a valid email address" should be displayed.
- Password reset request should not be submitted.

### Test Case ID: TC_006
**Test Case Name:** Forgot Password with Empty Email Field

**Scenario:** Verify that the email field is mandatory on the Forgot Password page and that validation messages are displayed when the field is left blank.

**Preconditions:**
- User should be on the Forgot Password page.

**Test Steps:**
- Launch the browser.
- Navigate to https://blazedemo.com/.
- Verify that the landing page is displayed.
- Click on the Home link; verify redirection to the Login page.
- Click the Forgot Password link.
- Leave the email field blank.
- Click the Send Invitation button.

**Expected Result:**
- Mandatory email field should be highlighted.
- Appropriate validation message should be displayed.
- Password reset request should not be submitted.

### Test Case ID: TC_007
**Test Case Name:** New User Registration with Valid Details

**Scenario:** Verify that a new user can successfully register by providing all required valid information.

**Preconditions:**
- User account should not already exist.

**Test Steps:**
- Launch the browser.
- Navigate to https://blazedemo.com/.
- Verify that the landing page is displayed.
- Click on the Home link; verify redirection to the Login page.
- Click the Register link.
- Enter a valid name.
- Enter a valid company name.
- Enter a valid email address.
- Enter a valid password.
- Enter the same value in the Confirm Password field.
- Click the Register button.

**Expected Result:**
- New user account should be created successfully.
- A "New user created" confirmation message should be displayed.

### Test Case ID: TC_008
**Test Case Name:** User Registration with Mismatched Passwords

**Scenario:** Verify that the application prevents user registration when the password and confirm password fields do not match.

**Preconditions:**
- User should be on the Registration page.

**Test Steps:**
- Launch the browser.
- Navigate to https://blazedemo.com/.
- Verify that the landing page is displayed.
- Click on the Home link; verify redirection to the Login page.
- Click the Register link.
- Enter valid name, company, and email.
- Enter a valid password.
- Enter a different/invalid value in the Confirm Password field.
- Click the Register button.

**Expected Result:**
- Registration should fail.
- A "Passwords do not match" popup/error message should be displayed.
- User account should not be created.

### Test Case ID: TC_009
**Test Case Name:** User Registration with Blank Mandatory Fields

**Scenario:** Verify that all mandatory fields on the registration page are validated and highlighted when the user attempts to register without entering any information.

**Preconditions:**
- User should be on the Registration page.

**Test Steps:**
- Launch the browser.
- Navigate to https://blazedemo.com/.
- Verify that the landing page is displayed.
- Click on the Home link; verify redirection to the Login page.
- Click the Register link.
- Leave all fields (Name, Company, Email, Password, Confirm Password) blank.
- Click the Register button.

**Expected Result:**
- Mandatory fields should be highlighted in red/error state.
- Appropriate validation messages should be displayed.
- User account should not be created and no confirmation message should appear.

**Note (Human review):** Original notes listed the expected result as a "New user created confirmation message" — corrected, since blank mandatory fields should prevent account creation, not confirm it.

### Test Case ID: TC_010
**Test Case Name:** Flight Booking with Valid Details

**Scenario:** Verify that a user can successfully search for flights, select a flight, complete the booking process with valid information, and view the booking confirmation details on the confirmation page.

**Preconditions:**
- Application URL should be accessible.

**Test Steps:**
- Launch the browser.
- Navigate to https://blazedemo.com/.
- Verify that the landing page is displayed.
- Select the departure city from the dropdown.
- Select the destination city from the dropdown.
- Click the Find Flights button.
- Verify that the reserve.php (flight results) page is displayed with all flight details.
- Click the Choose This Flight button for the desired flight.
- Enter all valid passenger and payment details on the purchase page.
- Click the Purchase Flight button.

**Expected Result:**
- Booking should be completed successfully.
- The Thank You/Purchase Confirmation page should be displayed.
- All entered booking details (passenger info, flight info) should be correctly displayed on the confirmation page.
- A booking confirmation popup/message should be displayed.

---

## Summary of Human + AI Review

- **AI contribution:** Added structured Preconditions, numbered Test Steps, and detailed Expected Results for traceability and consistency.
- **Human contribution:** Provided original scenario intent, real navigation flow (Home → Login → Register/Forgot Password), and field-level testing context from manual exploration of BlazeDemo.
- **Corrections made during review:** TC_003 and TC_009 expected results were corrected — blank mandatory field submissions should be blocked with validation, not result in a success/confirmation message as originally noted.
