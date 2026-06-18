QA Manual Test Cases:-   

Member:- Tista Dutta.  
Query/Test cases:- Write test cases based on the given website  https://eventhub.rahulshettyacademy.com/   

Human Thinking Test Cases  

TestCase_001 – New User Registration with Valid Data  
Open EventHub website.  
Click on "Register".  
Enter a valid email address.  
Enter a password satisfying all requirements.  
Enter the same password in the Confirm Password field.  
Click Create Account.  
Verify that account is created successfully.  
Verify that the user is redirected to the login page.   

TestCase_002 – Registration with Empty Fields  
Open EventHub website.  
Click on Register.  
Leave all fields blank.  
Click Create Account.  
Verify mandatory field validation messages are displayed.  
TestCase_003 – Registration with Existing Email.  
Open EventHub website.  
Click Register.  
Enter an email already registered.  
Enter valid password.  
Click Create Account.  
Verify appropriate error messages are displayed.  


TestCase_004 – Registration with Invalid Email   
Open EventHub website.  
Click on "Register".  
Enter invalid email format.  
Enter valid password.  
Enter confirm password.  
Click Create Account.  
Verify validation message is displayed.  

TestCase_005 – Registration with Password Mismatch  
Open EventHub website.  
Enter valid email.  
Enter password.  
Enter a different confirm password.  
Click Create Account.  
Verify password mismatch message.  

TestCase_006 – Login with Valid Credentials  
Open EventHub website.  
Enter a registered email.  
Enter valid password.  
Click Sign In.  
Verify successful login.  
Verify the dashboard is displayed.  
TestCase_007 – Login with Invalid Password  
Open EventHub website.  
Enter a registered email.  
Enter the wrong password.  
Click Sign In.  
Verify error message.  

TestCase_008 – Session Persistence after Refresh  
Login with valid credentials.  
Refresh browser.  
Verify the user remains logged in. 

TestCase_009 – Access Protected Page Without Login  
Copy a protected URL.  
Open it in a new browser without login.  
Verify the user is redirected to the Login page.  

TestCase_010 – Browse Available Events  
Login with valid credentials.  
Click Browse Events.
Verify the event list is displayed.

TestCase_011 – Search Event  
Login with valid credentials.
Navigate to Browse Events.
Search event by keyword.
Verify relevant events appear.

TestCase_012 – Search Non-Existing Event  
Login with valid credentials.
Navigate to Browse Events.
Search with invalid keywords.
Verify "No events found" message.


TestCase_013 – Event Booking
Login with valid credentials.
Click on the ‘Browse Events’ button.
Select an available event.
Click ‘Book Now’.
Enter Full Name, Email, Phone Number and Select number of tickets.
Click the button ‘Confirm booking’.
Verify the success message.
Verify booking appears in the My Bookings section.
TestCase_014 – Duplicate Event Booking
Login with valid credentials.
Click on the ‘Browse Events’ button.
Select an available event.
Click ‘Book Now’.
Enter Full Name, Email, Phone Number and Select number of tickets.
Click the button ‘Confirm booking’.
Attempt to book the same event again.
Verify duplicate booking is prevented.
TestCase_015 – Booking with Invalid Phone Number
Login with valid credentials.
Click on the ‘Browse Events’ button.
Select an available event.
Click ‘Book Now’.
Enter invalid phone number.
Submit booking.
Verify validation message.

TestCase_016 – Cancel Event Booking
Login with valid credentials.
Navigate to My Bookings.
Select booked event.
Click Cancel Booking.
Confirm cancellation.
Verify booking is removed.
Verify the success message.
TestCase_017 – Logout
Login with valid credentials.
Click the Logout button on the EventHub menu.
Verify the user is logged out.
Verify the login page is displayed.

AI Manual Test Cases:- 
Member:- Tista Dutta.
Prompt:-
Role:
Act as a Senior QA Engineer with expertise in Manual Testing, Functional Testing, Regression Testing, and Web Application Testing.
Task:
Generate comprehensive manual test cases for the EventHub web application. Cover all major functionalities including User Registration, Login, Event Browsing, Event Search, Event Booking, Booking Cancellation, Session Management, Security Validation, and Logout.
Context:
The application under test is:
https://eventhub.rahulshettyacademy.com/
EventHub is an event management platform where users can:
Register a new account
Login using registered credentials
Browse available events
Search for events
View event details
Book events
Manage bookings through the My Bookings section
Cancel booked events
Logout from the application
The objective is to validate the complete end-to-end user journey and identify possible functional, validation and security-related issues.
Constraints:
Include both Positive and Negative test scenarios.
Include Validation and Error Handling scenarios.
Include Session Management and Security-related scenarios.
Consider real-world user behavior and edge cases.
Avoid duplicate test cases.
Write test cases in a clear step-by-step format.
Ensure test cases are suitable for future automation.
Cover mandatory field validations wherever applicable.
Include business-critical scenarios such as duplicate booking prevention and unauthorized access checks.
Output Format:
Generate test cases using the following format:
TestCase_ID: TC_XXX - Test Scenario
Test Steps:
Step 1
Step 2
Step 3


TestCase_AI_001 – Register New User with Valid Data
Open EventHub website.
Click Register.
Enter valid email and password.
Confirm password.
Click Create Account.
Verify registration is successful.
TestCase_AI_002 – Register with Invalid Email
Open Registration page.
Enter invalid email format.
Enter valid password.
Submit form.
Verify validation message.
TestCase_AI_003 – Register with Existing Email
Open Registration page.
Enter an already registered email.
Enter valid password.
Submit form.
Verify duplicate account error.
TestCase_AI_004 – Register with Weak Password
Enter a weak password.
Submit registration.
Verify password policy message.
TestCase_AI_005 – Register with Empty Fields
Leave all fields blank.
Submit registration form.
Verify mandatory field validations.
TestCase_AI_006 – Register with Password Mismatch
Enter a different password and confirm the password.
Submit form.
Verify mismatch error.
TestCase_AI_007 – Login with Valid Credentials
Enter valid email and password.
Click Login.
Verify successful login.
TestCase_AI_008 – Login with Invalid Password
Enter valid email.
Enter incorrect password.
Click Login.
Verify error message.
TestCase_AI_009 – Login with Invalid Email
Enter invalid email.
Enter password.
Click Login.
Verify login failure.
TestCase_AI_010 – Login with Empty Credentials
Leave email and password blank.
Click Login.
Verify validation messages.
TestCase_AI_011 – Verify Forgot Password Link
Open Login page.
Click Forgot Password.
Verify navigation to reset page.
TestCase_AI_012 – Verify Session Persistence
Login successfully.
Refresh browser.
Verify the user remains logged in.
TestCase_AI_013 – Access Protected Page Without Login
Copy protected URL.
Open in a new browser session.
Verify redirect to Login page.
TestCase_AI_014 – Browse Available Events
Login successfully.
Click Browse Events.
Verify event list appears.
TestCase_AI_015 – View Event Details
Open an event.
Verify event title, description, and date are displayed.
TestCase_AI_016 – Search Event by Valid Keyword
Search using a valid event name.
Verify matching results appear.
TestCase_AI_017 – Search Event by Invalid Keyword
Search using random keywords.
Verify no matching results.
TestCase_AI_018 – Search Event with Empty Input
Leave the search box empty.
Click Search.
Verify all events are displayed.
TestCase_AI_019 – Book Event Successfully
Select an event.
Click Book Now.
Enter valid booking details.
Confirm booking.
Verify booking success.
TestCase_AI_020 – Book Event with Empty Fields
Open booking form.
Leave mandatory fields blank.
Submit booking.
Verify validation messages.
TestCase_AI_021 – Book Event with Invalid Phone Number
Enter invalid phone number.
Submit booking.
Verify validation message.
TestCase_AI_022 – Book Event with Invalid Email Address
Enter invalid email.
Submit booking.
Verify validation message.
TestCase_AI_023 – Book Multiple Tickets
Select event.
Choose multiple tickets.
Confirm booking.
Verify successful booking.
TestCase_AI_024 – Verify Booking Appears in My Bookings
Complete booking.
Open My Bookings.
Verify booking record exists.
TestCase_AI_025 – Verify Booking Details Accuracy
Open My Bookings.
Verify event name, date and ticket count are correct.
TestCase_AI_026 – Cancel Existing Booking
Open My Bookings.
Select booking.
Click Cancel Booking.
Verify successful cancellation.
TestCase_AI_027 – Verify Cancelled Booking Removal
Cancel booking.
Refresh page.
Verify booking is removed.
TestCase_AI_028 – Cancel Booking Multiple Times
Cancel booking.
Attempt cancellation again.
Verify appropriate error handling.
TestCase_AI_029 – Logout Functionality
Click Logout.
Verify the user is logged out.
Verify Login page is displayed.
TestCase_AI_030 – Browser Back Button After Logout
Logout successfully.
Click the browser Back button.
Verify protected pages are inaccessible.
Verify Login page is displayed.
My thoughts:-
 ● What I felt Suitable:-
AI generated a large number of test cases within seconds, significantly reducing test design effort.
AI covered all major modules including Registration, Login, Event Search, Event Booking, Booking Cancellation, Session Management, and Logout.
AI provided both positive and negative test scenarios.
AI helped identify commonly missed scenarios such as Forgot Password, Session Persistence, and Browser Back Button validation.
AI-generated test cases followed a structured and easy-to-understand format.
AI was useful for obtaining initial test coverage before starting detailed manual testing.
AI suggested validation-related scenarios that improved overall coverage.
AI can be a valuable productivity tool during test planning activities.

 ● What I felt Not suitable:- 
AI generated generic test cases and lacked understanding of actual business requirements.
Some scenarios were repetitive and overlapped with one another.
AI did not identify application-specific validations through exploration of the website.
AI missed important business-rule scenarios such as duplicate booking prevention and edge cases related to ticket limits.
Several test cases lacked detailed expected results, making them less suitable for direct automation.
AI did not prioritize test cases based on business impact or risk.
Boundary value analysis and exploratory testing scenarios were limited.
AI could not verify whether certain functionalities actually exist on the website before generating test cases.
Human review was still necessary to remove irrelevant scenarios and improve test quality.
AI-generated test cases alone were not sufficient to create an automation-ready test suite; manual refinement was required.

Final Test Cases (AI + Manual Combined) – Automation Ready
Member:- Tista Dutta.
Application Under Test (AUT):
https://eventhub.rahulshettyacademy.com/
Application Name:
EventHub
Objective: To validate the end-to-end functionality of the EventHub application including user registration, authentication, event discovery, event booking, booking management, session handling, security validations, and logout functionality.

Priority Definitions:
P1 – Critical Business Functionality
P2 – Important Functionality
P3 – Nice-to-Have / Low Business Impact

TestCase_Final_001 – New User Registration with Valid Data
Priority: P1
Open EventHub website.
Click on Register.
Enter a valid email address.
Enter a password satisfying all requirements.
Enter the same password in the Confirm Password field.
Click Create Account.
Verify account creation is successful.
Verify the user is redirected to the Login page.
Expected Result:
The user account is created successfully and the Login page is displayed.

TestCase_Final_002 – Registration with Empty Fields
Priority: P1
Open EventHub website.
Click Register.
Leave all fields blank.
Click Create Account.
Verify validation messages are displayed.
Expected Result:
Mandatory field validation messages should appear for all required fields.

TestCase_Final_003 – Registration with Existing Email
Priority: P1
Open EventHub website.
Click Register.
Enter an already registered email address.
Enter valid password.
Click Create Account.
Expected Result:
An appropriate error message should indicate that the account already exists.

TestCase_Final_004 – Registration with Invalid Email Format
Priority: P1
Open EventHub website.
Click Register.
Enter invalid email format.
Enter valid password.
Confirm password.
Click Create Account.
Expected Result:
Email format validation message should be displayed.

TestCase_Final_005 – Registration with Password Mismatch
Priority: P1
Open EventHub website.
Click Register.
Enter valid email.
Enter password.
Enter a different Confirm Password.
Click Create Account.
Expected Result:
Password mismatch validation message should be displayed.

TestCase_Final_006 – Registration with Weak Password
Priority: P2
Open EventHub website.
Click Register.
Enter valid email.
Enter a weak password.
Click Create Account.
Expected Result:
Password policy validation should be displayed.

TestCase_Final_007 – Login with Valid Credentials
Priority: P1
Open EventHub website.
Enter a registered email.
Enter valid password.
Click Sign In.
Expected Result:
Users should be logged in successfully and Dashboard should be displayed.

TestCase_Final_008 – Login with Invalid Password
Priority: P1
Open EventHub website.
Enter valid email.
Enter incorrect password.
Click Sign In.
Expected Result:
Login failure message should be displayed.

TestCase_Final_009 – Login with Invalid Email
Priority: P1
Open EventHub website.
Enter invalid email.
Enter password.
Click Sign In.
Expected Result:
Login should fail with an appropriate error message.

TestCase_Final_010 – Login with Empty Credentials
Priority: P1
Open EventHub website.
Leave email and password blank.
Click Sign In.
Expected Result:
Mandatory field validations should appear.

TestCase_Final_011 – Verify Forgot Password Navigation
Priority: P3
Open EventHub website.
Open Login page.
Click Forgot Password.
Expected Result:
Users should be redirected to the password recovery page.

TestCase_Final_012 – Verify Session Persistence After Refresh
Priority: P2
Open EventHub website.
Enter a registered email.
Enter valid password.
Click Sign In.
Refresh browser page.
Expected Result:
The user session should remain active.

TestCase_Final_013 – Access Protected Page Without Login
Priority: P1
Copy a protected URL.
Open URL in a new browser session without login.
Expected Result:
Users should be redirected to the Login page.

TestCase_Final_014 – Browse Available Events
Priority: P1
Open EventHub website.
Enter a registered email.
Enter valid password.
Click Sign In.
Click Browse Events.
Expected Result:
Available events should be displayed successfully.

TestCase_Final_015 – View Event Details
Priority: P2
Open EventHub website.
Enter a registered email.
Enter valid password.
Click Sign In.
Open any available event.
Expected Result:
Event title, description, venue, and date should be displayed correctly.

TestCase_Final_016 – Search Event with Valid Keyword
Priority: P2
Open EventHub website.
Enter a registered email.
Enter valid password.
Click Sign In.
Navigate to Browse Events.
Search using valid event keywords.
Expected Result:
Matching events should be displayed.

TestCase_Final_017 – Search Event with Invalid Keyword
Priority: P2
Open EventHub website.
Enter a registered email.
Enter valid password.
Click Sign In.
Navigate to Browse Events.
Search using random keywords.
Expected Result:
"No Events Found" or equivalent message should be displayed.

TestCase_Final_018 – Search Event with Empty Search Input
Priority: P3
Open EventHub website.
Enter a registered email.
Enter valid password.
Click Sign In.
Navigate to Browse Events.
Leave the search field blank.
Click Search.
Expected Result:
All available events should be displayed.

TestCase_Final_019 – Book Event Successfully
Priority: P1
Open EventHub website.
Enter a registered email.
Enter valid password.
Click Sign In.
Click Browse Events.
Select an event.
Click Book Now.
Enter Full Name, Email, Phone Number and Ticket Count.
Click Confirm Booking.
Expected Result:
Booking should be completed successfully.

TestCase_Final_020 – Verify Booking Success Message
Priority: P1
Login with valid credentials.
Click on the ‘Browse Events’ button.
Select an available event.
Click ‘Book Now’.
Enter Full Name, Email, Phone Number and Select number of tickets.
Click the button ‘Confirm booking’.
Verify the success message.
Expected Result:
A success confirmation message should be displayed.

TestCase_Final_021 – Verify Booking Appears in My Bookings
Priority: P1
Login with valid credentials.
Click on the ‘Browse Events’ button.
Select an available event.
Click ‘Book Now’.
Enter Full Name, Email, Phone Number and Select number of tickets.
Click the button ‘Confirm booking’.
Verify the success message.
Verify booking appears in the My Bookings section.
Expected Result:
Booked events should appear in My Bookings.

TestCase_Final_022 – Verify Booking Details Accuracy
Priority: P1
Login with valid credentials.
Click on the ‘Browse Events’ button.
Select an available event.
Click ‘Book Now’.
Enter Full Name, Email, Phone Number and Select number of tickets.
Click the button ‘Confirm booking’.
Verify the success message.
Open My Bookings after booking.
Expected Result:
Event Name, Date, User Details and Ticket Count should match booking information.

TestCase_Final_023 – Booking with Empty Mandatory Fields
Priority: P1
Login with valid credentials.
Click on the ‘Browse Events’ button.
Select an available event.
Click ‘Book Now’ to open the booking form.
Leave mandatory fields blank.
Click Confirm Booking.
Expected Result:
Validation messages should be displayed.

TestCase_Final_024 – Booking with Invalid Phone Number
Priority: P1
Login with valid credentials.
Click on the ‘Browse Events’ button.
Select an available event.
Click ‘Book Now’ to open the booking form.
Enter invalid phone number.
Submit booking.
Expected Result:
Phone number validation message should be displayed.

TestCase_Final_025 – Booking with Invalid Email
Priority: P1
Login with valid credentials.
Click on the ‘Browse Events’ button.
Select an available event.
Click ‘Book Now’ to open the booking form.
Enter invalid email address.
Submit booking.
Expected Result:
Email validation message should be displayed.

TestCase_Final_026 – Book Multiple Tickets
Priority: P2
Login with valid credentials.
Click on the ‘Browse Events’ button.
Select an available event.
Click ‘Book Now’ to open the booking form.
Choose multiple tickets.
Complete booking.
Expected Result:
Booking should be completed successfully.

TestCase_Final_027 – Prevent Duplicate Booking
Priority: P1
Login with valid credentials.
Click on the ‘Browse Events’ button.
Select an available event.
Click ‘Book Now’.
Enter Full Name, Email, Phone Number and Select number of tickets.
Click the button ‘Confirm booking’.
Attempt to book the same event again.
Verify duplicate booking is prevented.
Expected Result:
Duplicate booking should be prevented or appropriate warning displayed.

TestCase_Final_028 – Cancel Existing Booking
Priority: P1
Login with valid credentials.
Navigate to My Bookings.
Select booked event.
Click Cancel Booking.
Confirm cancellation.
Verify booking is removed.
Verify the success message.
Expected Result:
Booking should be cancelled successfully.

TestCase_Final_029 – Verify Cancelled Booking Removal
Priority: P1
Login with valid credentials.
Navigate to My Bookings.
Select booked event.
Click Cancel Booking.
Confirm cancellation to cancel a booking.
Refresh My Bookings page.
Expected Result:
Cancelled booking should no longer appear in My Bookings.

TestCase_Final_030 – Attempt to Cancel Already Cancelled Booking
Priority: P2
Login with valid credentials.
Navigate to My Bookings.
Select booked event.
Click Cancel Booking.
Confirm cancellation to cancel booking.
Attempt cancellation again.
Expected Result:
Proper error message or validation should be displayed.

TestCase_Final_031 – Logout Functionality
Priority: P1
Login with valid credentials.
Click the Logout button on the EventHub menu.
Verify the user is logged out.
Expected Result:
Users should be logged out successfully.

TestCase_Final_032 – Verify Login Page After Logout
Priority: P1
Login with valid credentials.
Click the Logout button on the EventHub menu.
Verify the user is logged out.
Verify the login page is displayed.
Expected Result:
The login page should be displayed.

TestCase_Final_033 – Browser Back Button After Logout
Priority: P1
Login with valid credentials.
Click the Logout button on the EventHub menu.
Click the browser Back button.
Expected Result:
Protected pages should not be accessible.

TestCase_Final_034 – Direct URL Access After Logout
Priority: P1
Login with valid credentials.
Click the Logout button on the EventHub menu.
Open protected URL directly.
Expected Result:
Users should be redirected to the Login page.

TestCase_Final_035 – End-to-End User Journey
Priority: P1
Open EventHub website.
Click on "Register".
Enter a valid email address.
Enter a password satisfying all requirements.
Enter the same password in the Confirm Password field.
Click Create Account.
Login with registered credentials.
Browse available events.
Search for an event.
Book an event.
Verify booking in My Bookings.
Cancel booking.
Logout.
Expected Result:
The entire user journey should complete successfully without any functional issues.
