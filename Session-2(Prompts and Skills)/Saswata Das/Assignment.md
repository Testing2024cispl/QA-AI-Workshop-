Member 1:-Saswata Das
Query/Test cases:- https://www.saucedemo.com/

## Manual Human Thinking Test Cases

TestCases_001:-

1. Open https://www.saucedemo.com
2. Login with valid credentials
3. Navigate to Inventory page
4. Verify all products are displayed
5. Verify each product has Name, Description and Price
6. Verify each product has Add to Cart button
7. Add one product to cart
8. Verify Remove button replaces Add to Cart button

TestCases_002:-

1. Login to SauceDemo
2. Add Sauce Labs Backpack to cart
3. Open Cart page
4. Verify selected product appears in cart
5. Verify quantity is displayed as 1
6. Verify price matches inventory page
7. Verify Checkout button is enabled

TestCases_003:-

1. Login to SauceDemo
2. Add multiple products
3. Open Cart page
4. Click Continue Shopping
5. Verify user returns to Inventory page
6. Verify previously selected products remain in cart

TestCases_004:-

1. Login to SauceDemo
2. Add multiple products
3. Open Cart page
4. Remove one product
5. Verify only selected product is removed
6. Verify remaining products stay in cart

TestCases_005:-

1. Login to SauceDemo
2. Add products
3. Open Cart page
4. Remove all products
5. Verify cart becomes empty
6. Verify checkout cannot proceed with empty cart

TestCases_006:-

1. Add products to cart
2. Open Cart page
3. Click Checkout
4. Leave all fields blank
5. Click Continue
6. Verify validation message is displayed

TestCases_007:-

1. Add product to cart
2. Open Checkout Information page
3. Leave First Name blank
4. Enter Last Name and Zip Code
5. Click Continue
6. Verify proper error message appears

TestCases_008:-

1. Add product to cart
2. Open Checkout Information page
3. Enter First Name
4. Leave Last Name blank
5. Enter Zip Code
6. Click Continue
7. Verify validation message appears

TestCases_009:-

1. Add product to cart
2. Open Checkout Information page
3. Enter First Name
4. Enter Last Name
5. Leave Zip Code blank
6. Click Continue
7. Verify validation message appears

TestCases_010:-

1. Add products to cart
2. Enter valid checkout information
3. Click Continue
4. Verify Checkout Overview page opens
5. Verify product names are correct
6. Verify quantity is correct
7. Verify total price calculation is correct

## AI Generated Test Case

TC_AI_001:-

1. Login with valid user credentials
2. Add multiple products to cart
3. Open Cart page
4. Proceed to Checkout
5. Enter valid customer information
6. Continue to Overview page
7. Verify Payment Information section
8. Verify Shipping Information section
9. Verify Item Total
10. Verify Tax Amount
11. Verify Total Amount
12. Click Finish
13. Verify successful order confirmation

Why suitable:-

* Covers complete end-to-end purchase flow.
* Verifies cart functionality.
* Verifies checkout validation.
* Covers order overview calculations.
* Easy to automate using Playwright.
* Reusable in regression testing.

● Why Not Suitable:-

* AI missed field-level validation scenarios.
* AI did not consider empty cart behavior.
* AI did not verify cart persistence.
* AI did not verify removal of products.
* AI focused mainly on happy path.


Final Test Case (AI + Human Combined) Automation Ready
----------------

TC_FINAL_001:- Verify Successful Product Purchase Flow

Preconditions:

1. User is registered.
2. User has valid credentials.
3. SauceDemo application is accessible.

Test Steps:

1. Launch SauceDemo application.
2. Login using valid username and password.
3. Verify Inventory page loads successfully.
4. Verify all products display Name, Description and Price.
5. Add Sauce Labs Backpack to cart.
6. Add Sauce Labs Bike Light to cart.
7. Verify cart badge count becomes 2.
8. Open Cart page.
9. Verify both products appear in cart.
10. Verify product quantity is displayed correctly.
11. Verify product prices match inventory page.
12. Click Checkout.
13. Verify Checkout Information page opens.
14. Enter valid First Name.
15. Enter valid Last Name.
16. Enter valid Zip Code.
17. Click Continue.
18. Verify Checkout Overview page opens.
19. Verify selected products are displayed.
20. Verify quantity is correct.
21. Verify Payment Information section is displayed.
22. Verify Shipping Information section is displayed.
23. Verify Item Total calculation is correct.
24. Verify Tax calculation is displayed.
25. Verify Final Total calculation is correct.
26. Click Finish.
27. Verify order confirmation page appears.
28. Verify success message is displayed.
29. Click Back Home.
30. Verify user is redirected to Inventory page.

Expected Result:

* User should successfully complete purchase.
* Product information should remain consistent across pages.
* Cart quantity should be accurate.
* Checkout validation should work correctly.
* Overview calculations should be accurate.
* Order should be created successfully.
* User should return to Inventory page after clicking Back Home.

=======================================================================================================
Day 2 assignment
# QA Test Case Generator Skill

## Role
Act as a Senior QA Engineer with expertise in Manual Testing, API Testing, and Test Automation.

## Objective
Generate comprehensive, unique, and automation-ready test cases for the given application, feature, user story, requirement, or API.

## Coverage
- Positive Scenarios
- Negative Scenarios
- Functional Testing
- Non-Functional Testing
- Edge Cases
- Boundary Value Analysis (BVA)
- Field Validation
- Authentication & Authorization
- Error Handling
- Usability
- Security Functional Checks
- API Validation (if applicable)

## Validation Checklist
Cover wherever applicable:
- Mandatory & Optional fields
- Input/Data type validation
- Min/Max length
- Boundary values
- Invalid, empty and null inputs
- Special characters
- SQL Injection
- Cross-Site Scripting (XSS)
- Authentication & Authorization
- Session validation
- Duplicate data
- Error messages
- API status codes
- Response body, schema & headers
- Response time
- Data consistency
- Database validation
- Accessibility
- Cross-browser compatibility
- Responsive UI
- Performance-related functional checks

## API Checks
Include verification for:
- HTTP Method
- Endpoint
- Request Headers
- Request Body
- Authentication
- Status Code
- Response Body
- Response Schema
- Response Headers
- Response Time
- Error Responses
- Invalid Payload
- Missing Parameters
- Authorization Failure
- Data Integrity

## Output Requirements
- Generate only unique test cases.
- Avoid duplicate or overlapping scenarios.
- Use clear QA language.
- Make every test case independent.
- Make test cases automation-ready.
- One validation objective per test case.
- Include positive and negative scenarios.
- Use realistic test data.
- Expected Result must be measurable and verifiable.

## Output Table

| Sl No | Test Scenario ID | Test Scenario Name | Test Case ID | Test Case Description | Test Data | Expected Result | Actual Result | Severity | Priority | Comments |
|-------|------------------|--------------------|--------------|----------------------|-----------|-----------------|---------------|----------|----------|----------|

## Severity
- Critical
- High
- Medium
- Low

## Priority
- P1
- P2
- P3
- P4

## Naming Convention
Scenario IDs:
- TS_001
- TS_002
- TS_003

Test Case IDs:
- TC_001
- TC_002
- TC_003

## Quality Rules
Each test case must:
- Be atomic (one validation only)
- Be independent
- Be reusable
- Be automation-friendly
- Have clear expected results
- Use consistent naming
- Avoid duplicate coverage
- Follow industry QA standards

## Final Instruction
Generate all applicable test cases based on the provided feature or requirement. Ensure maximum functional coverage with no duplicate test cases. Organize related test cases under appropriate test scenarios and present the final output in the specified table format.
