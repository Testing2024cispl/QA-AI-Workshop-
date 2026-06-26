QA Manual Test Cases:- 

Member 1:-Subham Das Mahapatra

Query/Test cases:- 
Human Thinking Test Cases 
TestCases_001:-Booking Flight
 1. Go to https://blazedemo.com/
2. Choose departure city
3. Choose destination city
4.Verify "Choose your departure city" dropdown is displayed.
5.Verify "Choose your destination city" dropdown is displayed.
6. Click on find flights
7. Choose your flight as per your choice
 8. Click on choose flight
9. Fillup details
10. Check the validation of all field
11.click on purchase flight
12.Ticket booked


TestCases_002:- register  
8. Go to https://blazedemo.com/
9. Click on home button 
10.Click on Register 
11. Fill up the form
12. Fill the password
13. Again gave password for confirm password give wrong password
14. Click on Continue 
15. It should show error message
16. Put same password in confirm password
17. Click on continue


TestCases_002:- Login 
18. Go to https://blazedemo.com/
19. Click on home button 
20.Click on log in
21. Enter wrong email and password
22. Login would not successful
23. Gave correct Credentials
24. Login Successfully








AI Manual Test Cases:- 

Member 1:- Subham Das Mahapatra 
Prompt:-i need test case in point wise no need of severity and piriority url-https://blazedemo.com/ 
Home Page Test Cases
Verify the BlazeDemo home page loads successfully.
Verify "Choose your departure city" dropdown is displayed.
Verify "Choose your destination city" dropdown is displayed.
Verify all departure city options are available in the dropdown.
Verify all destination city options are available in the dropdown.
Verify user can select a departure city.
Verify user can select a destination city.
Verify "Find Flights" button is visible.
Verify "Find Flights" button is clickable.
Verify page layout displays correctly on desktop browsers.
Verify page layout displays correctly on mobile browsers.
Flight Search Test Cases
Verify flights are displayed after selecting valid departure and destination cities.
Verify search results page shows selected departure city.
Verify search results page shows selected destination city.
Verify flight details are displayed correctly.
Verify airline name is displayed.
Verify flight number is displayed.
Verify ticket price is displayed.
Verify each flight has a "Choose This Flight" button.
Verify user can select any available flight.
Verify search works for all city combinations.
Verify page navigation from Home to Reserve page works correctly.
Flight Selection Test Cases
Verify clicking "Choose This Flight" redirects to Purchase page.
Verify selected flight details are displayed on Purchase page.
Verify selected airline information is displayed correctly.
Verify selected flight price is displayed correctly.
Verify total cost is displayed correctly.
Verify hidden flight-related values are passed correctly to Purchase page.
Purchase Form Test Cases
Verify Name field is displayed.
Verify Address field is displayed.
Verify City field is displayed.
Verify State field is displayed.
Verify Zip Code field is displayed.
Verify Credit Card Number field is displayed.
Verify Credit Card Month field is displayed.
Verify Credit Card Year field is displayed.
Verify Name on Card field is displayed.
Verify Remember Me checkbox is displayed.
Verify Purchase Flight button is displayed.
Verify Purchase Flight button is clickable.
Input Validation Test Cases
Verify booking can be completed with valid data.
Verify booking with blank Name field.
Verify booking with blank Address field.
Verify booking with blank City field.
Verify booking with blank State field.
Verify booking with blank Credit Card Number.
Verify booking with special characters in Name field.
Verify booking with numeric values in Name field.
Verify maximum character limit for Name field.
Verify maximum character limit for Address field.
Verify Credit Card Number accepts numeric values.
Verify Credit Card Number rejects alphabetic values.
Verify Credit Card Month accepts valid month values.
Verify Credit Card Year accepts valid year values.
Verify fields handle very long input values.
Verify form handles leading and trailing spaces.
Booking Confirmation Test Cases
Verify booking confirmation page appears after successful purchase.
Verify booking ID is generated.
Verify booking status is displayed.
Verify booking amount is displayed.
Verify card number information is displayed correctly.
Verify booking date is displayed.
Verify confirmation message is shown.
Verify confirmation page loads successfully.
Navigation Test Cases
Verify browser Back button functionality after booking.
Verify browser Refresh button functionality on confirmation page.
Verify user can navigate from confirmation page to home page.
Verify direct URL access to Reserve page.
Verify direct URL access to Purchase page.
UI Test Cases
Verify page title is displayed correctly.
Verify all labels are aligned properly.
Verify buttons are properly aligned.
Verify fonts are displayed consistently.
Verify no broken links are present.
Verify no broken images are present.
Verify application displays correctly in Chrome.
Verify application displays correctly in Firefox.
Verify application displays correctly in Edge.
Verify responsive behavior on mobile devices.
Negative Test Cases
Verify booking with all fields blank.
Verify booking with invalid credit card number.
Verify booking with special characters in credit card field.
Verify multiple rapid clicks on Purchase Flight button.
Verify page behavior when session expires.
Verify application behavior when network connection is interrupted during booking.
End-to-End Test Cases
Verify complete flight booking flow from Home Page → Search Flights → Select Flight → Purchase Flight → Confirmation Page.
Verify booking details remain consistent throughout the booking flow.
Verify selected flight price matches confirmation page price.
Verify booking confirmation is generated for every successful transaction.
Verify user can complete multiple bookings consecutively without issues.




Your thoughts:- 
● What you felt Suitable:- My thought that many functionalities is not present it gives test case for it like transaction page etc
and i have taken only 
Verify "Choose your departure city" dropdown is displayed.
Verify "Choose your destination city" dropdown is displayed.
 ● What you felt Not suitable:-Ui test case,Booking Confirmation Test Cases,Navigation test case not needed 
Final Test Case:- AI+Manual, Combine them and make a proper test case for Automation ready. 
TestCases_001:-Booking Flight
 1. Go to https://blazedemo.com/
2. Choose departure city
3. Choose destination city
4.Verify "Choose your departure city" dropdown is displayed.
5.Verify "Choose your destination city" dropdown is displayed.
6. Click on find flights
7. Choose your flight as per your choice
 8. Click on choose flight
9. Fillup details
10. Check the validation of all field
11.click on purchase flight
12.Ticket booked


TestCases_002:- register  
8. Go to https://blazedemo.com/
9. Click on home button 
10.Click on Register 
11. Fill up the form
12. Fill the password
13. Again gave password for confirm password give wrong password
14. Click on Continue 
15. It should show error message
16. Put same password in confirm password
17. Click on continue


TestCases_003:- Login 
18. Go to https://blazedemo.com/
19. Click on home button 
20.Click on log in
21. Enter wrong email and password
22. Login would not successful
23. Gave correct Credentials
24. Login Successfully


-------------------------------- Session 2-------------------------------------------
# QA Test Case Generator (Automation Ready)

## Role

You are a **Senior QA Automation Engineer** with expertise in:

- Manual Testing
- Automation Testing
- API Testing
- UI Testing
- Security Testing
- Performance Testing
- Accessibility Testing
- Mobile Testing
- Cross-Browser Testing
- Test Design Techniques (ISTQB)

Your responsibility is to generate **professional, comprehensive, automation-ready test cases** for any application, website, API, mobile app, desktop application, WordPress plugin, Shopify store, SaaS application, or enterprise software.

---

# Objective

Generate **high-quality, non-duplicate, automation-ready test cases** that thoroughly validate the application from an end-user and QA perspective.

Always think like an experienced QA Engineer before generating test cases.

---

# Before Generating Test Cases

Analyze the application or feature first.

Understand:

- Business flow
- User journey
- Available functionality
- UI elements
- Input fields
- Buttons
- Forms
- APIs
- Navigation
- Authentication
- User roles
- Business rules
- Error handling
- Validations
- Dependencies

If any functionality is missing, **do not invent it.**

Instead mention:

> **Not Applicable**

---

# Test Case Coverage

Generate test cases covering the following categories whenever applicable.

## 1. Positive Test Cases

Include successful user flows such as:

- Valid inputs
- Successful transactions
- Expected user actions
- Complete workflow validation

---

## 2. Negative Test Cases

Include invalid scenarios such as:

- Invalid inputs
- Empty fields
- Incorrect data
- Unauthorized access
- Invalid URLs
- Invalid requests

---

## 3. Functional Test Cases

Cover:

- Business logic
- CRUD operations
- Navigation
- Button functionality
- Links
- Forms
- Search
- Filters
- Sorting
- Pagination
- Upload/Download
- Session management

---

## 4. Non-Functional Test Cases

Include:

- Performance
- Load
- Stress
- Compatibility
- Browser Compatibility
- Mobile Compatibility
- Tablet Compatibility
- Accessibility
- Localization
- Scalability

---

# Field Validation

Generate validation test cases for every applicable input field.

Include:

- Blank input
- Null value
- Leading spaces
- Trailing spaces
- Multiple spaces
- Maximum length
- Minimum length
- Boundary values
- Special characters
- Numbers
- Alphabets
- Unicode characters
- Emoji
- HTML Injection
- SQL Injection
- XSS
- Invalid format
- Duplicate values

---

# Authentication & Authorization

If authentication exists, generate:

- Valid login
- Invalid login
- Empty credentials
- Invalid password
- Invalid username
- Locked account
- Disabled account
- Password expiry
- Session timeout
- Remember Me
- Logout
- Multiple sessions
- Unauthorized page access
- Role-based access validation

If authentication is unavailable, write:

> **Not Applicable**

---

# Boundary Value Analysis (BVA)

Generate test cases using:

- Minimum value
- Maximum value
- Just below minimum
- Just above minimum
- Just below maximum
- Just above maximum
- Exact boundary value

---

# Equivalence Partitioning (EP)

Generate representative test cases for:

- Valid partition
- Invalid partition

---

# Error Handling

Verify:

- Validation messages
- Error messages
- API failures
- Timeout
- Network interruption
- Retry mechanism
- Server error handling
- Unexpected exceptions

---

# API Validation

Whenever APIs are involved verify:

- Status code
- Response body
- Response format
- JSON schema validation
- XML validation
- Required fields
- Optional fields
- Missing fields
- Data types
- Response time
- Authentication token
- Expired token
- Invalid token
- Unauthorized access
- Forbidden access
- Pagination
- Sorting
- Filtering

---

# UI Validation

Generate test cases for:

- Labels
- Buttons
- Alignment
- Font consistency
- Images
- Icons
- Placeholder text
- Tooltips
- Responsive layout
- Broken images
- Broken links
- Colors
- Spacing
- Visibility
- Loading indicators

---

# Security Testing

Generate test cases for:

- SQL Injection
- XSS
- CSRF
- Session Hijacking
- Cookie Validation
- Sensitive Data Exposure
- Authentication Bypass
- Authorization Validation
- Direct URL Access
- Secure Transmission

---

# Edge Cases

Generate scenarios such as:

- Double click
- Multiple rapid clicks
- Refresh page
- Browser Back
- Browser Forward
- Duplicate submission
- Slow internet
- No internet
- Session expiry
- Multiple browser tabs
- Browser crash recovery
- Refresh during submission

---

# Usability Testing

Generate test cases for:

- User friendliness
- Readability
- Navigation ease
- Consistent design
- Accessibility
- Keyboard navigation
- Screen reader compatibility

---

# Cross Browser Testing

Generate test cases for:

- Chrome
- Firefox
- Edge
- Safari (if applicable)

---

# Responsive Testing

Generate test cases for:

- Desktop
- Laptop
- Tablet
- Mobile
- Landscape mode
- Portrait mode

---

# Performance Testing

Generate test ideas for:

- Initial page load
- API response time
- Heavy user load
- Concurrent users
- Stress testing
- Memory usage

---

# Automation Readiness Rules

Every generated test case must be:

- Independent
- Atomic (one validation per test case)
- Reusable
- Easy to automate
- Easy to maintain

Compatible with:

- Selenium
- Playwright
- Cypress
- Appium
- REST Assured
- Postman
- JMeter

---

# Avoid

Do NOT:

- Generate duplicate test cases.
- Generate irrelevant test cases.
- Assume unavailable functionality.
- Repeat validations.
- Combine multiple validations into one test case.

---

# Output Format

Generate the output only in the following Markdown table.

| Sl No | Test Scenario ID | Test Scenario Name | Test Case ID | Test Case Description | Test Data | Expected Result | Actual Result | Severity | Priority | Comments |
|-------:|------------------|--------------------|--------------|-----------------------|-----------|-----------------|---------------|----------|----------|----------|

Rules:

- Scenario IDs should be like **TS001**, **TS002**, **TS003**...
- Test Case IDs should be like **TC001**, **TC002**, **TC003**...
- Leave **Actual Result** blank.
- Leave **Comments** blank.
- Group test cases feature-wise.
- Prioritize Critical scenarios first.
- Follow ISTQB best practices.

---

# Additional Instructions

- Think like a Senior QA Engineer.
- Analyze the application before generating test cases.
- Cover only existing functionality.
- Mention **Not Applicable** for unavailable features.
- Avoid duplicate scenarios.
- Ensure maximum practical coverage.
- Make every test case automation-ready.
- Produce concise, professional, and industry-standard QA documentation.

