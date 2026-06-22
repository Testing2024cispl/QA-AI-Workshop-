https://eventhub.rahulshettyacademy.com/login

Test case by QA:

## TC_001: New User Creation with Valid Data

### Test Steps:

1. Open the EventHub application URL in a browser.
2. Click on the Register link below the Sign In section.
3. Enter a valid email address.
4. Enter a valid password that follows the password rules.
5. Enter the same password in the Confirm Password field.
6. Click on the Create Account button.

---

## TC_002: New User Creation with Invalid Email Format

### Test Steps:

1. Open the EventHub application URL in a browser.
2. Click on the Register link below the Sign In section.
3. Enter an invalid email address format.
4. Enter a valid password.
5. Enter the same password in the Confirm Password field.
6. Click on the Create Account button.

---

## TC_003: Verify User Creation Fails When Password Does Not Meet Required Format

### Test Steps:

1. Open the EventHub application URL in a browser.
2. Click on the Register link below the Sign In section.
3. Enter a valid email address.
4. Enter a password that does not satisfy the password requirements.
5. Enter the same password in the Confirm Password field.
6. Click on the Create Account button.

---

## TC_004: Verify User Creation Fails When Confirm Password Does Not Match Password

### Test Steps:

1. Open the EventHub application URL in a browser.
2. Click on the Register link below the Sign In section.
3. Enter a valid email address.
4. Enter a valid password.
5. Enter a different password in the Confirm Password field.
6. Click on the Create Account button.

---

## TC_005: Verify User Creation Fails When Mandatory Fields Are Left Blank

### Test Steps:

1. Open the EventHub application URL in a browser.
2. Click on the Register link below the Sign In section.
3. Leave the Email field blank.
4. Leave the Password field blank.
5. Leave the Confirm Password field blank.
6. Click on the Create Account button.

---

## TC_006: Verify Copy-Paste Functionality Is Disabled for Password Fields

### Test Steps:

1. Open the EventHub application URL in a browser.
2. Click on the Register link below the Sign In section.
3. Enter a valid email address.
4. Enter a valid password.
5. Select and copy the password.
6. Try to paste the copied password into the Confirm Password field.

---

## TC_007: Verify User Registration with Already Registered Email Address

### Test Steps:

1. Open the EventHub application URL in a browser.
2. Click on the Register link below the Sign In section.
3. Enter an already registered email address.
4. Enter a valid password.
5. Enter the same password in the Confirm Password field.
6. Click on the Create Account button.

---

## TC_008: Verify Admin Section Visibility After Successful Registration

### Test Steps:

1. Open the EventHub application URL in a browser.
2. Click on the Register link below the Sign In section.
3. Enter a valid email address.
4. Enter a valid password.
5. Enter the same password in the Confirm Password field.
6. Click on the Create Account button.
7. Wait for the application to redirect to the Dashboard page.
8. Check whether the Admin dropdown is displayed.




---

# EventHub Application Test Cases

---

## TC_001: New User Creation with Valid Data

**Precondition:** User email is not already registered.

**Test Steps:**

1. Open the application URL in a browser.
2. Click the **Register** link below the Sign In section.
3. Enter a valid email address.
4. Enter a valid password that satisfies all password requirements.
5. Enter the same password in the Confirm Password field.
6. Click the **Create Account** button.

**Expected Result:**

1. User account should be created successfully.
2. User should be redirected to the Dashboard page.

---

## TC_002: New User Creation with Invalid Email Format

**Precondition:** Registration page is accessible.

**Test Steps:**

1. Open the application URL.
2. Click the **Register** link.
3. Enter an invalid email format (e.g., testemail.com).
4. Enter a valid password.
5. Enter the same password in Confirm Password.
6. Click **Create Account**.

**Expected Result:**

1. Account should not be created.
2. Email validation error message should be displayed.

---

## TC_003: Verify User Creation Fails When Password Does Not Meet Required Format

**Test Steps:**

1. Open the application URL.
2. Click the **Register** link.
3. Enter a valid email address.
4. Enter a password that does not satisfy the password requirements.
5. Enter the same password in Confirm Password.
6. Click **Create Account**.

**Expected Result:**

1. Account should not be created.
2. Error message "Password does not meet the requirements below" should be displayed.

---

## TC_004: Verify User Creation Fails When Confirm Password Does Not Match

**Test Steps:**

1. Open the application URL.
2. Click the **Register** link.
3. Enter a valid email address.
4. Enter a valid password.
5. Enter a different password in Confirm Password.
6. Click **Create Account**.

**Expected Result:**

1. Account should not be created.
2. Error message "Password does not match" should be displayed.

---

## TC_005: Verify User Creation Fails When Mandatory Fields Are Blank

**Test Steps:**

1. Open the application URL.
2. Click the **Register** link.
3. Leave Email field blank.
4. Leave Password field blank.
5. Leave Confirm Password field blank.
6. Click **Create Account**.

**Expected Result:**

1. User registration should not proceed.
2. Validation messages should appear for all mandatory fields.

---

## TC_006: Verify Copy-Paste Functionality Is Disabled for Password Fields

**Test Steps:**

1. Open the application URL.
2. Click the **Register** link.
3. Enter a valid email address.
4. Enter a valid password.
5. Select and copy the password.
6. Attempt to paste it into the Confirm Password field.

**Expected Result:**

1. Copy and paste functionality should be disabled.
2. User should manually enter the Confirm Password value.

---

## TC_007: Verify Registration with Already Registered Email Address

**Precondition:** Email address already exists in the system.

**Test Steps:**

1. Open the application URL.
2. Click the **Register** link.
3. Enter an already registered email address.
4. Enter a valid password.
5. Enter the same password in Confirm Password.
6. Click **Create Account**.

**Expected Result:**

1. Registration should fail.
2. "Email Address Already Registered" message should be displayed.

---

## TC_008: Verify Dashboard and Admin Section Visibility After Registration

**Test Steps:**

1. Complete a successful registration.
2. Observe the Dashboard page after redirection.
3. Verify the navigation menu.

**Expected Result:**

1. Dashboard should be displayed.
2. Admin dropdown should be visible.
3. Admin dropdown should contain:

   * Manage Events
   * Manage Bookings

---

## TC_009: Verify Manage Events Navigation

**Precondition:** User is logged in as Admin.

**Test Steps:**

1. Click the Admin dropdown menu.
2. Click the **Manage Events** option.

**Expected Result:**

1. User should be redirected to the New Event page.

---

## TC_010: Verify New Event Creation

**Precondition:** User is on New Event page.

**Test Steps:**

1. Enter Event Name.
2. Select Event Date.
3. Enter Event Location.
4. Enter Event Description.
5. Fill all remaining mandatory fields.
6. Click **Submit**.

**Expected Result:**

1. Event should be created successfully.
2. Success message should be displayed.
3. Newly created event should appear in the Events List.

---

## TC_011: Verify Login with Valid Credentials

**Precondition:** User account exists.

**Test Steps:**

1. Open the Login page.
2. Enter a valid registered email.
3. Enter the correct password.
4. Click **Sign In**.

**Expected Result:**

1. User should be logged in successfully.
2. Dashboard page should be displayed.

---

## TC_012: Verify Login with Invalid Password

**Precondition:** User account exists.

**Test Steps:**

1. Open the Login page.
2. Enter a valid email address.
3. Enter an incorrect password.
4. Click **Sign In**.

**Expected Result:**

1. Login should fail.
2. Appropriate error message should be displayed.

---

## TC_013: Verify Event Creation with Missing Mandatory Fields

**Precondition:** Admin user is on the New Event page.

**Test Steps:**

1. Enter Event Name.
2. Leave Event Date blank.
3. Fill remaining fields.
4. Click **Submit**.

**Expected Result:**

1. Event should not be created.
2. Validation message should be displayed for the missing field.

---

## TC_014: Verify Event Date Cannot Be Earlier Than Current Date

**Test Steps:**

1. Navigate to New Event page.
2. Enter all mandatory details.
3. Select a past date.
4. Click **Submit**.

**Expected Result:**

1. Event creation should fail.
2. Validation message should indicate invalid date selection.

---

## TC_015: Verify Unauthorized User Cannot Access Admin Pages

**Precondition:** User is not logged in.

**Test Steps:**

1. Copy an Admin page URL.
2. Open a new browser tab.
3. Paste the Admin URL directly.
4. Press Enter.

**Expected Result:**

1. User should be redirected to Login page.
2. Admin page should not be accessible.

---

## TC_016: Verify Session Termination After Logout

**Precondition:** User is logged in.

**Test Steps:**

1. Click Logout.
2. Verify redirection to Login page.
3. Click browser Back button.

**Expected Result:**

1. Previously visited protected pages should not be accessible.
2. User should remain logged out.

---

## TC_017: Verify SQL Injection Handling in Login Form

**Test Steps:**

1. Open Login page.
2. Enter SQL injection string in Email field.
3. Enter SQL injection string in Password field.
4. Click Sign In.

**Expected Result:**

1. Login should fail.
2. Application should not crash.
3. SQL code should not be executed.

---

## TC_018: Verify XSS Protection in Event Description Field

**Test Steps:**

1. Navigate to New Event page.
2. Enter valid event information.
3. Enter "<script>alert('XSS')</script>" in Description field.
4. Submit the event.

**Expected Result:**

1. Script should not execute.
2. Input should be sanitized or rejected.
3. Application should remain secure.

