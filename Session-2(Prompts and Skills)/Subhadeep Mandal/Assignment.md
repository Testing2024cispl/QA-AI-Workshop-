Member : Subhradeep Mandal 
Test site :- https://blazedemo.com/
Date- 17/06/26


Human Thinking Test Cases:-

HTTC_001: Verify “Destination of the week ! The Beach!“ hypertext redirection is working correctly
Steps:
1. Go to https://blazedemo.com/
2. Click on “Destination of the week ! The Beach!” hypertext
Expected Result: It should redirect to the Destination of the week page with where destination place name and the image should show correctly

HTTC_002: Verify search flights functionality working correctly
Steps:
1. Go to https://blazedemo.com/
2. Select departure city
3. Select destination city
4. Click on find flights button
Expected Result: All flight details ,Departs city name and Arrives city name should show correctly

HTTC_003: Verify purchase flight functionality working correctly
Steps:
1. Go to https://blazedemo.com/
2. Select departure city
3. Select destination city
4. Click on find flights button
5. Click on choose this flight button of any flight 
6. Fill up all required fields 
7. Click on purchase flight button 
Expected Result: 
1. It should redirect to the thank you page
2. All flight booking details should show correctly
3. For credit card number only last 4 digits should visible 

HTTC_004: Verify after book a flight the flight booking ID is unique everytime

HTTC_005: Verify in flight booking page the remember me checkbox functionality is working correctly


HTTC_006: Verify without enter required fields user can’t book a flight
Steps:
1. Go to https://blazedemo.com/
2. Select departure city
3. Select destination city
4. Click on find flights button
5. Click on choose this flight button of any flight 
6. Click on Purchase Flight button without fillup required fields
Expected Result: 
1. It should show some error message similar to : Please fill up required fields to purchase your flight
 2. All the required fields should have asterisk mark on them

HTTC_007: Verify with wrong zip code format user can’t purchase a flight
Steps:
1. Go to https://blazedemo.com/
2. Select departure city
3. Select destination city
4. Click on find flights button
5. Click on choose this flight button of any flight 
6. Enter wrong zip code format (example : 12, tes3,test)
7. Fill up other required fields and click on Purchase Flight button
Expected Result: 
1. Zip code length should be between 5-9 digits 
2. With wrong zipcode submission there should be an error message similar to: Please enter the correct zipcode to purchase your flight.

HTTC_008: Verify with wrong credit card format user can’t purchase a flight
Steps:
1. Go to https://blazedemo.com/
2. Select departure city
3. Select destination city
4. Click on find flights button
5. Click on choose this flight button of any flight 
6. Enter wrong credit card format (example : 123 343, 1212121 212121 2121212)
7. Fill up other required fields and click on Purchase Flight button
Expected Result: 
1. Credit card Number field should accept only 13–19 digits
2. With wrong credit card submission there should be an error message similar to: Please enter the correct credit card Number to purchase your flight.

HTTC_009: Verify with invalid credit card user can’t purchase a flight
Steps:
1. Go to https://blazedemo.com/
2. Select departure city
3. Select destination city
4. Click on find flights button
5. Click on choose this flight button of any flight 
6. Enter invalid credit card number(example : 4111 4444 4444 4444)
7. Fill up other required fields and click on Purchase Flight button
Expected Result: With invalid credit card number there should be an error message similar to: Invalid card, please enter valid card to purchase your flight.


HTTC_010: Verify with wrong month field format user can’t purchase a flight
Steps:
1. Go to https://blazedemo.com/
2. Select departure city
3. Select destination city
4. Click on find flights button
5. Click on choose this flight button of any flight 
6. Enter wrong month format (example : 13, test)
7. Fill up other required fields and click on Purchase Flight button
Expected Result: 
1. Month format should be 1-12 only 
2. With wrong month format submission there should be an error message similar to: Please enter the correct month to purchase your flight.

HTTC_011: Verify with wrong year field format user can’t purchase a flight
Steps:
1. Go to https://blazedemo.com/
2. Select departure city
3. Select destination city
4. Click on find flights button
5. Click on choose this flight button of any flight 
6. Enter wrong year format (example : 123, tes3,test)
7. Fill up other required fields and click on Purchase Flight button
Expected Result: 
1. With wrong month format submission there should be an error message similar to: Please enter the correct year to purchase your flight.

HTTC_012: Verify user can’t purchase a flight with an expire card
Steps:
1. Go to https://blazedemo.com/
2. Select departure city
3. Select destination city
4. Click on find flights button
5. Click on choose this flight button of any flight 
6. Enter month and year as expired already(example : month: 12, year: 2020)
7. Fill up other required fields and click on Purchase Flight button
Expected Result: With expired card submission there should be an error message similar to: Your card is expired, please enter another card details.

HTTC_013: Verify “Travel the world” menu redirection working correctly
Steps:
1. Go to https://blazedemo.com/
2. Go to any other page
3. Click on Travel to world
Expected Result: IT should redirect to the search flight page

HTTC_013: Verify “Home” menu redirection working correctly
Steps:
1. Go to https://blazedemo.com/
2. Go to any other page
3. Click on Home
Expected Result: IT should redirect to the login page

HTTC_014: Verify login working correctly
Steps:
1. https://blazedemo.com/login
2. Enter registered email address
3. Enter password
4. Click on login
Expected Result: User should login successfully

HTTC_015: Verify login is not working with invalid credential
Steps:
1. https://blazedemo.com/login
2. Enter non-registered email address
3. Enter password
4. Click on login
Expected Result: There should be an error message: invalid credentials

HTTC_016: Verify login is not working with wrong email format 
Steps:
1. https://blazedemo.com/login
2. Enter wrong email address format (example: test@)
3. Enter password
4. Click on login
Expected Result: There should be an error message: invalid credentials

HTTC_016: Verify login is not working without fill up required fields
Steps:
1. https://blazedemo.com/login
2. Click on login button without enter email and password
Expected Result: There should be an error message: Missing required fields

HTTC_017: Verify forgot password is working correctly
Steps:
1. https://blazedemo.com/login
2. Click on “Forgot your password?” hyperlink
3. Enter registered email address
Expected Result: IT should redirect to the next page of forgot password process

HTTC_018: Verify user can;t use forgot password with wrong email format
Steps:
1. https://blazedemo.com/login
2. Click on “Forgot your password?” hyperlink
3. Enter wrong email format (example: test@)
4. Click on Send password reset link
Expected Result: IT should show some error message,example: wrong email format

HTTC_019: Verify forgot password is not working with non-registered email address
Steps:
1. https://blazedemo.com/login
2. Click on “Forgot your password?” hyperlink
3. Enter non-registered email address
4. Click on Send password reset link
Expected Result: IT should show some error message,example: email not registered

HTTC_020: Verify registration is working correctly
Steps:
1. https://blazedemo.com/register
2. Enter required fields
3. Click on register button
Expected Result: IT should register the user

HTTC_021: Verify registration is working with duplicate email id
Steps:
1. https://blazedemo.com/register
2. Enter an email which is already registered
3. Enter other required fields
4. Click on register button
Expected Result: IT should show error message, example: duplicate email

HTTC_022: Verify registration is not working with wrong email format
Steps:
1. https://blazedemo.com/register
2. Enter wrong email format in email address field (example: test@)
3. Enter other required fields
4. Click on register button
Expected Result: IT should show error message, example: wrong email format

HTTC_023: Verify registration is not working when password and confirm password field does not match
Steps:
1. https://blazedemo.com/register
2. Enter password and confirm password fields different
3. Enter other required fields
3. Click on register button
Expected Result: IT should show error message, example: password and confirm password does not matched
________________________________________________________________________________________________________________________________________________________
AI Manual Test Cases:-
AMTC_001: Verify Register page loads with all fields and elements
Steps:
1. Launch browser
2. Navigate to https://blazedemo.com/register
Expected Result: Register page loads with Name, Company, E-Mail Address, Password, Confirm Password fields and an active Register button. Top nav shows Login and Register.

AMTC_002: Verify successful registration with all valid details
Steps:
1. Navigate to https://blazedemo.com/register
2. Enter a valid Name
3. Enter a Company
4. Enter a valid email format
5. Enter a valid Password
6. Enter the same value in Confirm Password
7. Click Register
Expected Result: User account is created successfully and user is redirected to the logged-in/home page (or success message shown).

AMTC_003: Verify registration is accepted with a valid email format
Steps:
1. Navigate to https://blazedemo.com/register
2. Enter valid email in E-Mail Address field
3. Enter all other required fields validly
4. Click Register
Expected Result: Email is accepted and no email-format error is shown.

AMTC_004: Verify registration fails with wrong email format (missing domain)
Steps:
1. Navigate to https://blazedemo.com/register
2. Enter wrong email format in E-Mail Address field
3. Enter all other required fields
4. Click Register
Expected Result: Error message is shown indicating invalid/wrong email format; registration is not completed.

AMTC_005: Verify registration fails with email missing @ symbol
Steps:
1. Navigate to https://blazedemo.com/register
2. Enter email without @ in E-Mail Address field
3. Enter all other required fields
4. Click Register
Expected Result: Error message for invalid email format is shown; registration is not completed.

AMTC_006: Verify registration fails with email missing local part
Steps:
1. Navigate to https://blazedemo.com/register
2. Enter email with missing local part
3. Enter all other required fields
4. Click Register
Expected Result: Error message for invalid email format is shown; registration is not completed.

AMTC_007: Verify registration fails with email missing top-level domain
Steps:
1. Navigate to https://blazedemo.com/register
2. Enter email without a TLD
3. Enter all other required fields
4. Click Register
Expected Result: Error message for invalid email format is shown; registration is not completed.

AMTC_008: Verify registration fails with email containing spaces
Steps:
1. Navigate to https://blazedemo.com/register
2. Enter email containing a space
3. Enter all other required fields
4. Click Register
Expected Result: Error message for invalid email format is shown; registration is not completed.

AMTC_009: Verify registration fails with email containing multiple @ symbols
Steps:
1. Navigate to https://blazedemo.com/register
2. Enter email with multiple @
3. Enter all other required fields
4. Click Register
Expected Result: Error message for invalid email format is shown; registration is not completed.

AMTC_010: Verify registration fails with email having consecutive dots
Steps:
1. Navigate to https://blazedemo.com/register
2. Enter email with consecutive dots
3. Enter all other required fields
4. Click Register
Expected Result: Error message for invalid email format is shown; registration is not completed.

AMTC_011: Verify registration fails with empty Name field
Steps:
1. Navigate to https://blazedemo.com/register
2. Leave Name field blank
3. Enter all other required fields validly
4. Click Register
Expected Result: Required-field validation error is shown for Name; registration is not completed.

AMTC_012: Verify registration fails with empty E-Mail Address field
Steps:
1. Navigate to https://blazedemo.com/register
2. Leave E-Mail Address field blank
3. Enter all other required fields validly
4. Click Register
Expected Result: Required-field validation error is shown for E-Mail Address; registration is not completed.

AMTC_013: Verify registration fails with empty Password field
Steps:
1. Navigate to https://blazedemo.com/register
2. Leave Password field blank
3. Enter all other required fields validly
4. Click Register
Expected Result: Required-field validation error is shown for Password; registration is not completed.

AMTC_014: Verify registration fails with empty Confirm Password field
Steps:
1. Navigate to https://blazedemo.com/register
2. Enter Password
3. Leave Confirm Password blank
4. Click Register
Expected Result: Required-field/confirmation validation error is shown; registration is not completed.

AMTC_015: Verify registration fails when Password and Confirm Password do not match
Steps:
1. Navigate to https://blazedemo.com/register
2. Enter a Password
3. Enter a different value in Confirm Password
4. Enter all other required fields
5. Click Register
Expected Result: Error message indicating passwords do not match is shown; registration is not completed.

AMTC_016: Verify registration fails with password below minimum length
Steps:
1. Navigate to https://blazedemo.com/register
2. Enter a very short password in Password and Confirm Password
3. Enter all other required fields
4. Click Register
Expected Result: Validation error for minimum password length is shown; registration is not completed.

AMTC_017: Verify Company field is optional
Steps:
1. Navigate to https://blazedemo.com/register
2. Enter Name, Email, Password, Confirm Password
3. Leave Company blank
4. Click Register
Expected Result: Registration proceeds without a Company value (Company is optional).

AMTC_018: Verify Name field rejects only-numeric / special-character input
Steps:
1. Navigate to https://blazedemo.com/register
2. Enter only numbers/special chars in Name
3. Enter all other valid fields
4. Click Register
Expected Result: Validation error for invalid Name is shown; registration is not completed.

AMTC_019: Verify email field handles leading/trailing spaces
Steps:
1. Navigate to https://blazedemo.com/register
2. Enter email with leading and trailing spaces
3. Enter other valid fields
4. Click Register
Expected Result: Spaces are trimmed and email accepted, OR a format error is shown - behavior must be consistent and defined.

AMTC_020: Verify registration with an already registered email is rejected
Steps:
1. Navigate to https://blazedemo.com/register
2. Enter an email that is already registered
3. Enter other valid fields
4. Click Register
Expected Result: Error message indicating the email is already taken is shown; duplicate account is not created.

AMTC_021: Verify Password and Confirm Password fields mask the input
Steps:
1. Navigate to https://blazedemo.com/register
2. Type a value into Password
3. Type a value into Confirm Password
Expected Result: Entered characters are masked (shown as dots/asterisks), not in plain text.

AMTC_022: Verify input fields reject script/XSS injection
Steps:
1. Navigate to https://blazedemo.com/register
2. Enter a script payload in Name/Company
3. Enter other valid fields
4. Click Register
Expected Result: Input is sanitized/escaped; no script executes and no error/breakage occurs.

AMTC_023: Verify field maximum length boundary handling
Steps:
1. Navigate to https://blazedemo.com/register
2. Enter very long strings (e.g. 256+ chars) in each text field
3. Click Register
Expected Result: Fields enforce a defined max length and either truncate or show a validation message; page does not break.

AMTC_024: Verify email accepts valid special characters in local part
Steps:
1. Navigate to https://blazedemo.com/register
2. Enter a valid email using dots and plus addressing
3. Enter other valid fields
4. Click Register
Expected Result: Email is accepted as valid; no format error is shown.

AMTC_025: Verify Login page loads with all fields and elements
Steps:
1. Navigate to https://blazedemo.com/login
Expected Result: Login page loads with E-Mail Address, Password fields, Remember Me checkbox, Login button and Forgot Your Password link.

AMTC_026: Verify successful login with valid registered credentials
Steps:
1. Navigate to https://blazedemo.com/login
2. Enter registered email
3. Enter correct password
4. Click Login
Expected Result: User is logged in successfully and redirected to the home/dashboard page.

AMTC_027: Verify login fails with wrong email format
Steps:
1. Navigate to https://blazedemo.com/login
2. Enter a wrongly formatted email
3. Enter any password
4. Click Login
Expected Result: Error message for invalid email format is shown; login is not performed.

AMTC_028: Verify login fails with incorrect password
Steps:
1. Navigate to https://blazedemo.com/login
2. Enter registered email
3. Enter an incorrect password
4. Click Login
Expected Result: Error message such as invalid credentials is shown; user is not logged in.

AMTC_029: Verify login fails with unregistered email
Steps:
1. Navigate to https://blazedemo.com/login
2. Enter an email that is not registered
3. Enter any password
4. Click Login
Expected Result: Error message indicating account not found/invalid credentials is shown; user is not logged in.

AMTC_030: Verify login fails with empty email field
Steps:
1. Navigate to https://blazedemo.com/login
2. Leave email blank
3. Enter a password
4. Click Login
Expected Result: Required-field validation error is shown for email; login is not performed.

AMTC_031: Verify login fails with empty password field
Steps:
1. Navigate to https://blazedemo.com/login
2. Enter email
3. Leave password blank
4. Click Login
Expected Result: Required-field validation error is shown for password; login is not performed.

AMTC_032: Verify login fails with both fields empty
Steps:
1. Navigate to https://blazedemo.com/login
2. Leave email and password blank
3. Click Login
Expected Result: Required-field validation errors are shown for both fields; login is not performed.

AMTC_033: Verify Remember Me checkbox can be checked and unchecked
Steps:
1. Navigate to https://blazedemo.com/login
2. Click the Remember Me checkbox to check it
3. Click again to uncheck it
Expected Result: Checkbox toggles between checked and unchecked states correctly.

AMTC_034: Verify Forgot Your Password link navigates to reset page
Steps:
1. Navigate to https://blazedemo.com/login
2. Click the Forgot Your Password? link
Expected Result: User is navigated to https://blazedemo.com/password/reset (Reset Password page).

AMTC_035: Verify password field masks the entered input
Steps:
1. Navigate to https://blazedemo.com/login
2. Type a value into the Password field
Expected Result: Entered characters are masked (dots/asterisks).

AMTC_036: Verify password is treated as case-sensitive
Steps:
1. Navigate to https://blazedemo.com/login
2. Enter registered email
3. Enter password with altered case
4. Click Login
Expected Result: Login fails with invalid-credentials error (password is case-sensitive).

AMTC_037: Verify login form rejects SQL injection input
Steps:
1. Navigate to https://blazedemo.com/login
2. Enter SQL payload in email/password
3. Click Login
Expected Result: Input is sanitized; no authentication bypass occurs; login fails normally.

AMTC_038: Verify Reset Password page loads with field and button
Steps:
1. Navigate to https://blazedemo.com/password/reset
Expected Result: Reset Password page loads with E-Mail Address field and a Send Password Reset Link button.

AMTC_039: Verify reset link is sent with valid registered email
Steps:
1. Navigate to https://blazedemo.com/password/reset
2. Enter a valid registered email
3. Click Send Password Reset Link
Expected Result: Confirmation message is shown that a reset link has been sent to the email.

AMTC_040: Verify reset fails with wrong email format
Steps:
1. Navigate to https://blazedemo.com/password/reset
2. Enter a wrongly formatted email
3. Click Send Password Reset Link
Expected Result: Error message for invalid email format is shown; reset link is not sent.

AMTC_041: Verify reset fails with empty email field
Steps:
1. Navigate to https://blazedemo.com/password/reset
2. Leave email field blank
3. Click Send Password Reset Link
Expected Result: Required-field validation error is shown; reset link is not sent.

AMTC_042: Verify reset behavior with unregistered email
Steps:
1. Navigate to https://blazedemo.com/password/reset
2. Enter an unregistered but well-formatted email
3. Click Send Password Reset Link
Expected Result: Appropriate message is shown (e.g. email not found) and no reset link is sent to an invalid account.

AMTC_043: Verify home page loads with welcome content and dropdowns
Steps:
1. Navigate to https://blazedemo.com/
Expected Result: Home page loads with 'Welcome to the Simple Travel Agency!' heading, departure & destination dropdowns and a Find Flights button.

AMTC_044: Verify departure city dropdown contains all expected cities
Steps:
1. Navigate to https://blazedemo.com/
2. Open the 'Choose your departure city' dropdown
Expected Result: Dropdown lists all 7 departure cities exactly as expected.

AMTC_045: Verify destination city dropdown contains all expected cities
Steps:
1. Navigate to https://blazedemo.com/
2. Open the 'Choose your destination city' dropdown
Expected Result: Dropdown lists all 7 destination cities exactly as expected.

AMTC_046: Verify Find Flights works with default selections
Steps:
1. Navigate to https://blazedemo.com/
2. Keep default departure (Paris) and destination (Buenos Aires)
3. Click Find Flights
Expected Result: User is taken to the flight results page listing available flights from Paris to Buenos Aires.

AMTC_047: Verify Find Flights works with custom departure and destination
Steps:
1. Navigate to https://blazedemo.com/
2. Select a different departure city
3. Select a different destination city
4. Click Find Flights
Expected Result: Flight results page header reflects the selected From and To cities and lists flights.

AMTC_048: Verify behavior when departure equals destination
Steps:
1. Navigate to https://blazedemo.com/
2. Select the same value (where possible) for departure and destination
3. Click Find Flights
Expected Result: System should ideally prevent same-city selection or show an appropriate message rather than returning an invalid result.

AMTC_049: Verify 'destination of the week' link opens the vacation page
Steps:
1. Navigate to https://blazedemo.com/
2. Click 'destination of the week! The Beach!' link
Expected Result: User is navigated to https://blazedemo.com/vacation.html showing 'Destination of the week: Hawaii!' with an image.

AMTC_050: Verify top navigation links (Travel The World / home) work
Steps:
1. Navigate to https://blazedemo.com/
2. Click 'home' nav link
3. Click 'Travel The World' brand link
Expected Result: Both links navigate back to the home/index page without error.

AMTC_051: Verify flight results header shows correct From and To cities
Steps:
1. From home, select departure and destination
2. Click Find Flights
3. Observe the results page heading
Expected Result: Heading reads 'Flights from Paris to Buenos Aires:' matching the selected cities.

AMTC_052: Verify flight results table displays all expected columns
Steps:
1. Perform a flight search
2. Observe the results table columns
Expected Result: Table displays Choose, Flight #, Airline, Departs, Arrives and Price columns with flight rows.

AMTC_053: Verify Price is shown in valid currency format
Steps:
1. Perform a flight search
2. Inspect each row's Price value
Expected Result: All prices are displayed with a currency symbol and two decimal places (e.g. $472.56).

AMTC_054: Verify Flight # values are numeric
Steps:
1. Perform a flight search
2. Inspect each row's Flight # value
Expected Result: Each Flight # contains numeric values only (e.g. 43, 234, 9696).

AMTC_055: Verify 'Choose This Flight' navigates to the purchase page
Steps:
1. Perform a flight search
2. Click 'Choose This Flight' on any row
Expected Result: User is navigated to the purchase page (purchase.php) showing the reservation summary for the selected flight.

AMTC_056: Verify purchase page shows flight summary and total cost
Steps:
1. Choose a flight
2. Observe purchase page summary
Expected Result: Page shows reservation message, Airline, Flight Number, Price, Arbitrary Fees and Taxes, and a Total Cost value.

AMTC_057: Verify Total Cost equals Price plus Fees and Taxes
Steps:
1. Choose a flight
2. Note Price and Arbitrary Fees and Taxes
3. Compare with Total Cost
Expected Result: Total Cost equals Price + Arbitrary Fees and Taxes.

AMTC_058: Verify successful purchase with all valid details
Steps:
1. Choose a flight
2. Fill Name, Address, City, State, Zip Code
3. Select Card Type
4. Enter Credit Card Number, Month, Year, Name on Card
5. Click Purchase Flight
Expected Result: Purchase is processed and the confirmation page is displayed with booking details.

AMTC_059: Verify Zip Code field accepts only numeric input
Steps:
1. Choose a flight
2. Enter alphabetic/special characters in Zip Code
3. Fill other fields
4. Click Purchase Flight
Expected Result: Validation error is shown; non-numeric zip code is rejected.

AMTC_060: Verify Zip Code accepts standard 5-digit format
Steps:
1. Choose a flight
2. Enter a 5-digit zip code
3. Fill other fields
4. Click Purchase Flight
Expected Result: Valid 5-digit zip code is accepted without error.

AMTC_061: Verify Credit Card Number accepts only numeric input
Steps:
1. Choose a flight
2. Enter letters/special chars in Credit Card Number
3. Fill other fields
4. Click Purchase Flight
Expected Result: Validation error is shown; non-numeric credit card number is rejected.

AMTC_062: Verify Credit Card Number length validation
Steps:
1. Choose a flight
2. Enter a CC number that is too short (e.g. 5 digits)
3. Fill other fields
4. Click Purchase Flight
Expected Result: Validation error is shown for invalid card length (expected 15-16 digits).

AMTC_063: Verify Month field accepts only valid months (1-12)
Steps:
1. Choose a flight
2. Enter an invalid month value
3. Fill other fields
4. Click Purchase Flight
Expected Result: Validation error is shown; month outside 1-12 is rejected.

AMTC_064: Verify Month field rejects non-numeric input
Steps:
1. Choose a flight
2. Enter alphabetic characters in Month
3. Fill other fields
4. Click Purchase Flight
Expected Result: Validation error is shown; non-numeric month is rejected.

AMTC_065: Verify Year field accepts a valid 4-digit future year
Steps:
1. Choose a flight
2. Enter a valid future 4-digit year
3. Fill other fields
4. Click Purchase Flight
Expected Result: Valid 4-digit future year is accepted without error.

AMTC_066: Verify Year field rejects a past/expired year
Steps:
1. Choose a flight
2. Enter a past year in Year field
3. Fill other fields
4. Click Purchase Flight
Expected Result: Validation error is shown indicating the card is expired / year is in the past.

AMTC_067: Verify Year field rejects non-numeric input
Steps:
1. Choose a flight
2. Enter non-numeric value in Year
3. Fill other fields
4. Click Purchase Flight
Expected Result: Validation error is shown; non-numeric year is rejected.

AMTC_068: Verify Card Type dropdown lists all expected options
Steps:
1. Choose a flight
2. Open the Card Type dropdown
Expected Result: Dropdown displays all expected card types and is selectable.

AMTC_069: Verify Remember me checkbox toggles correctly
Steps:
1. Choose a flight
2. Click Remember me checkbox to check
3. Click again to uncheck
Expected Result: Checkbox toggles checked/unchecked correctly.

AMTC_070: Verify purchasing with empty mandatory fields is handled
Steps:
1. Choose a flight
2. Leave Name, Zip, Credit Card Number blank
3. Click Purchase Flight
Expected Result: Validation errors are shown for required fields; purchase is not processed.

AMTC_071: Verify Name field rejects numeric-only input
Steps:
1. Choose a flight
2. Enter only numbers in Name
3. Fill other fields
4. Click Purchase Flight
Expected Result: Validation error for invalid name is shown; purchase is not processed.

AMTC_072: Verify Credit Card Number rejects spaces and special characters
Steps:
1. Choose a flight
2. Enter CC number with spaces/special chars
3. Fill other fields
4. Click Purchase Flight
Expected Result: Validation error is shown; invalid characters are rejected.

AMTC_073: Verify confirmation page is shown after a successful purchase
Steps:
1. Complete and submit the purchase form
2. Observe the resulting page
Expected Result: Confirmation page is displayed thanking the user and showing booking details such as an Id/confirmation number.

AMTC_074: Verify confirmation page displays a unique booking Id / auth code
Steps:
1. Complete a purchase
2. Inspect the confirmation details
Expected Result: A unique booking Id (and any auth code) is generated and displayed on the confirmation page.

AMTC_075: Verify BlazeDemo brand/logo navigates to home
Steps:
1. Navigate to any BlazeDemo page
2. Click the BlazeDemo logo/brand
Expected Result: User is navigated to the home/landing page.

AMTC_076: Verify browser page title is correct
Steps:
1. Navigate to https://blazedemo.com/register (and other pages)
2. Check the browser tab title
Expected Result: Page title displays 'BlazeDemo' (or the page-specific title) correctly.

AMTC_077: Verify Login and Register links appear in the top navigation
Steps:
1. Navigate to https://blazedemo.com/login or /register
2. Observe the top-right navigation
Expected Result: Both Login and Register links are visible and navigate to their respective pages.

AMTC_078: Verify pages render correctly on mobile viewport
Steps:
1. Open the site on a mobile-width viewport
2. Navigate through Register, Login, Home pages
Expected Result: Layout is responsive; fields, buttons and nav remain usable and not broken/overlapping.

AMTC_079: Verify cross-browser compatibility
Steps:
1. Open the site in Chrome, Firefox and Edge
2. Perform core flows (search, choose flight, purchase form)
Expected Result: Core functionality and layout behave consistently across browsers.

AMTC_080: Verify browser Back button maintains correct page state
Steps:
1. Go Home > Find Flights > Choose This Flight > purchase page
2. Click the browser Back button repeatedly
Expected Result: Back button returns to the previous page in the correct state without errors.



**Your Thoughts**

**What I felt was suitable:**

* We can avoid duplicate and assumption-based test cases by using the correct prompt.
* It significantly speeds up the test case creation process. For example, I wrote 23 test cases in 2 hours, whereas AI generated around 80 test cases in under 5 minutes.

**What I felt was not suitable:**

* AI tends to create multiple test cases for a single validation scenario, leading to unnecessary duplication. For example, for email validation, it generated separate test cases for the "@" symbol, domain verification, number of dots, and other format checks. In practice, a single well-designed test case can cover all these validations, making the additional test cases redundant.
* Some generated test cases are based on assumptions rather than actual business requirements. Test cases should be derived from defined requirements and expected system behavior, not assumptions.



Final Test Case:- AI+Manual: 

----------------------- FLIGHT SEARCH / HOME ------------------------

AMTC_001: Verify "Destination of the week ! The Beach!" hypertext redirection is working correctly
Steps:
1. Go to https://blazedemo.com/
2. Click on "Destination of the week ! The Beach!" hypertext
Expected Result: It should redirect to the Destination of the week page where the destination place name and the image should show correctly

AMTC_002: Verify search flights functionality working correctly
Steps:
1. Go to https://blazedemo.com/
2. Select departure city
3. Select destination city
4. Click on find flights button
Expected Result: All flight details, Departs city name and Arrives city name should show correctly

AMTC_003: Verify departure and destination dropdowns contain all expected cities
Steps:
1. Go to https://blazedemo.com/
2. Open the "Choose your departure city" dropdown
3. Open the "Choose your destination city" dropdown
Expected Result:
1. Departure dropdown should list: Paris, Philadelphia, Boston, Portland, San Diego, Mexico City, Sao Paolo
2. Destination dropdown should list: Buenos Aires, Rome, London, Berlin, New York, Dublin, Cairo

AMTC_004: Verify search flights does not allow the same departure and destination city
Steps:
1. Go to https://blazedemo.com/
2. Select the same city for both departure and destination
3. Click on find flights button
Expected Result: It should show an error message similar to: Departure and destination city cannot be the same

AMTC_005: Verify "Travel The World" menu redirection working correctly
Steps:
1. Go to https://blazedemo.com/
2. Go to any other page
3. Click on Travel The World
Expected Result: It should redirect to the search flight page

AMTC_006: Verify "Home" menu redirection working correctly
Steps:
1. Go to https://blazedemo.com/
2. Go to any other page
3. Click on Home
Expected Result: It should redirect to the login page

------------------------- FLIGHT RESULTS ----------------------------

AMTC_007: Verify flight price is displayed in correct currency format
Steps:
1. Go to https://blazedemo.com/
2. Select departure city
3. Select destination city
4. Click on find flights button
5. Check the Price column of each flight
Expected Result: Each price should be displayed with a currency symbol and two decimal places (example: $472.56)

------------------------- PURCHASE / BOOKING ------------------------

AMTC_008: Verify purchase flight functionality working correctly
Steps:
1. Go to https://blazedemo.com/
2. Select departure city
3. Select destination city
4. Click on find flights button
5. Click on choose this flight button of any flight
6. Fill up all required fields
7. Click on purchase flight button
Expected Result:
1. It should redirect to the thank you page
2. All flight booking details should show correctly
3. For credit card number only last 4 digits should be visible

AMTC_009: Verify total cost is calculated correctly
Steps:
1. Go to https://blazedemo.com/
2. Select departure city
3. Select destination city
4. Click on find flights button
5. Click on choose this flight button of any flight
6. Check the Price, Arbitrary Fees and Taxes, and Total Cost values
Expected Result: Total Cost should be equal to Price + Arbitrary Fees and Taxes

AMTC_010: Verify card type dropdown contains all expected options
Steps:
1. Go to https://blazedemo.com/
2. Select departure city
3. Select destination city
4. Click on find flights button
5. Click on choose this flight button of any flight
6. Open the Card Type dropdown
Expected Result: Dropdown should list all expected card types: Visa, American Express, Diners Club

AMTC_011: Verify after booking a flight the flight booking ID is unique every time
Steps:
1. Go to https://blazedemo.com/
2. Select departure city, destination city and click on find flights button
3. Click on choose this flight button of any flight
4. Fill up all required fields and click on purchase flight button
5. Note the booking ID shown on the thank you page
6. Repeat the booking process and note the new booking ID
Expected Result: Each completed booking should generate a different, unique booking ID

AMTC_012: Verify in flight booking page the remember me checkbox functionality is working correctly
Steps:
1. Go to https://blazedemo.com/
2. Select departure city, destination city and click on find flights button
3. Click on choose this flight button of any flight
4. Click on the Remember me checkbox to check it
5. Click again to uncheck it
Expected Result: The Remember me checkbox should toggle between checked and unchecked states correctly

AMTC_013: Verify without entering required fields user can't book a flight
Steps:
1. Go to https://blazedemo.com/
2. Select departure city
3. Select destination city
4. Click on find flights button
5. Click on choose this flight button of any flight
6. Click on Purchase Flight button without filling up required fields
Expected Result:
1. It should show some error message similar to: Please fill up required fields to purchase your flight
2. All the required fields should have an asterisk mark on them

AMTC_014: Verify with wrong zip code format user can't purchase a flight
Steps:
1. Go to https://blazedemo.com/
2. Select departure city
3. Select destination city
4. Click on find flights button
5. Click on choose this flight button of any flight
6. Enter wrong zip code format (example: 12, tes3, test)
7. Fill up other required fields and click on Purchase Flight button
Expected Result:
1. Zip code length should be between 5-9 digits
2. With wrong zipcode submission there should be an error message similar to: Please enter the correct zipcode to purchase your flight.

AMTC_015: Verify with wrong credit card format user can't purchase a flight
Steps:
1. Go to https://blazedemo.com/
2. Select departure city
3. Select destination city
4. Click on find flights button
5. Click on choose this flight button of any flight
6. Enter wrong credit card format (example: 123 343, 1212121 212121 2121212)
7. Fill up other required fields and click on Purchase Flight button
Expected Result:
1. Credit card Number field should accept only 13-19 digits
2. With wrong credit card submission there should be an error message similar to: Please enter the correct credit card Number to purchase your flight.

AMTC_016: Verify with invalid credit card user can't purchase a flight
Steps:
1. Go to https://blazedemo.com/
2. Select departure city
3. Select destination city
4. Click on find flights button
5. Click on choose this flight button of any flight
6. Enter invalid credit card number (example: 4111 4444 4444 4444)
7. Fill up other required fields and click on Purchase Flight button
Expected Result: With invalid credit card number there should be an error message similar to: Invalid card, please enter a valid card to purchase your flight.

AMTC_017: Verify with wrong month field format user can't purchase a flight
Steps:
1. Go to https://blazedemo.com/
2. Select departure city
3. Select destination city
4. Click on find flights button
5. Click on choose this flight button of any flight
6. Enter wrong month format (example: 13, test)
7. Fill up other required fields and click on Purchase Flight button
Expected Result:
1. Month format should be 1-12 only
2. With wrong month format submission there should be an error message similar to: Please enter the correct month to purchase your flight.

AMTC_018: Verify with wrong year field format user can't purchase a flight
Steps:
1. Go to https://blazedemo.com/
2. Select departure city
3. Select destination city
4. Click on find flights button
5. Click on choose this flight button of any flight
6. Enter wrong year format (example: 123, tes3, test)
7. Fill up other required fields and click on Purchase Flight button
Expected Result: With wrong year format submission there should be an error message similar to: Please enter the correct year to purchase your flight.

AMTC_019: Verify user can't purchase a flight with an expired card
Steps:
1. Go to https://blazedemo.com/
2. Select departure city
3. Select destination city
4. Click on find flights button
5. Click on choose this flight button of any flight
6. Enter month and year as already expired (example: month: 12, year: 2020)
7. Fill up other required fields and click on Purchase Flight button
Expected Result: With expired card submission there should be an error message similar to: Your card is expired, please enter another card details.

------------------------------ LOGIN --------------------------------

AMTC_020: Verify login working correctly
Steps:
1. Go to https://blazedemo.com/login
2. Enter registered email address
3. Enter password
4. Click on login
Expected Result: User should login successfully

AMTC_021: Verify login is not working with invalid credential
Steps:
1. Go to https://blazedemo.com/login
2. Enter non-registered email address
3. Enter password
4. Click on login
Expected Result: There should be an error message: invalid credentials

AMTC_022: Verify login is not working with wrong email format
Steps:
1. Go to https://blazedemo.com/login
2. Enter wrong email address format (example: test@)
3. Enter password
4. Click on login
Expected Result: There should be an error message: invalid credentials

AMTC_023: Verify login is not working without filling up required fields
Steps:
1. Go to https://blazedemo.com/login
2. Click on login button without entering email and password
Expected Result: There should be an error message: Missing required fields

AMTC_024: Verify remember me checkbox on login page works correctly
Steps:
1. Go to https://blazedemo.com/login
2. Click on the Remember Me checkbox to check it
3. Click again to uncheck it
Expected Result: The Remember Me checkbox should toggle between checked and unchecked states correctly

-------------------------- FORGOT PASSWORD --------------------------

AMTC_025: Verify forgot password is working correctly
Steps:
1. Go to https://blazedemo.com/login
2. Click on "Forgot your password?" hyperlink
3. Enter registered email address
4. Click on Send password reset link
Expected Result: It should redirect to the next page of the forgot password process

AMTC_026: Verify user can't use forgot password with wrong email format
Steps:
1. Go to https://blazedemo.com/login
2. Click on "Forgot your password?" hyperlink
3. Enter wrong email format (example: test@)
4. Click on Send password reset link
Expected Result: It should show some error message, example: wrong email format

AMTC_027: Verify forgot password is not working with non-registered email address
Steps:
1. Go to https://blazedemo.com/login
2. Click on "Forgot your password?" hyperlink
3. Enter non-registered email address
4. Click on Send password reset link
Expected Result: It should show some error message, example: email not registered

AMTC_028: Verify forgot password is not working with empty email field
Steps:
1. Go to https://blazedemo.com/login
2. Click on "Forgot your password?" hyperlink
3. Leave the email field blank
4. Click on Send password reset link
Expected Result: It should show some error message, example: email field is required

----------------------------- REGISTRATION --------------------------

AMTC_029: Verify registration is working correctly
Steps:
1. Go to https://blazedemo.com/register
2. Enter required fields
3. Click on register button
Expected Result: It should register the user

AMTC_030: Verify registration is not working with duplicate email id
Steps:
1. Go to https://blazedemo.com/register
2. Enter an email which is already registered
3. Enter other required fields
4. Click on register button
Expected Result: It should show error message, example: duplicate email

AMTC_031: Verify registration is not working with wrong email format
Steps:
1. Go to https://blazedemo.com/register
2. Enter wrong email format in email address field (example: test@)
3. Enter other required fields
4. Click on register button
Expected Result: It should show error message, example: wrong email format

AMTC_032: Verify registration is not working when password and confirm password fields do not match
Steps:
1. Go to https://blazedemo.com/register
2. Enter different values in password and confirm password fields
3. Enter other required fields
4. Click on register button
Expected Result: It should show error message, example: password and confirm password do not match

AMTC_033: Verify registration is not working without filling up required fields
Steps:
1. Go to https://blazedemo.com/register
2. Click on register button without entering required fields
Expected Result: It should show error message, example: required fields are missing

AMTC_034: Verify registration is not working with a weak/short password
Steps:
1. Go to https://blazedemo.com/register
2. Enter a password below the minimum length (example: 123) in both password and confirm password
3. Enter other required fields
4. Click on register button
Expected Result: It should show error message, example: password must be at least the minimum required length

AMTC_035: Verify registration is working when the optional Company field is left blank
Steps:
1. Go to https://blazedemo.com/register
2. Enter Name, Email, Password and Confirm Password
3. Leave the Company field blank
4. Click on register button
Expected Result: It should register the user successfully (Company is an optional field)

