QA Manual Test Cases:-
Member 1:- Abhishek Debnath
Query/Test cases:- EventHub

---

Human Thinking Test Cases TestCases_001:- (New User Registration)
------------------------------------------------------------------
1. Go to eventhub.rahulshettyacademy.com/login
2. Click on "Register" link below the Sign In button
3. Enter invalid email format like "abc@" in the Email field
4. Enter a weak password like "password" (no uppercase, number or symbol)
5. Click on Create Account
6. Check if password format validations are shown 
7. Enter valid email like "testuser@yopmail.com"
8. Enter password missing uppercase like "test@1234"
9. Check if the uppercase rule still shows as not satisfied
10. Enter valid password "Test@1234" satisfying password validation
11. Check if password green chack mark is shown
12. Enter a different value in Confirm Password field
13. Click on Create Account
14. Check validation error for password mismatch
15. Enter "Test@1234" in Confirm Password to match
16. Click on Create Account
17. Check if user is redirected to the home dashboard
18. Check if user email is shown in the top navbar
    
TestCases_002:- (Event Booking)
------------------------------------------------------------------
1. On the home dashboard check if Featured Events section is visible
2. Note down event name, date, city, price and available seats for first event
3. Click on "Book Now" for the event "Dilli Diwali Mela"
4. Check event detail page shows date, time, venue, city, available seats and price 5. Check default ticket quantity is set to 1
6. Click the "+" button more than 10 times
7. Check if ticket quantity stops at max 10
8. Set ticket quantity back to 1
9. Leave Full Name field empty and click Confirm Booking
10. Check if Full Name field shows required field validation
11. Enter Full Name as "Test User"
12. Enter Email as "testuser@yopmail.com"
13. Enter Phone Number as "9876543210"
14. Check if total price updates correctly showing "$300 x 1 = $300"
15. Click on Confirm Booking
16. Check if confirmation message shows "Booking Confirmed!"
17. Note down the Booking Reference number displayed
    
TestCases_003:- (Booking Cancellation)
------------------------------------------------------------------
1. Click on "My Bookings" from the top navbar
2. Check if the booked event is listed with status "confirmed"
3. Check booking reference, event name, date, tickets, city and total match
4. Click on "Cancel Booking" button on the booking card
5. Check if a confirmation modal appears
6. Check the modal message mentions the correct booking reference and seat count
7. Click the "Cancel" button inside the modal to dismiss
8. Check if booking is still showing with confirmed status
9. Click on "Cancel Booking" again
10. Click "Yes, cancel it" button in the modal
11. Check if a success toast message appears saying "Booking cancelled successfully"
12. Check if the bookings list now shows "No bookings yet"
    
TestCases_004:- (Logout)
------------------------------------------------------------------
1. Click on "Logout" button visible in the top navbar
2. Check if user is redirected back to the login page
3. Check that email and password fields are empty on the login page
4. Try navigating to /bookings directly in the browser
5. Check if protected page is not accessible and user is redirected to login


# AI Manual Test Cases:-

**Member 1:-** QA / Automation Agent
**Prompt:-** Write test cases for EventHub — New user creation, event booking, booking cancel, logout
**Website URL:-** https://eventhub.rahulshettyacademy.com/login
**Test Date:-** June 18, 2026

---

## TestCases_001: New User Registration (Happy Path)

1. Navigate to https://eventhub.rahulshettyacademy.com/register
2. Enter a valid email address in the **Email** field (e.g., `user@test.com`)
3. Enter a valid password in the **Password** field (minimum 8 characters, 1 uppercase letter, 1 number, 1 special character, e.g., `Test@1234`)
4. Re-enter the same password in the **Confirm Password** field (`Test@1234`)
5. Verify all four password validation requirements show green checkmarks (✓ At least 8 characters, ✓ One uppercase letter, ✓ One number, ✓ One special character)
6. Click the **Create Account** button
7. Verify the user is redirected to the Dashboard (URL: `https://eventhub.rahulshettyacademy.com/`)
8. Verify the user email is displayed in the top-right navigation bar
9. Verify the navigation links are visible: Home, Events, My Bookings, API Docs, Admin
10. Verify the **Logout** button is visible next to the user email

---

## TestCases_002: New User Registration — Password Validation Failures

1. Navigate to https://eventhub.rahulshettyacademy.com/register
2. Enter a valid email address (e.g., `user@test.com`)
3. Enter a password with fewer than 8 characters (e.g., `Test@1`) in the **Password** field
4. Verify the "At least 8 characters" validation requirement shows a failure indicator (✗ or no green checkmark)
5. Clear the **Password** field
6. Enter a password without an uppercase letter (e.g., `test@1234`) in the **Password** field
7. Verify the "One uppercase letter (A–Z)" validation requirement shows a failure indicator
8. Clear the **Password** field
9. Enter a password without a number (e.g., `Test@abcd`) in the **Password** field
10. Verify the "One number (0–9)" validation requirement shows a failure indicator
11. Clear the **Password** field
12. Enter a password without a special character (e.g., `Test1234`) in the **Password** field
13. Verify the "One special character (!@#$%^&*…)" validation requirement shows a failure indicator
14. Verify the **Create Account** button is not clickable or an error message is shown

---

## TestCases_003: New User Registration — Confirm Password Mismatch

1. Navigate to https://eventhub.rahulshettyacademy.com/register
2. Enter a valid email address (e.g., `user@test.com`)
3. Enter a valid password in the **Password** field (e.g., `Test@1234`)
4. Enter a different password in the **Confirm Password** field (e.g., `Different@123`)
5. Click the **Create Account** button
6. Verify an error message is displayed indicating passwords do not match
7. Verify the user is NOT redirected to the Dashboard

---

## TestCases_004: New User Registration — Duplicate Email

1. Navigate to https://eventhub.rahulshettyacademy.com/register
2. Enter an email that was previously registered (e.g., `user@test.com`) in the **Email** field
3. Enter a valid password in the **Password** field (e.g., `Test@1234`)
4. Re-enter the same password in the **Confirm Password** field
5. Click the **Create Account** button
6. Verify an error message is displayed indicating the email is already registered
7. Verify the user is NOT redirected to the Dashboard

---

## TestCases_005: Login — Happy Path

1. Navigate to https://eventhub.rahulshettyacademy.com/login
2. Enter a valid registered email address in the **Email** field (e.g., `user@test.com`)
3. Enter the correct password in the **Password** field (e.g., `Test@1234`)
4. Click the **Sign In** button
5. Verify the user is redirected to the Dashboard (URL: `https://eventhub.rahulshettyacademy.com/`)
6. Verify the user email is displayed in the top-right navigation bar
7. Verify all navigation links are visible: Home, Events, My Bookings, API Docs, Admin, Logout

---

## TestCases_006: Login — Invalid Email

1. Navigate to https://eventhub.rahulshettyacademy.com/login
2. Enter an invalid or unregistered email address in the **Email** field (e.g., `nonexistent@test.com`)
3. Enter any password in the **Password** field (e.g., `Test@1234`)
4. Click the **Sign In** button
5. Verify an error message is displayed indicating invalid credentials
6. Verify the user is NOT redirected to the Dashboard
7. Verify the user remains on the Login page

---

## TestCases_007: Login — Invalid Password

1. Navigate to https://eventhub.rahulshettyacademy.com/login
2. Enter a valid registered email address in the **Email** field (e.g., `user@test.com`)
3. Enter an incorrect password in the **Password** field (e.g., `WrongPass123!`)
4. Click the **Sign In** button
5. Verify an error message is displayed indicating invalid credentials
6. Verify the user is NOT redirected to the Dashboard
7. Verify the user remains on the Login page

---

## TestCases_008: Login — Empty Fields

1. Navigate to https://eventhub.rahulshettyacademy.com/login
2. Leave the **Email** field empty
3. Leave the **Password** field empty
4. Click the **Sign In** button
5. Verify an error message is displayed indicating email and password are required
6. Verify the user remains on the Login page

---

## TestCases_009: Login — CAPTCHA After Multiple Failed Attempts

1. Navigate to https://eventhub.rahulshettyacademy.com/login
2. Enter a valid registered email address in the **Email** field
3. Enter an incorrect password in the **Password** field
4. Click the **Sign In** button
5. Verify an error message is displayed
6. Repeat steps 2-5 three more times (4 total failed attempts)
7. Verify a CAPTCHA challenge or "Too many attempts" message appears on the login form
8. Verify the user cannot proceed with login until CAPTCHA is solved or waiting period elapses

---

## TestCases_010: Browse Events — View All Events

1. Login with valid credentials
2. Click on **Events** in the navigation bar
3. Verify the page URL is `https://eventhub.rahulshettyacademy.com/events`
4. Verify the page heading shows "Upcoming Events"
5. Verify the search bar is visible with placeholder "Search events, venues…"
6. Verify the Category dropdown shows options: All Categories, Conference, Concert, Sports, Workshop, Festival
7. Verify the City dropdown shows options: All Cities, Mumbai, Bangalore, Delhi, Hyderabad, Chennai, Pune
8. Verify at least one event card is visible with: event image, event name, category tag, date, venue, city, price, seats available, and **Book Now** button

---

## TestCases_011: Browse Events — Search and Filter

1. Login with valid credentials
2. Click on **Events** in the navigation bar
3. Type a search term in the search bar (e.g., "Diwali")
4. Verify the event list is filtered to show only matching events
5. Clear the search bar
6. Verify all events are displayed again
7. Select "Concert" from the **Category** dropdown
8. Verify only Concert-type events are displayed
9. Select "Delhi" from the **City** dropdown
10. Verify only events in Delhi are displayed
11. Reset both filters to "All Categories" and "All Cities"
12. Verify all events are displayed again

---

## TestCases_012: Event Detail Page — View Event Information

1. Login with valid credentials
2. Navigate to the Events page
3. Click on any event card (e.g., "Dilli Diwali Mela")
4. Verify the page URL is `https://eventhub.rahulshettyacademy.com/events/{event_id}`
5. Verify the event name is displayed as a heading
6. Verify the event image is visible
7. Verify the event details are shown: Date, Time, Venue, City, Available seats, Price per ticket
8. Verify the "About this event" description section is visible
9. Verify the "Book Tickets" section is visible on the right side with: ticket price, ticket counter (default 1), Full Name field, Email field, Phone Number field, price summary, and **Confirm Booking** button
10. Verify the breadcrumb navigation shows: Events / {Event Name}

---

## TestCases_013: Event Booking — Happy Path

1. Login with valid credentials
2. Navigate to an event detail page (e.g., /events/3)
3. Verify the ticket count is set to 1 (default)
4. Enter a valid name in the **Full Name*** field (e.g., "John Doe")
5. Enter a valid email in the **Email*** field (e.g., "john@test.com")
6. Enter a valid phone number in the **Phone Number*** field (e.g., "+91 9876543210")
7. Verify the price summary shows: {price} × 1 ticket = {total}
8. Verify the **Total** amount is correct
9. Click the **Confirm Booking** button
10. Verify the "Booking Confirmed! 🎉" success message is displayed
11. Verify the message "Your tickets are reserved." is shown
12. Verify a booking reference number is displayed (e.g., D-HPAAZZ)

---

## TestCases_014: Event Booking — Multiple Tickets

1. Login with valid credentials
2. Navigate to an event detail page (e.g., /events/3)
3. Click the **+** button on the ticket counter to increase quantity to 3
4. Verify the ticket count displays "3"
5. Verify the price summary updates: {price} × 3 tickets = {price × 3}
6. Verify the **Total** amount updates correctly
7. Enter a valid name in the **Full Name*** field
8. Enter a valid email in the **Email*** field
9. Enter a valid phone number in the **Phone Number*** field
10. Click the **Confirm Booking** button
11. Verify the "Booking Confirmed! 🎉" success message is displayed

---

## TestCases_015: Event Booking — Maximum Ticket Limit

1. Login with valid credentials
2. Navigate to an event detail page (e.g., /events/3)
3. Click the **+** button repeatedly until the ticket count reaches 10
4. Verify the ticket count displays "10" (maximum)
5. Verify the **+** button is now disabled (cannot increase further)
6. Verify the text "(max 10)" is visible next to the counter

---

## TestCases_016: Event Booking — Minimum Ticket Limit

1. Login with valid credentials
2. Navigate to an event detail page (e.g., /events/3)
3. Verify the ticket count starts at 1 (default)
4. Verify the **−** button is disabled (cannot decrease below 1)

---

## TestCases_017: Event Booking — Empty Required Fields

1. Login with valid credentials
2. Navigate to an event detail page (e.g., /events/3)
3. Leave all fields empty (Full Name, Email, Phone Number)
4. Click the **Confirm Booking** button
5. Verify validation error messages are displayed for: Full Name, Email, Phone Number
6. Verify the booking is NOT confirmed
7. Verify the user remains on the event detail page

---

## TestCases_018: Event Booking — Invalid Email Format

1. Login with valid credentials
2. Navigate to an event detail page (e.g., /events/3)
3. Enter a valid name in the **Full Name*** field
4. Enter an invalid email format in the **Email*** field (e.g., "notanemail")
5. Enter a valid phone number in the **Phone Number*** field
6. Click the **Confirm Booking** button
7. Verify an email validation error message is displayed
8. Verify the booking is NOT confirmed

---

## TestCases_019: My Bookings — View Bookings List

1. Login with valid credentials (with at least one existing booking)
2. Click on **My Bookings** in the navigation bar
3. Verify the page URL is `https://eventhub.rahulshettyacademy.com/bookings`
4. Verify the page heading shows "My Bookings"
5. Verify the description text "View and manage all your ticket bookings" is displayed
6. Verify at least one booking card is visible
7. Verify each booking card displays: booking reference, status badge ("confirmed"), booking ID (e.g., #63737), event name, date, number of tickets, city, booked date, and total price
8. Verify the **View Details** button is visible on each booking card
9. Verify the **Cancel Booking** button is visible on each booking card
10. Verify the **Clear all bookings** button is visible at the top

---

## TestCases_020: My Bookings — View Booking Details

1. Login with valid credentials (with at least one existing booking)
2. Navigate to the My Bookings page
3. Click the **View Details** button on a booking
4. Verify the page URL is `https://eventhub.rahulshettyacademy.com/bookings/{booking_id}`
5. Verify the booking status badge shows "confirmed"
6. Verify the event name is displayed
7. Verify the booking details are shown: date, tickets, city, booked date
8. Verify the **Cancel Booking** button is visible
9. Verify the **Check eligibility for refund?** button is visible
10. Verify the **← Back to My Bookings** button is visible
11. Click the **← Back to My Bookings** button
12. Verify the user is redirected back to the My Bookings list page

---

## TestCases_021: Cancel Booking — Happy Path

1. Login with valid credentials (with at least one confirmed booking)
2. Navigate to the My Bookings page
3. Click the **Cancel Booking** button on a confirmed booking
4. Verify a browser confirmation dialog appears (e.g., "Are you sure you want to cancel this booking?")
5. Click **OK** or **Yes** on the confirmation dialog
6. Verify the booking status changes from "confirmed" to "cancelled"
7. Verify the booking card reflects the updated status

---

## TestCases_022: Cancel Booking — From Booking Detail Page

1. Login with valid credentials (with at least one confirmed booking)
2. Navigate to the My Bookings page
3. Click **View Details** on a confirmed booking
4. Verify the booking detail page loads with status "confirmed"
5. Click the **Cancel Booking** button
6. Verify a browser confirmation dialog appears
7. Click **OK** or **Yes** on the confirmation dialog
8. Verify the booking status changes from "confirmed" to "cancelled"

---

## TestCases_023: Cancel Booking — Decline Confirmation

1. Login with valid credentials (with at least one confirmed booking)
2. Navigate to the My Bookings page
3. Click the **Cancel Booking** button on a confirmed booking
4. Verify a browser confirmation dialog appears
5. Click **Cancel** or **No** on the confirmation dialog
6. Verify the booking status remains "confirmed"
7. Verify the booking is NOT cancelled

---

## TestCases_024: Clear All Bookings

1. Login with valid credentials (with at least one existing booking)
2. Navigate to the My Bookings page
3. Verify at least one booking is visible
4. Click the **Clear all bookings** button
5. Verify all bookings are removed from the list
6. Verify the page shows an empty state (e.g., "No bookings found" or similar message)

---

## TestCases_025: Logout — Happy Path

1. Login with valid credentials
2. Verify the user email is displayed in the navigation bar
3. Click the **Logout** button
4. Verify the user is redirected to the Login page (URL: `https://eventhub.rahulshettyacademy.com/login`)
5. Verify the login form is visible (Email, Password, Sign In button)
6. Verify the "Don't have an account? Register" link is visible

---

## TestCases_026: Logout — Session Invalidation

1. Login with valid credentials
2. Note the current URL (Dashboard)
3. Click the **Logout** button
4. Verify the user is redirected to the Login page
5. Attempt to navigate directly to `https://eventhub.rahulshettyacademy.com/` (Dashboard)
6. Verify the user is redirected back to the Login page
7. Verify the user cannot access any protected pages (Events, My Bookings) without logging in again

---

## TestCases_027: Navigation — All Links Work

1. Login with valid credentials
2. Click on **Home** in the navigation bar
3. Verify the page URL is `https://eventhub.rahulshettyacademy.com/`
4. Click on **Events** in the navigation bar
5. Verify the page URL is `https://eventhub.rahulshettyacademy.com/events`
6. Click on **My Bookings** in the navigation bar
7. Verify the page URL is `https://eventhub.rahulshettyacademy.com/bookings`
8. Click on **EventHub** logo/brand name
9. Verify the user is redirected to the Dashboard (`/`)

---

## TestCases_028: Navigation — Breadcrumbs and Back Navigation

1. Login with valid credentials
2. Navigate to the Events page
3. Click on an event card to view its details
4. Verify the breadcrumb shows: Events / {Event Name}
5. Click on **Events** in the breadcrumb
6. Verify the user is redirected back to the Events list page
7. Navigate to an event detail page again
8. Verify the breadcrumb shows: Events / {Event Name}

---

## TestCases_029: Event Detail — Featured Event Badge

1. Login with valid credentials
2. Navigate to the Events page
3. Identify an event with the "Featured" badge
4. Click on the featured event
5. Verify the "Featured" badge is displayed on the event detail page
6. Verify the message "This is a featured event — always available for practice" is shown
7. Verify the event has available seats (e.g., "10000 / 10000 seats")

---

## TestCases_030: Admin Panel — Access Control

1. Login with valid credentials
2. Click on the **Admin** button in the navigation bar
3. Verify the Admin dropdown or admin panel loads
4. Verify the user can access the admin features (Manage Events, Manage Bookings)
5. Verify the admin panel shows event management options

---

## TestCases_031: Full End-to-End Flow — Register to Booking to Cancel to Logout

1. Navigate to https://eventhub.rahulshettyacademy.com/register
2. Enter a new email address in the **Email** field (e.g., `e2e_test_{timestamp}@test.com`)
3. Enter a valid password in the **Password** field (e.g., `Test@1234`)
4. Re-enter the same password in the **Confirm Password** field
5. Click the **Create Account** button
6. Verify the user is redirected to the Dashboard
7. Click on **Events** in the navigation bar
8. Verify the Events page loads with event listings
9. Click on any event (e.g., "Dilli Diwali Mela")
10. Verify the event detail page loads
11. Enter a name in the **Full Name*** field (e.g., "E2E Test User")
12. Enter the registered email in the **Email*** field
13. Enter a phone number in the **Phone Number*** field (e.g., "+91 9999999999")
14. Click the **Confirm Booking** button
15. Verify the "Booking Confirmed! 🎉" success message is displayed
16. Click on **My Bookings** in the navigation bar
17. Verify the new booking appears in the list with status "confirmed"
18. Click the **Cancel Booking** button on the new booking
19. Click **OK** on the confirmation dialog
20. Verify the booking status changes to "cancelled"
21. Click the **Logout** button
22. Verify the user is redirected to the Login page
23. Attempt to navigate to `https://eventhub.rahulshettyacademy.com/` directly
24. Verify the user is redirected back to the Login page (session invalidated)

---

## Summary

| Test Case | Category | Description |
|-----------|----------|-------------|
| TC_001 | Registration | Happy path registration |
| TC_002 | Registration | Password validation failures |
| TC_003 | Registration | Confirm password mismatch |
| TC_004 | Registration | Duplicate email |
| TC_005 | Login | Happy path login |
| TC_006 | Login | Invalid email |
| TC_007 | Login | Invalid password |
| TC_008 | Login | Empty fields |
| TC_009 | Login | CAPTCHA after failed attempts |
| TC_010 | Events | View all events |
| TC_011 | Events | Search and filter |
| TC_012 | Events | Event detail page |
| TC_013 | Booking | Happy path booking |
| TC_014 | Booking | Multiple tickets |
| TC_015 | Booking | Maximum ticket limit |
| TC_016 | Booking | Minimum ticket limit |
| TC_017 | Booking | Empty required fields |
| TC_018 | Booking | Invalid email format |
| TC_019 | My Bookings | View bookings list |
| TC_020 | My Bookings | View booking details |
| TC_021 | Cancel | Happy path cancel |
| TC_022 | Cancel | Cancel from detail page |
| TC_023 | Cancel | Decline confirmation |
| TC_024 | My Bookings | Clear all bookings |
| TC_025 | Logout | Happy path logout |
| TC_026 | Logout | Session invalidation |
| TC_027 | Navigation | All links work |
| TC_028 | Navigation | Breadcrumbs and back |
| TC_029 | Events | Featured event badge |
| TC_030 | Admin | Access control |
| TC_031 | E2E | Full register → book → cancel → logout flow |

**Total Test Cases: 31**

Your thoughts:-
● What you felt Suitable:- Extensive coverage of almost all scenarios available, nothing is left out
● What you felt Not suitable:- Too much information can cause confusion especially when doing smoke testing, a few of the negative cases may not be even replicated in real world scenarios.


Final Test Case:-
AI + Manual, Combined and made automation-ready

---

TestCases_001: New User Registration — Automation Ready
------------------------------------------------------------------
1. Navigate to https://eventhub.rahulshettyacademy.com/login
2. Verify page title is 'EventHub — Discover & Book Events'
3. Verify Email field, Password field and Sign In button are visible
4. Verify 'Don't have an account? Register' link is visible below Sign In
5. Click the Register link — verify URL changes to /register
6. Verify form shows Email, Password and Confirm Password fields
7. Verify 4 password rule hints are shown below Password field
8. Leave Email blank, click Create Account — verify required field error
9. Enter 'plaintext' (no @) — verify invalid email format error
10. Enter 'missing@' (no domain) — verify invalid email format error
11. Enter valid email 'testuser_auto@yopmail.com'
12. Enter 'short' (< 8 chars) — verify length rule shows as failed
13. Enter 'alllower1!' (no uppercase) — verify uppercase rule shows as failed
14. Enter 'NOLOWER1!' (no lowercase) — verify appropriate rule indicator shows
15. Enter 'NoNumber!!' (no digit) — verify number rule shows as failed
16. Enter 'NoSpecial1' (no symbol) — verify special character rule shows as failed
17. Enter 'Test@1234' — verify all 4 rule indicators turn green
18. Enter 'Mismatch@9999' in Confirm Password — verify mismatch error appears
19. Enter 'Test@1234' in Confirm Password — verify mismatch error disappears
20. Click Create Account
21. Verify redirect to Dashboard URL: https://eventhub.rahulshettyacademy.com/
22. Verify 'testuser_auto@yopmail.com' is displayed in top-right navbar
23. Verify nav links visible: Home, Events, My Bookings, API Docs, Admin, Logout
24. Logout, navigate to /register, attempt same email 'testuser_auto@yopmail.com'
25. Verify error message is shown: email already registered
26. Verify user is NOT redirected to Dashboard
    
TestCases_002: Login — Automation Ready
------------------------------------------------------------------
1. Navigate to https://eventhub.rahulshettyacademy.com/login
2. Leave Email and Password empty, click Sign In — verify required field errors
3. Enter unregistered email 'ghost@test.com', any password, click Sign In — verify invalid credentials error
4. Enter valid email 'testuser_auto@yopmail.com', wrong password 'Wrong@9999', click Sign In — verify invalid credentials error
5. Verify user remains on /login after all failed attempts
6. Enter valid email 'testuser_auto@yopmail.com' and correct password 'Test@1234'
7. Click Sign In
8. Verify redirect to Dashboard URL: https://eventhub.rahulshettyacademy.com/
9. Verify user email is shown in top-right navbar
10. Verify nav links visible: Home, Events, My Bookings, API Docs, Admin, Logout
    
TestCases_003: Browse Events — Automation Ready
------------------------------------------------------------------
1. Login with valid credentials
2. Verify Featured Events section is visible on the Dashboard with at least 1 event card
3. Verify each card shows: event name, category badge, date, venue, city, price, seats, Book Now button
4. Click on Events in navbar — verify URL is /events
5. Verify page heading 'Upcoming Events' is displayed
6. Verify search bar with placeholder 'Search events, venues...' is visible
7. Verify Category dropdown options: All Categories, Conference, Concert, Sports, Workshop, Festival
8. Verify City dropdown options: All Cities, Mumbai, Bangalore, Delhi, Hyderabad, Chennai, Pune
9. Type 'Diwali' in search bar — verify only matching events shown   
10. Clear search — verify all events are displayed again
11. Select 'Concert' from Category — verify only Concert events shown 12. Select 'Delhi' from City — verify only Delhi events shown
13. Reset both filters — verify all events are displayed

TestCases_004: Event Detail Page — Automation Ready
------------------------------------------------------------------
1. Click 'Book Now' on 'Dilli Diwali Mela' from Events page
2. Verify URL is /events/3
3. Verify event name 'Dilli Diwali Mela' is shown as heading
4. Verify event details: date Tuesday 20 October, time 10:30 pm, venue Pragati Maidan Exhibition Grounds, city Delhi 5. Verify available seats counter is shown (e.g., 10000 / 10000)
6. Verify price per ticket shows '$300'
7. Verify 'About this event' description section is visible
8. Verify breadcrumb shows: Events / Dilli Diwali Mela
9. Click 'Events' in breadcrumb — verify redirect back to /events
10. Verify 'Featured' badge is displayed on the event detail page
11. Verify 'This is a featured event — always available for practice' message is shown
    
TestCases_005: Event Booking — Automation Ready
------------------------------------------------------------------
1. Navigate to /events/3 (Dilli Diwali Mela)
2. Verify Book Tickets section is visible with ticket counter, Full Name, Email, Phone fields and Confirm Booking button 3. Verify default ticket quantity is 1
4. Verify - (minus) button is disabled at quantity 1
5. Click + button — verify quantity increases to 2, total price updates to $600
6. Click + button until quantity reaches 10 — verify it stops at 10
7. Verify + button is disabled at quantity 10
8. Verify '(max 10)' text is visible next to the counter
9. Reset quantity to 1 — verify total is $300
10. Click Confirm Booking with all fields empty — verify validation errors for Full Name, Email, Phone Number
11. Enter Full Name 'Test User', Email 'invalid-email', Phone '9876543210'
12. Click Confirm Booking — verify email format validation error
13. Fix email to 'testuser_auto@yopmail.com'
14. Verify price summary shows '$300 x 1 ticket = $300'
15. Click Confirm Booking
16. Verify 'Booking Confirmed!' success message is displayed
17. Verify 'Your tickets are reserved.' message is shown
18. Verify Booking Reference number is displayed (format: D-XXXXX)
19. Verify Customer name, Tickets count and Total amount are shown correctly
20. Note Booking Reference for use in cancellation test

TestCases_006: My Bookings — Automation Ready
------------------------------------------------------------------
1. Click My Bookings in navbar — verify URL is /bookings
2. Verify page heading 'My Bookings' and description 'View and manage all your ticket bookings' are displayed 3. Verify booking card is visible with: booking reference, status badge 'confirmed', booking ID, event name, date, tickets, city, booked date, total price
4. Verify 'View Details' and 'Cancel Booking' buttons are present on the card
5. Verify 'Clear all bookings' button is visible at the top of the page
6. Click 'View Details' on the booking
7. Verify URL is /bookings/{booking_id}
8. Verify booking status badge shows 'confirmed'
9. Verify event name, date, tickets, city and booked date are shown
10. Verify 'Cancel Booking' button is visible
11. Verify 'Check eligibility for refund?' button is visible
12. Click 'Back to My Bookings' — verify redirect to /bookings
    
TestCases_007: Booking Cancellation — Automation Ready
------------------------------------------------------------------
1. Navigate to /bookings
2. Verify booking with status 'confirmed' is listed
3. Click 'Cancel Booking' on the booking card
4. Verify a confirmation modal appears with cancellation warning
5. Verify modal text references the correct booking reference and seat release count
6. Verify modal has two buttons: Cancel (dismiss) and Yes, cancel it (confirm)
7. Click Cancel in the modal — verify modal closes and booking status remains 'confirmed' 8. Click 'Cancel Booking' again
9. Click 'Yes, cancel it' in the modal
10. Verify success toast appears: 'Booking cancelled successfully'
11. Verify toast disappears after a few seconds
12. Verify booking list shows 'No bookings yet' empty state
13. Verify 'Browse Events' CTA is present on the empty state
14. Refresh page — verify cancelled booking does not reappear
15. Navigate to /bookings via URL — verify empty state persists
16. Click 'Clear all bookings' (when bookings exist) — verify all are removed
    
TestCases_008: Logout and Session Security — Automation Ready
------------------------------------------------------------------
1. Verify Logout button is visible in navbar while logged in
2. Verify logged-in user email is displayed alongside Logout button
3. Click Logout button
4. Verify redirect to /login
5. Verify login form is displayed with empty Email and Password fields
6. Verify 'Don't have an account? Register' link is visible
7. Verify user email and Logout button are no longer in navbar
8. Click browser Back button — verify authenticated page does NOT load 9. Navigate directly to / (Dashboard) — verify redirect to /login
10. Navigate directly to /bookings — verify redirect to /login
11. Navigate directly to /events — verify redirect to /login
12. Login again with valid credentials — verify session is restored correctly
    
TestCases_009: Navigation — Automation Ready
------------------------------------------------------------------
1. Login with valid credentials
2. Click Home in navbar — verify URL is https://eventhub.rahulshettyacademy.com/ 3. Click Events in navbar — verify URL is /events
4. Click My Bookings in navbar — verify URL is /bookings
5. Click EventHub logo — verify redirect to Dashboard (/)
6. Click API Docs — verify API documentation page or external link opens
7. Click Admin — verify Admin panel or dropdown loads
   
TestCases_010: Full E2E Flow — Register > Book > Cancel > Logout
------------------------------------------------------------------
1. Navigate to https://eventhub.rahulshettyacademy.com/register
2. Enter unique email 'e2e_test_{timestamp}@test.com', password 'Test@1234', confirm password 'Test@1234' 3. Click Create Account — verify redirect to Dashboard
4. Verify registered email shown in navbar
5. Click Events — verify /events page loads with event listings
6. Click 'Book Now' on 'Dilli Diwali Mela'
7. Enter Full Name 'E2E Test User', Email 'e2e_test_{timestamp}@test.com', Phone '+91 9999999999'
8. Click Confirm Booking — verify 'Booking Confirmed!' is shown with a Booking Reference
9. Click My Bookings — verify new booking appears with status 'confirmed'
10. Click 'Cancel Booking' — verify confirmation modal appears
11. Click 'Yes, cancel it' — verify 'Booking cancelled successfully' toast appears
12. Verify booking list shows 'No bookings yet' 
13. Click Logout — verify redirect to /login
14. Attempt to navigate to / directly — verify redirect to /login (session invalidated)
