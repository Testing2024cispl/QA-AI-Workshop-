Table of Contents
##QA Manual Test Cases
##Human Thinking Test Cases
##AI Manual Test Cases
##Prompt
##My Thoughts
##Final Test Cases (AI + Manual Combined) – Automation Ready
-------------------------------------------------
QA Manual Test Cases:- 
-------------------------------------------------
Member 1:- Susanta Das 

Site URL :- https://eventhub.rahulshettyacademy.com/  

Query/Test cases :- 
Scenario 2 : Old user login , event booking, booking cancel , logout 
----------

Human Thinking Test Cases 
------------------------------------------
TestCases_001:-  Old Existing user login with invalid email or password
---
Go to eventhub.rahulshettyacademy.com 
Click on Sign in CTA using invalid email address or password 
Users will get an error message "Invalid email or password” within a modal.

TestCases_002:- Old Existing user login with valid email and password
---
Go to eventhub.rahulshettyacademy.com 
Click on Sign in CTA using existing valid email address and password 
Users will be logged into the homepage of the site.

TestCases_003:- Old Existing user login & event booking functionality.
---
 Go to eventhub.rahulshettyacademy.com
Click on Sign in CTA using existing valid email address and password 
Users will be logged into the homepage of the site.
Click on “Browse Event” CTA.
Users will be redirected to the Events section of the site.
Users can search for any event after applying category or city filters or Users can directly search with any event name.
Click the "Book Now" CTA on the selected event. 
Verify that the user is redirected to that event's detail page, where the event history is visible. 
On the event page, increase the ticket quantity using the "+" icon to book for multiple attendees. Verify that the ticket count cannot exceed a maximum of “10”. 
 Fill in the required attendee details (name, email address, and contact number), then click "Confirm Booking." 
Verify that an error message is displayed like the sample error message  "Only 8 seat(s) available, but 10 requested" . Reduce the ticket count to a value less than the actual available seats. 
 Verify that a "Booking Confirmed" message is displayed on the event page with available ticket counts. 
Users can observe the booking reference number , ticket counts, price and customer name.
Users can click on “View My bookings” or “Browse more events” CTA.
If the user clicks on “Browse more events” CTA then the user will be redirected to the “Events” page and users can book other events also in the same way by following the above steps .
If the user clicks on “ View My Bookings" CTA then  the user will be redirected to the “My Bookings” page .

TestCases_004:- Old Existing user login & booking event cancel and logout functionality.
---
Go to eventhub.rahulshettyacademy.com
Click on Sign in CTA using existing valid email address and password 
Users will be logged into the homepage of the site.
Click on “My Bookings” CTA.
Users will be redirected to the “My Bookings” page or section of the site. 
In the “My Bookings” page if a user clicks on “View Details” CTA then the user will observe the booking details of that particular event .
If the user clicks on “Check eligibility for refund?” option under the “Refund” section on the “Event Details” page then the message will be displayed as “Eligible for refund. Single-ticket bookings qualify for a full refund.”
 users can click on “Cancel Booking” CTA also to cancel the event booking.
Users can also scroll down to the bottom of the page and click on “Back to My Bookings” CTA and  then the user will be redirected back to the previous section or User can click on "Cancel Booking” CTA also to cancel the event booking.
 After clicking on “Back to My Bookings” CTA when the user will be redirected back to the previous section then the user can click on “Cancel Booking” CTA also to cancel the event booking.
 Users need to click on “Yes, cancel it” CTA within the pop-up modal to cancel the event and will get a cancellation message “Booking Cancelled successfully”  within the pop-up window
 Users can click on “cancel” CTA within the pop-up modal to cancel this booking cancellation process.
 Users can click on “Clear all bookings”CTA to cancel all existing bookings and click on “Ok” buttons within the alert pop-up window. All existing bookings will be cleared from the “My Bookings” page.

TestCases_005:- Old Existing user login & view booking event status in events page and logout functionality.
---
Go to eventhub.rahulshettyacademy.com
Click on Sign in CTA using existing valid email address and password 
Users will be logged into the homepage of the site.
Click on “My Bookings” CTA.
Users will be redirected to the “My Bookings” page or section of the site and check the status of booking events.
The user clicks on “Logout” CTA at the top-right corner of the page and will be redirected to the login page . The user will validate that a validation message “logout successfully done” is displayed within a pop-up window or not. 

TestCases_006:- Old Existing user login & perform booking the event with invalid credentials in full name, phone number , email address input fields.
---
Go to eventhub.rahulshettyacademy.com
Click on Sign in CTA using existing valid email address and password 
Users will be logged into the homepage of the site.
Click the "Book Now" CTA on any events from the home page . 
Users can fill numbers in the full name input field and click on “Confirm Booking” CTA and can observe whether the validation message appears or not. 
Users can fill invalid email addresses like “test7@gmail.comefsefgdfdfgfrrrrr34231312”  in the full name input field and click on “Confirm Booking” CTA and can observe whether the validation message appears or not. 
Users can fill invalid phone numbers in the phone number input field and click on “Confirm Booking” CTA and can observe whether the validation message appears or not. 
Users can directly click on  “Confirm Booking” CTA without filling any values in all input fields and validate whether the error validation  message appears on the bottom of all input fields or not. 

-------------------------------------------------------------------
AI Manual Test Cases:- 
-------------------------------------------------------------------
Member 1:- Susanta Das
Prompt :- 
-----
Write test cases for https://eventhub.rahulshettyacademy.com/ site with existing valid email "susantadas7044554389@gmail.com" and password "Test@1234" to validate the scenario Old existing user login , event booking, booking cancel and logout . 
Sample Format: TestCases_001: Old Existing User Login with Invalid Email or Password Precondition: User accounts already exist in the system. Test Steps:
Navigate to https://eventhub.rahulshettyacademy.com
Click on the Login button. Enter an invalid email address.
Enter an invalid password. Click on the Login button.
User should not be logged in.
Appropriate error message should be displayed.
User should remain on the Login page.
don't make test cases steps based on only sample format  . make the test cases based on "Write test cases for https://eventhub.rahulshettyacademy.com/ site with existing valid email "susantadas7044554389@gmail.com" and password "Test@1234" to validate the scenario Old existing user login , event booking, booking cancel and logout ."

----------------------------------------
Test Cases for Old Existing User Login, Event Booking, Booking Cancellation, and Logout
----------------------------------------
TestCases_001: Verify Login with Valid Existing User Credentials
---
Precondition: Existing user account is registered with email susantadas7044554389@gmail.com and password Test@1234.
Test Steps:
Navigate to https://eventhub.rahulshettyacademy.com.
Click on the Login button.
Enter email: susantadas7044554389@gmail.com.
Enter password: Test@1234.
Click on the Login button.
Expected Result:
User should be successfully authenticated.
User should be redirected to the dashboard/home page.
User profile/account icon should be displayed.
No validation or error message should appear.

TestCases_002: Verify Login Page UI Elements
---
Precondition: User is on the Login page.
Test Steps:
Navigate to the Login page.
Verify Email field.
Verify Password field.
Verify Login button.
Verify Forgot Password link (if available).
Verify Sign Up/Register option.
Expected Result:
All UI elements should be displayed properly.
Fields and buttons should be aligned correctly.
Login button should be enabled after entering valid credentials.

TestCases_003: Verify Password Field Masking
---
Precondition: User is on Login page.
Test Steps:
Navigate to Login page.
Enter password Test@1234.
Expected Result:
Password characters should be masked.
Actual password should not be visible.

TestCases_004: Verify Successful Login Session Persistence
---
Precondition: User account exists.
Test Steps:
Login using valid credentials.
Refresh the browser page.
Navigate across different pages.
Expected Result:
Users should remain logged in.
The session should remain active.
Users should not be redirected to the Login page.

----------------------------------
Event Booking Test Cases
----------------------------------
TestCases_005: Verify Event Listing Display After Login
---
Precondition: User is logged in.
Test Steps:
Login with valid credentials.
Navigate to the Events page.
Expected Result:
Available events should be displayed.
Event details should be visible including event name, date, venue, and booking option.

TestCases_006: Verify Event Details Page Navigation
---
Precondition: User is logged in.
Test Steps:
Login successfully.
Select any available event.
Click on the event card/title.
Expected Result:
Users should be redirected to the event details page.
Event information should be displayed correctly.

TestCases_007: Verify Successful Event Booking
---
Precondition: User is logged in and event seats are available.
Test Steps:
Login with valid credentials.
Open an available event.
Click the Book Event/Register button.
Complete any required booking information.
Submit booking.
Expected Result:
Booking should be completed successfully.
A success confirmation message should be displayed.
Events should appear under the My Bookings/My Events section.

TestCases_008: Verify Booking Confirmation Visibility
---
Precondition: Event booking completed successfully.
Test Steps:
Login to application.
Navigate to My Bookings/My Events section.
Expected Result:
Newly booked events should be displayed.
Event details should match selected events.
Booking status should show Confirmed/Booked.

TestCases_009: Verify Multiple Event Booking
---
Precondition: User is logged in and multiple events are available.
Test Steps:
Login with valid credentials.
Book Event A.
Book Event B.
Navigate to My Bookings section.
Expected Result:
Both events should appear in booking history.
Booking details should be displayed correctly.

TestCases_010: Verify Duplicate Event Booking Behavior
---
Precondition: User already booked an event.
Test Steps:
Login with valid credentials.
Open an already booked event.
Attempt to book the same event again.
Expected Result:
The system should follow business rules.
Either duplicate booking should be prevented with an appropriate message or multiple bookings should be handled correctly.

TestCases_011: Verify Booking Persistence After Browser Refresh
---
Precondition: Event successfully booked.
Test Steps:
Complete event booking.
Refresh browser.
Navigate to My Bookings.
Expected Result:
Booking should remain intact.
Booking information should not be lost.

------------------------------------
Booking Cancellation Test Cases
------------------------------------
TestCases_012: Verify Availability of Cancel Booking Option
---
Precondition: User has at least one booked event.
Test Steps:
Login with valid credentials.
Navigate to My Bookings section.
Open booked event.
Expected Result:
Cancel Booking option should be available (if cancellation is permitted).

TestCases_013: Verify Successful Event Booking Cancellation
---
Precondition: User has a confirmed event booking.
Test Steps:
Login successfully.
Navigate to My Bookings.
Select booked event.
Click Cancel Booking.
Confirm cancellation.
Expected Result:
Booking should be cancelled successfully.
A confirmation message should be displayed.
Events should be removed from active bookings or marked as Cancelled.

TestCases_014: Verify Booking Status After Cancellation
---
Precondition: Event booking has been cancelled.
Test Steps:
Login with valid credentials.
Navigate to My Bookings.
Expected Result:
Cancelled booking should display correct status.
Users should not be considered an active attendee.

TestCases_015: Verify Rebooking After Cancellation
---
Precondition: Event booking was cancelled.
Test Steps:
Login successfully.
Navigate to a cancelled event.
Attempt to book an event again.
Expected Result:
Users should be able to rebook the event if seats are available.
New booking confirmation should be generated.

TestCases_016: Verify Cancellation Persistence After Refresh
---
Precondition: Event booking has been cancelled.
Test Steps:
Cancel event booking.
Refresh browser.
Navigate to My Bookings.
Expected Result:
Cancelled status should remain unchanged.
Booking should not reappear as active.

------------------------------------
Logout Test Cases
------------------------------------
TestCases_017: Verify Successful Logout
---
Precondition: User is logged in.
Test Steps:
Login successfully.
Click on Profile/Account menu.
Click Logout.
Expected Result:
Users should be logged out successfully.
Users should be redirected to the Login/Home page.
The session should be terminated.

TestCases_018: Verify Restricted Page Access After Logout
---
Precondition: User has logged out.
Test Steps:
Logout from application.
Press the browser Back button.
Attempt to access My Bookings URL directly.
Expected Result:
Users should not access authenticated pages.
Users should be redirected to the Login page.

TestCases_019: Verify Session Expiry After Logout
---
Precondition: User logged out.
Test Steps:
Logout from application.
Refresh browser multiple times.
Expected Result:
User sessions should remain terminated.
Users should not be automatically logged back in.

TestCases_020: End-to-End Flow Validation (Login → Book Event → Cancel Booking → Logout)
---
Precondition: Existing user account is available.
Test Steps:
Navigate to the EventHub website.
Login using:
Email: susantadas7044554389@gmail.com
Password: Test@1234
Open an available event.
Book the event.
Verify booking appears in My Bookings.
Cancel the booked event.
Verify booking status changes to Cancelled.
Logout from the application.
Expected Result:
Login should be successful.
Event booking should be completed successfully.
Booking should appear in booking history.
Booking cancellation should succeed.
Cancelled status should be reflected correctly.
Logout should terminate the session successfully.
Users should be redirected to the public/home page after logout.

---------------------------
My  thoughts:- 
---------------------------
● What I  felt Suitable:-  
    The test cases cover the complete end-to-end user journey, including login, event booking, booking cancellation, booking status verification, and logout. Both positive and negative login scenarios are included. Test steps are written in a logical sequence that closely follows actual user behavior. Important system messages such as booking confirmation, cancellation success, and login validation are verified. 

● What I  felt Not suitable:- 
    Boundary value validations (minimum and maximum character limits, special characters, blank spaces, etc.) are not covered for booking form fields. Session validation after logout (e.g., using browser Back button or direct URL access) is not covered. Test cases are not currently automation-ready because reusable preconditions, test data, and clear assertions are not defined separately. 

------------------------
Final Test Cases (AI + Manual Combined) – Automation Ready
------------------------

# EventHub Test Coverage Matrix

## Login Module

| Test Case ID | Scenario                         | Priority | Automation Ready | Smoke | Regression |
| ------------ | -------------------------------- | -------- | ---------------- | ----- | ---------- |
| TC_001       | Valid Email + Invalid Password   | High     | Yes              | No    | Yes        |
| TC_002       | Invalid Email + Valid Password   | High     | Yes              | No    | Yes        |
| TC_003       | Invalid Email + Invalid Password | High     | Yes              | No    | Yes        |
| TC_004       | Empty Email                      | Medium   | Yes              | No    | Yes        |
| TC_005       | Empty Password                   | Medium   | Yes              | No    | Yes        |
| TC_006       | Both Fields Empty                | Medium   | Yes              | No    | Yes        |
| TC_007       | Successful Login                 | Critical | Yes              | Yes   | Yes        |

---

## Events Module

| Test Case ID | Scenario                     | Priority | Automation Ready | Smoke | Regression |
| ------------ | ---------------------------- | -------- | ---------------- | ----- | ---------- |
| TC_008       | Browse Events                | High     | Yes              | Yes   | Yes        |
| TC_009       | Search Existing Event        | High     | Yes              | Yes   | Yes        |
| TC_010       | Search Non-Existing Event    | Medium   | Yes              | No    | Yes        |
| TC_011       | Filter by Category           | Medium   | Yes              | No    | Yes        |
| TC_012       | Filter by City               | Medium   | Yes              | No    | Yes        |
| TC_013       | Filter by Category and City  | Medium   | Yes              | No    | Yes        |
| TC_014       | No Result Filter Combination | Medium   | Yes              | No    | Yes        |

---

## Booking Module

| Test Case ID | Scenario                                     | Priority | Automation Ready | Smoke | Regression |
| ------------ | -------------------------------------------- | -------- | ---------------- | ----- | ---------- |
| TC_015       | Open Event Detail via Book Now               | High     | Yes              | Yes   | Yes        |
| TC_016       | Increase Ticket Quantity                     | High     | Yes              | No    | Yes        |
| TC_017       | Maximum Ticket Limit Validation              | High     | Yes              | No    | Yes        |
| TC_018       | Minimum Ticket Limit Validation              | High     | Yes              | No    | Yes        |
| TC_019       | More Tickets Than Available Seats            | Critical | Yes              | No    | Yes        |
| TC_020       | Successful Booking After Quantity Correction | Critical | Yes              | Yes   | Yes        |
| TC_021       | Successful Booking with Valid Data           | Critical | Yes              | Yes   | Yes        |
| TC_022       | Empty Attendee Name                          | High     | Yes              | No    | Yes        |
| TC_023       | Invalid Email Format                         | High     | Yes              | No    | Yes        |
| TC_024       | Invalid Contact Number                       | High     | Yes              | No    | Yes        |
| TC_025       | Empty Contact Number                         | High     | Yes              | No    | Yes        |
| TC_026       | All Attendee Fields Empty                    | High     | Yes              | No    | Yes        |
| TC_027       | Verify Booking Details                       | High     | Yes              | No    | Yes        |
| TC_028       | Browse More Events After Booking             | Medium   | Yes              | No    | Yes        |
| TC_029       | View My Bookings After Booking               | High     | Yes              | Yes   | Yes        |

---

## My Bookings Module

| Test Case ID | Scenario                       | Priority | Automation Ready | Smoke | Regression |
| ------------ | ------------------------------ | -------- | ---------------- | ----- | ---------- |
| TC_030       | View Booking Details           | High     | Yes              | No    | Yes        |
| TC_031       | Back to My Bookings Navigation | Medium   | Yes              | No    | Yes        |
| TC_032       | Cancel Booking                 | Critical | Yes              | Yes   | Yes        |
| TC_033       | Abort Booking Cancellation     | High     | Yes              | No    | Yes        |
| TC_034       | Cancel Specific Booking        | High     | Yes              | No    | Yes        |
| TC_035       | Clear All Bookings             | Critical | Yes              | No    | Yes        |
| TC_036       | Abort Clear All Bookings       | High     | Yes              | No    | Yes        |
| TC_037       | Empty State Validation         | Medium   | Yes              | No    | Yes        |

---

## Logout Module

| Test Case ID | Scenario                            | Priority | Automation Ready | Smoke | Regression |
| ------------ | ----------------------------------- | -------- | ---------------- | ----- | ---------- |
| TC_038       | Successful Logout                   | Critical | Yes              | Yes   | Yes        |
| TC_039       | Access Protected Pages After Logout | Critical | Yes              | No    | Yes        |
| TC_040       | Login Again After Logout            | High     | Yes              | Yes   | Yes        |
| TC_041       | Session Data Persistence Validation | High     | Yes              | No    | Yes        |

---

## Summary

| Module      | Total Test Cases |
| ----------- | ---------------- |
| Login       | 7                |
| Events      | 7                |
| Booking     | 15               |
| My Bookings | 8                |
| Logout      | 4                |
| **Total**   | **41**           |

### Test Suite Breakdown

* **Critical:** 7
* **High:** 24
* **Medium:** 10
* **Smoke Tests:** 10
* **Regression Tests:** 41
* **Automation Ready:** 41





