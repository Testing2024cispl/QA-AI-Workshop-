# Table of Contents

- [QA Manual Test Cases](#qa-manual-test-cases)
- [Human Thinking Test Cases](#human-thinking-test-cases)
- [AI Manual Test Cases](#ai-manual-test-cases)
- [Prompt](#prompt)
- [My Thoughts](#my-thoughts)
- [Final Test Cases (AI + Manual Combined) – Automation Ready](#final-test-cases-ai--manual-combined--automation-ready)

# QA Manual Test Cases   

## Member:- Tista Dutta.  
Query/Test cases:- Write test cases based on the given website  https://eventhub.rahulshettyacademy.com/   
---

## Human Thinking Test Cases  

### TestCase_001 – New User Registration with Valid Data
---
1. Open EventHub website.  
2. Click on "Register".  
3. Enter a valid email address.  
4. Enter a password satisfying all requirements.  
5. Enter the same password in the Confirm Password field.  
6. Click Create Account.  
7. Verify that account is created successfully.  
8. Verify that the user is redirected to the login page.   

### TestCase_002 – Registration with Empty Fields  
---
1. Open EventHub website.  
2. Click on Register.  
3. Leave all fields blank.  
4. Click Create Account.  
5. Verify mandatory field validation messages are displayed.
 
### TestCase_003 – Registration with Existing Email.  
---
1. Open EventHub website.  
2. Click Register.  
3. Enter an email already registered.  
4. Enter valid password.  
5. Click Create Account.  
5. Verify appropriate error messages are displayed.  


### TestCase_004 – Registration with Invalid Email   
---
1. Open EventHub website.  
2. Click on "Register".  
3. Enter invalid email format.  
4. Enter valid password.  
5. Enter confirm password.  
6. Click Create Account.  
7. Verify validation message is displayed.  

### TestCase_005 – Registration with Password Mismatch 
---
1. Open EventHub website.  
2. Enter valid email.  
3. Enter password.  
4. Enter a different confirm password.  
5. Click Create Account.  
6. Verify password mismatch message.  

### TestCase_006 – Login with Valid Credentials  
---
1. Open EventHub website.  
2. Enter a registered email.  
3. Enter valid password.  
4. Click Sign In.  
5. Verify successful login.  
6. Verify the dashboard is displayed.
     
### TestCase_007 – Login with Invalid Password  
---
1. Open EventHub website.  
1. Enter a registered email.  
1. Enter the wrong password.  
1. Click Sign In.  
1. Verify error message.  

### TestCase_008 – Session Persistence after Refresh  
---
1. Login with valid credentials.  
2. Refresh browser.  
3. Verify the user remains logged in. 

### TestCase_009 – Access Protected Page Without Login  
---
1. Copy a protected URL.  
2. Open it in a new browser without login.  
3. Verify the user is redirected to the Login page.  

### TestCase_010 – Browse Available Events  
---
1. Login with valid credentials.  
2. Click Browse Events.
3. Verify the event list is displayed.

### TestCase_011 – Search Event  
---
1. Login with valid credentials.
2. Navigate to Browse Events.
3. Search event by keyword.
4. Verify relevant events appear.

### TestCase_012 – Search Non-Existing Event  
---
1. Login with valid credentials.
2. Navigate to Browse Events.
3. Search with invalid keywords.
4. Verify "No events found" message.


### TestCase_013 – Event Booking
---
1. Login with valid credentials.
2. Click on the ‘Browse Events’ button.
3. Select an available event.
4. Click ‘Book Now’.
5. Enter Full Name, Email, Phone Number and Select number of tickets.
6. Click the button ‘Confirm booking’.
7. Verify the success message.
8. Verify booking appears in the My Bookings section.

### TestCase_014 – Duplicate Event Booking  
---
1. Login with valid credentials.  
2. Click on the ‘Browse Events’ button.  
3. Select an available event.  
4. Click ‘Book Now’.  
5. Enter Full Name, Email, Phone Number and Select number of tickets.  
6. Click the button ‘Confirm booking’.  
7. Attempt to book the same event again.  
8. Verify duplicate booking is prevented.
   
### TestCase_015 – Booking with Invalid Phone Number.  
---
1.  Login with valid credentials.  
1. Click on the ‘Browse Events’ button.  
1.  Select an available event.  
1.  Click ‘Book Now’.  
1.  Enter invalid phone number.  
1.  Submit booking.  
1.  Verify validation message.  

### TestCase_016 – Cancel Event Booking  
---
1. Login with valid credentials.  
2. Navigate to My Bookings.  
3. Select booked event.  
4. Click Cancel Booking.  
5. Confirm cancellation.  
6. Verify booking is removed.  
7. Verify the success message.  

### TestCase_017 – Logout  
---
1. Login with valid credentials.  
2. Click the Logout button on the EventHub menu.  
3. Verify the user is logged out.  
4. Verify the login page is displayed.  
---

# AI Manual Test Cases   
Member:- Tista Dutta.  
---

# Prompt 

### Role:  
Act as a Senior QA Engineer with expertise in Manual Testing, Functional Testing, Regression Testing, and Web Application Testing.  
### Task:  
Generate comprehensive manual test cases for the EventHub web application. Cover all major functionalities including User Registration, Login, Event Browsing, Event Search, Event Booking, Booking Cancellation, Session Management, Security Validation, and Logout.  
### Context:  
The application under test is:  
https://eventhub.rahulshettyacademy.com/  
EventHub is an event management platform where users can:  
Register a new account, 
Login using registered credentials,
Browse available events,
Search for events,
View event detail, 
Book events,
Manage bookings through the My Bookings section,
Cancel booked events,
Logout from the application.

The objective is to validate the complete end-to-end user journey and identify possible functional, validation and security-related issues.  
### Constraints:  
Include both Positive and Negative test scenarios.  
Include Validation and Error Handling scenarios.  
Include Session Management and Security-related scenarios.  
Consider real-world user behavior and edge cases.  
Avoid duplicate test cases.  
Write test cases in a clear step-by-step format.  
Ensure test cases are suitable for future automation.  
Cover mandatory field validations wherever applicable.  
Include business-critical scenarios such as duplicate booking prevention and unauthorized access checks.  
### Output Format:  
Generate test cases using the following format:  
TestCase_ID: TC_XXX - Test Scenario  
Test Steps:  
Step 1  
Step 2  
Step 3  

---

### TestCase_AI_001 – Register New User with Valid Data  
---
1. Open EventHub website.
1. Click Register.
1. Enter valid email and password.
1. Confirm password.
1. Click Create Account.
1. Verify registration is successful.

### TestCase_AI_002 – Register with Invalid Email
---
1. Open Registration page.
1. Enter invalid email format.
1. Enter valid password.
1. Submit form.
1. Verify validation message.
   
### TestCase_AI_003 – Register with Existing Email
---
1. Open Registration page.
1. Enter an already registered email.
1. Enter valid password.
1. Submit form.
1. Verify duplicate account error.
   
### TestCase_AI_004 – Register with Weak Password
---
1. Enter a weak password.
1. Submit registration.
1. Verify password policy message.
   
### TestCase_AI_005 – Register with Empty Fields
---
1. Leave all fields blank.
1. Submit registration form.
1. Verify mandatory field validations.
   
### TestCase_AI_006 – Register with Password Mismatch
---
1. Enter a different password and confirm the password.
1. Submit form.
1. Verify mismatch error.

### TestCase_AI_007 – Login with Valid Credentials
---
1. Enter valid email and password.
1. Click Login.
1. Verify successful login.

### TestCase_AI_008 – Login with Invalid Password
---
1. Enter valid email.
1. Enter incorrect password.
1. Click Login.
1. Verify error message.
   
### TestCase_AI_009 – Login with Invalid Email
---
1. Enter invalid email.
1. Enter password.
1. Click Login.
1. Verify login failure.
   
### TestCase_AI_010 – Login with Empty Credentials
---
1. Leave email and password blank.
1. Click Login.
1. Verify validation messages.
   
### TestCase_AI_011 – Verify Forgot Password Link
---
1. Open Login page.
1. Click Forgot Password.
1. Verify navigation to reset page.
   
### TestCase_AI_012 – Verify Session Persistence  
---
1. Login successfully.  
1. Refresh browser.  
1. Verify the user remains logged in.  

### TestCase_AI_013 – Access Protected Page Without Login 
---
1. Copy protected URL.  
1. Open in a new browser session.  
1. Verify redirect to Login page.  

### TestCase_AI_014 – Browse Available Events  
---
1. Login successfully.  
1. Click Browse Events.  
1. Verify event list appears.  

### TestCase_AI_015 – View Event Details  
---
1. Open an event.  
1. Verify event title, description, and date are displayed.  

### TestCase_AI_016 – Search Event by Valid Keyword  
---
1. Search using a valid event name.  
1. Verify matching results appear.  

### TestCase_AI_017 – Search Event by Invalid Keyword  
---
1. Search using random keywords.  
1. Verify no matching results.  

### TestCase_AI_018 – Search Event with Empty Input  
---
1. Leave the search box empty.  
1. Click Search.  
1. Verify all events are displayed.  

### TestCase_AI_019 – Book Event Successfully  
---
1. Select an event.  
1. Click Book Now.  
1. Enter valid booking details.  
1. Confirm booking.  
1. Verify booking success.  

### TestCase_AI_020 – Book Event with Empty Fields  
---
1. Open booking form.  
1. Leave mandatory fields blank.  
1. Submit booking.  
1. Verify validation messages.  

### TestCase_AI_021 – Book Event with Invalid Phone Number  
---
1. Enter invalid phone number.  
1. Submit booking.  
1. Verify validation message.  

### TestCase_AI_022 – Book Event with Invalid Email Address  
---
1. Enter invalid email.  
1. Submit booking.  
1. Verify validation message.  

### TestCase_AI_023 – Book Multiple Tickets  
---
1. Select event.  
1. Choose multiple tickets.  
1. Confirm booking.  
1. Verify successful booking.  

### TestCase_AI_024 – Verify Booking Appears in My Bookings  
---
1. Complete booking.  
1. Open My Bookings.  
1. Verify booking record exists.  

### TestCase_AI_025 – Verify Booking Details Accuracy  
---
1. Open My Bookings.  
1. Verify event name, date and ticket count are correct.  

### TestCase_AI_026 – Cancel Existing Booking  
---
1. Open My Bookings.  
1. Select booking.  
1. Click Cancel Booking.  
1. Verify successful cancellation.  

### TestCase_AI_027 – Verify Cancelled Booking Removal 
---
1. Cancel booking.  
1. Refresh page.  
1. Verify booking is removed.  

### TestCase_AI_028 – Cancel Booking Multiple Times  
---
1. Cancel booking.  
1. Attempt cancellation again.  
1. Verify appropriate error handling.  

### TestCase_AI_029 – Logout Functionality    
---
1. Click Logout.  
1. Verify the user is logged out.  
1. Verify Login page is displayed.  

### TestCase_AI_030 – Browser Back Button After Logout  
---
1. Logout successfully.  
1. Click the browser Back button.  
1. Verify protected pages are inaccessible.  
1. Verify Login page is displayed.  
---

# My thoughts  
## ● What I felt Suitable:-    
- AI generated a large number of test cases within seconds, significantly reducing test design effort.    
- AI covered all major modules including Registration, Login, Event Search, Event Booking, Booking Cancellation, Session Management, and Logout.   
- AI provided both positive and negative test scenarios.  
- AI helped identify commonly missed scenarios such as Forgot Password, Session Persistence, and Browser Back Button validation.  
- AI-generated test cases followed a structured and easy-to-understand format.  
- AI was useful for obtaining initial test coverage before starting detailed manual testing.  
- AI suggested validation-related scenarios that improved overall coverage.  
- AI can be a valuable productivity tool during test planning activities.  

## ● What I felt Not suitable:-    
- AI generated generic test cases and lacked understanding of actual business requirements.  
- Some scenarios were repetitive and overlapped with one another.  
- AI did not identify application-specific validations through exploration of the website.  
- AI missed important business-rule scenarios such as duplicate booking prevention and edge cases related to ticket limits.  
- Several test cases lacked detailed expected results, making them less suitable for direct automation.  
- AI did not prioritize test cases based on business impact or risk.  
- Boundary value analysis and exploratory testing scenarios were limited.  
- AI could not verify whether certain functionalities actually exist on the website before generating test cases.  
- Human review was still necessary to remove irrelevant scenarios and improve test quality.  
- AI-generated test cases alone were not sufficient to create an automation-ready test suite; manual refinement was required.  
---

# Final Test Cases (AI + Manual Combined) – Automation Ready  
## Member:- Tista Dutta.  
Application Under Test (AUT):  
https://eventhub.rahulshettyacademy.com/  
Application Name:  
EventHub  
Objective: To validate the end-to-end functionality of the EventHub application including user registration, authentication, event discovery, event booking, booking management, session handling, security validations, and logout functionality.  

Priority Definitions:  
P1 – Critical Business Functionality  
P2 – Important Functionality  
P3 – Nice-to-Have / Low Business Impact  

### TestCase_Final_001 – New User Registration with Valid Data 
---
Priority: P1  
1. Open EventHub website.  
1. Click on Register.  
1. Enter a valid email address.  
1. Enter a password satisfying all requirements.  
1. Enter the same password in the Confirm Password field.  
1. Click Create Account.  
1. Verify account creation is successful.  
1. Verify the user is redirected to the Login page.  
### Expected Result:  
The user account is created successfully and the Login page is displayed.  

### TestCase_Final_002 – Registration with Empty Fields  
---
Priority: P1  
1. Open EventHub website.  
1. Click Register.  
1. Leave all fields blank.  
1. Click Create Account.  
1. Verify validation messages are displayed.  
#### Expected Result:  
Mandatory field validation messages should appear for all required fields.  

### TestCase_Final_003 – Registration with Existing Email  
---
Priority: P1  
1. Open EventHub website.  
1. Click Register.  
1. Enter an already registered email address.  
1. Enter valid password.  
1. Click Create Account.  
#### Expected Result:  
An appropriate error message should indicate that the account already exists.  

### TestCase_Final_004 – Registration with Invalid Email Format  
---
Priority: P1  
1. Open EventHub website.  
1. Click Register.  
1. Enter invalid email format.  
1. Enter valid password.  
1. Confirm password.  
1. Click Create Account.  
#### Expected Result:  
Email format validation message should be displayed.  

### TestCase_Final_005 – Registration with Password Mismatch  
---
Priority: P1  
1. Open EventHub website.  
1. Click Register.  
1. Enter valid email.  
1. Enter password.  
1. Enter a different Confirm Password.  
1. Click Create Account.  
#### Expected Result:  
Password mismatch validation message should be displayed.  

### TestCase_Final_006 – Registration with Weak Password  
---
Priority: P2  
1. Open EventHub website.  
1. Click Register.  
1. Enter valid email.  
1. Enter a weak password.  
1. Click Create Account.  
#### Expected Result:  
Password policy validation should be displayed.  

### TestCase_Final_007 – Login with Valid Credentials  
---
Priority: P1  
1. Open EventHub website.  
1. Enter a registered email.  
1. Enter valid password.  
1. Click Sign In.  
#### Expected Result:  
Users should be logged in successfully and Dashboard should be displayed.  

### TestCase_Final_008 – Login with Invalid Password  
---
Priority: P1  
1. Open EventHub website.  
1. Enter valid email.  
1. Enter incorrect password.  
1. Click Sign In.  
#### Expected Result:  
Login failure message should be displayed.  

### TestCase_Final_009 – Login with Invalid Email  
---
Priority: P1  
1. Open EventHub website.   
1. Enter invalid email.  
1. Enter password.  
1. Click Sign In.  
#### Expected Result:  
Login should fail with an appropriate error message.  

### TestCase_Final_010 – Login with Empty Credentials  
---
Priority: P1  
1. Open EventHub website.  
1. Leave email and password blank.  
1. Click Sign In.  
#### Expected Result:  
Mandatory field validations should appear.  

### TestCase_Final_011 – Verify Forgot Password Navigation  
---
Priority: P3  
1. Open EventHub website.  
1. Open Login page.  
1. Click Forgot Password.  
#### Expected Result:  
Users should be redirected to the password recovery page.  

### TestCase_Final_012 – Verify Session Persistence After Refresh  
---
Priority: P2  
1. Open EventHub website.  
1. Enter a registered email.  
1. Enter valid password.  
1. Click Sign In.  
1. Refresh browser page.  
#### Expected Result:  
The user session should remain active.  

### TestCase_Final_013 – Access Protected Page Without Login  
---
Priority: P1  
1. Copy a protected URL.  
1. Open URL in a new browser session without login.  
#### Expected Result:  
Users should be redirected to the Login page.  

### TestCase_Final_014 – Browse Available Events  
---
Priority: P1  
1. Open EventHub website.  
1. Enter a registered email.  
1. Enter valid password.  
1. Click Sign In.  
1. Click Browse Events.  
#### Expected Result:  
Available events should be displayed successfully.  

### TestCase_Final_015 – View Event Details  
---
Priority: P2  
1. Open EventHub website.  
1. Enter a registered email.  
1. Enter valid password.  
1. Click Sign In.  
1. Open any available event.  
#### Expected Result:  
Event title, description, venue, and date should be displayed correctly.  

### TestCase_Final_016 – Search Event with Valid Keyword  
---
Priority: P2  
1. Open EventHub website.  
1. Enter a registered email.  
1. Enter valid password.  
1. Click Sign In.  
1. Navigate to Browse Events.  
1. Search using valid event keywords.  
#### Expected Result:  
Matching events should be displayed.  

### TestCase_Final_017 – Search Event with Invalid Keyword  
---
Priority: P2  
1. Open EventHub website.  
1. Enter a registered email.  
1. Enter valid password.  
1. Click Sign In.  
1. Navigate to Browse Events.  
1. Search using random keywords.  
#### Expected Result:  
"No Events Found" or equivalent message should be displayed.  

### TestCase_Final_018 – Search Event with Empty Search Input  
---
Priority: P3  
1. Open EventHub website.  
1. Enter a registered email.  
1. Enter valid password.  
1. Click Sign In.  
1. Navigate to Browse Events.  
1. Leave the search field blank.  
1. Click Search.  
#### Expected Result:  
All available events should be displayed.  

### TestCase_Final_019 – Book Event Successfully  
---
Priority: P1  
1. Open EventHub website.  
1. Enter a registered email.  
1. Enter valid password.  
1. Click Sign In.  
1. Click Browse Events.  
1. Select an event.  
1. Click Book Now.  
1. Enter Full Name, Email, Phone Number and Ticket Count.  
1. Click Confirm Booking.  
#### Expected Result:  
Booking should be completed successfully.  

### TestCase_Final_020 – Verify Booking Success Message  
---
Priority: P1  
1. Login with valid credentials.  
1. Click on the ‘Browse Events’ button.  
1. Select an available event.  
1. Click ‘Book Now’.  
1. Enter Full Name, Email, Phone Number and Select number of tickets.  
1. Click the button ‘Confirm booking’.  
1. Verify the success message.  
#### Expected Result:  
A success confirmation message should be displayed.  
 
### TestCase_Final_021 – Verify Booking Appears in My Bookings  
---
Priority: P1  
1. Login with valid credentials.  
1. Click on the ‘Browse Events’ button.  
1. Select an available event.  
1. Click ‘Book Now’.  
1. Enter Full Name, Email, Phone Number and Select number of tickets.  
1. Click the button ‘Confirm booking’.  
1. Verify the success message.  
1. Verify booking appears in the My Bookings section.  
#### Expected Result:  
Booked events should appear in My Bookings.  

### TestCase_Final_022 – Verify Booking Details Accuracy  
---
Priority: P1  
1. Login with valid credentials.  
1. Click on the ‘Browse Events’ button.  
1. Select an available event.  
1. Click ‘Book Now’.  
1. Enter Full Name, Email, Phone Number and Select number of tickets.  
1. Click the button ‘Confirm booking’.  
1. Verify the success message.  
1. Open My Bookings after booking.  
#### Expected Result:  
Event Name, Date, User Details and Ticket Count should match booking information.  

### TestCase_Final_023 – Booking with Empty Mandatory Fields  
---
Priority: P1  
1. Login with valid credentials.  
1. Click on the ‘Browse Events’ button.  
1. Select an available event.  
1. Click ‘Book Now’ to open the booking form.  
1. Leave mandatory fields blank.  
1. Click Confirm Booking.  
#### Expected Result:  
Validation messages should be displayed.  

### TestCase_Final_024 – Booking with Invalid Phone Number  
---
Priority: P1  
1. Login with valid credentials.   
1. Click on the ‘Browse Events’ button.  
1. Select an available event.  
1. Click ‘Book Now’ to open the booking form.  
1. Enter invalid phone number.  
1. Submit booking.  
#### Expected Result:  
Phone number validation message should be displayed.  

### TestCase_Final_025 – Booking with Invalid Email  
---
Priority: P1  
1. Login with valid credentials.  
1. Click on the ‘Browse Events’ button.  
1. Select an available event.  
1. Click ‘Book Now’ to open the booking form.  
1. Enter invalid email address.  
1. Submit booking.  
#### Expected Result:  
Email validation message should be displayed.  

### TestCase_Final_026 – Book Multiple Tickets  
---
Priority: P2   
1. Login with valid credentials.  
1. Click on the ‘Browse Events’ button.  
1. Select an available event.  
1. Click ‘Book Now’ to open the booking form.  
1. Choose multiple tickets.  
1. Complete booking.  
#### Expected Result:  
Booking should be completed successfully.  

### TestCase_Final_027 – Prevent Duplicate Booking  
---
Priority: P1  
1. Login with valid credentials.  
1. Click on the ‘Browse Events’ button.  
1. Select an available event.  
1. Click ‘Book Now’.  
1. Enter Full Name, Email, Phone Number and Select number of tickets.  
1. Click the button ‘Confirm booking’.  
1. Attempt to book the same event again.  
1. Verify duplicate booking is prevented.  
#### Expected Result:  
Duplicate booking should be prevented or appropriate warning displayed.  

### TestCase_Final_028 – Cancel Existing Booking  
---
Priority: P1  
1. Login with valid credentials.  
1. Navigate to My Bookings.  
1. Select booked event.  
1. Click Cancel Booking.  
1. Confirm cancellation.  
1. Verify booking is removed.  
1. Verify the success message.  
#### Expected Result:  
Booking should be cancelled successfully.  

### TestCase_Final_029 – Verify Cancelled Booking Removal  
---
Priority: P1  
1. Login with valid credentials.  
1. Navigate to My Bookings.  
1. Select booked event.  
1. Click Cancel Booking.  
1. Confirm cancellation to cancel a booking.  
1. Refresh My Bookings page.  
#### Expected Result:  
Cancelled booking should no longer appear in My Bookings.  

### TestCase_Final_030 – Attempt to Cancel Already Cancelled Booking  
---
Priority: P2  
1. Login with valid credentials.  
1. Navigate to My Bookings.  
1. Select booked event.  
1. Click Cancel Booking.  
1. Confirm cancellation to cancel booking.  
1. Attempt cancellation again.  
#### Expected Result:  
Proper error message or validation should be displayed.  

### TestCase_Final_031 – Logout Functionality  
---
Priority: P1  
1. Login with valid credentials.  
1. Click the Logout button on the EventHub menu.  
1. Verify the user is logged out.  
#### Expected Result:  
Users should be logged out successfully.  

### TestCase_Final_032 – Verify Login Page After Logout  
---
Priority: P1  
1. Login with valid credentials.  
1. Click the Logout button on the EventHub menu.  
1. Verify the user is logged out.  
1. Verify the login page is displayed.  
#### Expected Result:  
The login page should be displayed.  

### TestCase_Final_033 – Browser Back Button After Logout  
---
Priority: P1  
1. Login with valid credentials.  
1. Click the Logout button on the EventHub menu.  
1. Click the browser Back button.  
#### Expected Result:  
Protected pages should not be accessible.  

### TestCase_Final_034 – Direct URL Access After Logout  
---
Priority: P1  
1. Login with valid credentials.   
1. Click the Logout button on the EventHub menu.  
1. Open protected URL directly.  
#### Expected Result:  
Users should be redirected to the Login page.  

### TestCase_Final_035 – End-to-End User Journey  
---
Priority: P1  
1. Open EventHub website.  
1. Click on "Register".  
1. Enter a valid email address.  
1. Enter a password satisfying all requirements.  
1. Enter the same password in the Confirm Password field.  
1. Click Create Account.  
1. Login with registered credentials.  
1. Browse available events.  
1. Search for an event.  
1. Book an event.  
1. Verify booking in My Bookings.  
1. Cancel booking.  
1. Logout.  
#### Expected Result:
The entire user journey should complete successfully without any functional issues.

=====================================================================================


# skill.md

## Skill Name

EventHub Manual Test Case Generator

---

## Role

Act as a Senior QA Engineer with expertise in:

* Manual Testing
* Functional Testing
* Regression Testing
* Web Application Testing
* Validation Testing
* Security Testing
* Session Management Testing
* User Acceptance Testing

---

## Objective

Generate comprehensive manual test cases for the EventHub web application.

Application URL:
https://eventhub.rahulshettyacademy.com/

The objective is to validate the complete end-to-end user journey and identify:

* Functional defects
* Validation defects
* Business logic issues
* Security vulnerabilities
* Session management issues
* Data integrity issues
* Usability issues

---

## Application Features

The EventHub application allows users to:

1. Register a new account
2. Login using registered credentials
3. Browse available events
4. Search events
5. View event details
6. Book events
7. Manage bookings through My Bookings
8. Cancel booked events
9. Logout from application

---

## Assumptions

Unless explicitly specified otherwise, assume:

* Application is accessible and operational.
* User is testing on a supported browser.
* Stable internet connection is available.
* Latest application build is deployed.
* Test environment contains available events for booking.
* User has required permissions for intended actions.

---

## Business-Critical Rules

The following business rules must always be validated:

### Registration

* Duplicate email registration must not be allowed.
* User account must be created only with valid registration data.

### Authentication

* Only registered users can log in.
* Invalid credentials must not allow access.
* Authenticated sessions must be securely maintained.

### Event Booking

* Users must be logged in before booking an event.
* A user must not be able to create duplicate bookings for the same event.
* Booking confirmation must be displayed after successful booking.
* Booked events must appear in My Bookings.

### My Bookings

* Users must only see their own bookings.
* Users must not have access to other users' booking information.

### Booking Cancellation

* Users must only cancel their own bookings.
* Cancellation must update booking status correctly.
* Cancelled bookings must reflect appropriately in My Bookings.

### Session Management

* Logout must invalidate active sessions.
* Expired sessions must not allow access to protected pages.
* Browser back button must not expose authenticated pages after logout.

### Security

* Unauthorized users must not access protected pages.
* Direct URL access must respect authentication and authorization rules.
* Sensitive user information must not be exposed.
* User data must remain isolated from other users.

---

## Test Coverage Requirements

Generate test cases covering the following areas.

### 1. User Registration

Include:

* Successful registration
* Mandatory field validation
* Invalid email validation
* Password policy validation
* Confirm password mismatch
* Duplicate account registration
* Special character handling
* Boundary value testing
* SQL Injection validation
* XSS validation

---

### 2. Login

Include:

* Valid login
* Invalid credentials
* Blank fields
* Incorrect password
* Unregistered user login
* Password case sensitivity
* Session creation validation
* Multiple login attempts
* Security validations

---

### 3. Event Browsing

Include:

* View all available events
* Event card information validation
* Event list loading
* Pagination validation (if available)
* Event data consistency
* Empty event list handling

---

### 4. Event Search

Include:

* Search using full event name
* Search using partial event name
* Search using special characters
* Search using numbers
* Search with blank value
* Search with spaces
* No-result scenarios
* Case-insensitive search validation

---

### 5. Event Details

Include:

* Open event details page
* Validate event information
* Event date validation
* Event location validation
* Event capacity display validation
* Broken link validation

---

### 6. Event Booking

Include:

* Successful booking
* Booking confirmation validation
* Duplicate booking prevention
* Booking availability validation
* Multiple event booking
* Session timeout during booking
* Unauthorized booking attempts
* Network interruption scenarios

---

### 7. My Bookings

Include:

* View booked events
* Booking information validation
* Multiple booking visibility
* Booking persistence validation
* Booking history consistency

---

### 8. Booking Cancellation

Include:

* Successful cancellation
* Cancellation confirmation validation
* Repeated cancellation attempts
* Unauthorized cancellation attempts
* Cancellation reflection in My Bookings
* Event seat availability update validation

---

### 9. Session Management

Include:

* Session creation after login
* Session persistence after refresh
* Browser back button behavior
* Session expiration
* Idle timeout validation
* Multiple tab behavior
* Direct URL access validation
* Session invalidation after logout

---

### 10. Logout

Include:

* Successful logout
* Logout from multiple pages
* Session cleanup validation
* Browser cache validation
* Back button validation after logout

---

### 11. Security Testing

Include:

* Direct URL access without login
* Access control validation
* Session hijacking checks
* Authentication bypass attempts
* SQL Injection checks
* Cross-Site Scripting (XSS)
* Sensitive data exposure validation
* Cookie security validation
* Browser storage validation
* Forced browsing validation

---

### 12. Validation Testing

Include:

* Required field validation
* Input length validation
* Invalid data format validation
* Boundary value analysis
* Error message validation
* User-friendly validation messages

---

### 13. Error Handling

Include:

* Application error handling
* Invalid URL handling
* Network failure scenarios
* Unexpected input handling
* Server error handling
* Refresh during transaction

---

## Test Case Design Rules

### Positive Scenarios

Cover:

* Happy path workflows
* Valid user actions
* Successful transactions

### Negative Scenarios

Cover:

* Invalid inputs
* Unauthorized actions
* Business rule violations
* Incorrect user behavior

### Edge Cases

Cover:

* Maximum field lengths
* Minimum field lengths
* Empty values
* Special characters
* Duplicate requests
* Rapid repeated clicks
* Concurrent actions
* Browser refresh during transaction
* Multiple tab execution

---

## Additional Requirements

1. Avoid duplicate test cases.
2. Ensure each test case is atomic and independent.
3. Each test case must validate only one primary behavior.
4. Write reusable steps suitable for future automation.
5. Use clear and concise language.
6. Include business-critical scenarios.
7. Include validation and security checks.
8. Cover end-to-end workflows.
9. Cover regression-critical scenarios.
10. Cover data integrity validations.
11. Include both UI and backend validation checkpoints where applicable.
12. Prioritize high-risk business flows.
13. Consider real-world user behavior patterns.

---

## Priority Classification

Assign one of the following priorities:

* P1 = Critical
* P2 = High
* P3 = Medium
* P4 = Low

Critical flows include:

* Registration
* Login
* Event Booking
* Booking Cancellation
* Session Management
* Logout
* Access Control

---

## Severity Classification

Assign one of the following severities:

* Blocker
* Critical
* Major
* Minor
* Trivial

---

## Output Format

Generate test cases strictly using the following structure:

TestCase_ID: TC_001 - Test Scenario

Priority: P1

Severity: Critical

Preconditions:

* Required setup conditions

Test Data:

* Relevant test inputs

Test Steps:
Step 1:
Step 2:
Step 3:

Expected Result:

* Expected system behavior

Postconditions:

* Expected application state after execution

---

## Deliverable

Generate a complete manual test suite containing:

* Functional Test Cases
* Validation Test Cases
* Negative Test Cases
* Security Test Cases
* Session Management Test Cases
* Regression Test Cases

The resulting test suite should provide comprehensive coverage of the EventHub application user journey from registration through logout while ensuring security, usability, business logic, and data integrity validations are thoroughly covered.
