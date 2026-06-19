📝 QA Manual Test Cases for Swag Labs

Member 1:-Antara Roy Ghosh

Query/Test cases:- https://www.saucedemo.com/  
TestCase_001: Verify login with valid credentials
Test Steps:
Step 1- Open https://www.saucedemo.com/
Step 2- Enter valid username
Step 3- Enter valid password
Step 4- Click Login button
TestCase_002: Verify login with invalid credentials
Test Steps:
Step 1- Open the application
Step 2- Enter invalid username or password
Step 3- Click Login button
Step 4- Verify login is unsuccessful
TestCase_003: Verify products are displayed after successful login
Test Steps:
Step 1- Login with valid credentials
Step 2- Navigate to Products page
Step 3- Observe product list
Step 4- Verify product information
TestCase_004: Verify product details page
Test Steps:
Step 1- Login successfully
Step 2- Click on a product name
Step 3- Open product details page
Step 4- Verify product information
TestCase_005: Verify filter Name (A to Z)
Test Steps:
Step 1- Login successfully
Step 2- Click filter dropdown
Step 3- Select Name (A to Z)
Step 4- Verify product sorting order
TestCase_006: Verify filter Name (Z to A)
Test Steps:
Step 1- Login successfully
Step 2- Click filter dropdown
Step 3- Select Name (Z to A)
Step 4- Verify product sorting order
TestCase_007: Verify filter Price (Low to High)
Test Steps:
Step 1- Login successfully
Step 2- Click filter dropdown
Step 3- Select Price (Low to High)
Step 4- Verify product sorting order
TestCase_008: Verify filter Price (High to Low)
Test Steps:
Step 1- Login successfully
Step 2- Click filter dropdown
Step 3- Select Price (High to Low)
Step 4- Verify product sorting order
TestCase_009: Verify add single product to cart
Test Steps:
Step 1- Login successfully
Step 2- Select a product
Step 3- Click Add to Cart
Step 4- Verify cart badge count
TestCase_010: Verify add multiple products to cart
Test Steps:
Step 1- Login successfully
Step 2- Add multiple products
Step 3- Open cart page
Step 4- Verify all products are added
TestCase_011: Verify remove product from Cart page
Test Steps:
Step 1- Add product to cart
Step 2- Navigate to cart
Step 3- Click Remove button
Step 4- Verify product is removed
TestCase_012: Verify cart page displays selected products
Test Steps:
Step 1- Add products to cart
Step 2- Open cart page
Step 3- Review product list
Step 4- Verify product details
TestCase_013: Verify Continue Shopping functionality
Test Steps:
Step 1- Add product to cart
Step 2- Open cart page
Step 3- Click Continue Shopping
Step 4- Verify navigation to Products page
TestCase_014: Verify Checkout button functionality
Test Steps:
Step 1- Add product to cart
Step 2- Open Cart page
Step 3- Click Checkout
Step 4- Verify Checkout Information page opens
TestCase_015: Verify checkout with valid customer information
Test Steps:
Step 1- Enter First Name
Step 2- Enter Last Name
Step 3- Enter Zip/Postal Code
Step 4- Click Continue
TestCase_016: Verify Cancel button on Checkout Information page
Test Steps:
Step 1- Open Checkout Information page
Step 2- Click Cancel
Step 3- Observe navigation
Step 4- Verify Cart page is displayed
TestCase_017: Verify Checkout Overview page details
Test Steps:
Step 1- Complete Checkout Information
Step 2- Open Overview page
Step 3- Review products and pricing
Step 4- Verify subtotal, tax and total amount
TestCase_018: Verify Finish button functionality
Test Steps:
Step 1- Open Checkout Overview page
Step 2- Review order information
Step 3- Click Finish
Step 4- Verify order is completed successfully
TestCase_019: Verify successful order completion and Back Home functionality
Test Steps:
Step 1- Complete purchase successfully
Step 2- Verify confirmation page
Step 3- Click Back Home button
Step 4- Verify user is redirected to Products page
—----------------------------------------------------------------------------------------------------------------------------
—----------------------------------------------------------------------------------------------------------------------------

AI Manual Test Cases:- 
Member :-Antara Roy Ghosh


Prompt Given:- 

Write test cases for https://www.saucedemo.com/ 
Task Requirements:
Generate test cases for the Swag labs web application. Cover all the major functionalities including User Login,product browsing, filter product,add to cart,remove product from the cart,continue shopping,checkout details, shopping completed.
Test Objective
Validate the complete end-to-end user journey and ensure all functionalities work correctly.
Test Scope
Login
Product Browsing
Product Filtering
Add to Cart
Remove from Cart
Continue Shopping
Checkout Information
Checkout Overview
Order Completion
Validation & Error Handling
Test Coverage
Include:
Positive Test Cases
Negative Test Cases
Validation Scenarios
Error Handling Scenarios
End-to-End Functional Testing
Output Format:
TestCase_ID: Test Scenario
Test Steps:
Step 1
Step 2
Step 3
Expected Results:
Severity:
Priority:

TestCase_ID: TC_LOGIN_001 - Verify login with valid credentials
Test Steps:
Step 1: Open https://www.saucedemo.com/
Step 2: Enter valid username and password
Step 3: Click Login
Expected Results:
Users should be redirected to the Products page successfully.
Severity: Critical
Priority: High

TestCase_ID: TC_LOGIN_002 - Verify login with invalid username
Test Steps:
Step 1: Open the application
Step 2: Enter invalid username
Step 3: Enter valid password and click Login
Expected Results:
Appropriate error message should be displayed and login should fail.
Severity: High
Priority: High

TestCase_ID: TC_LOGIN_003 - Verify login with blank username
Test Steps:
Step 1: Leave username field blank
Step 2: Enter password
Step 3: Click Login
Expected Results:
Username required validation message should be displayed.
Severity: Medium
Priority: High

TestCase_ID: TC_PRODUCT_001 - Verify products are displayed after login
Test Steps:
Step 1: Login successfully
Step 2: Navigate to Products page
Step 3: Observe product listing
Expected Results:
All products should be displayed with image, name, description and price.
Severity: High
Priority: High

TestCase_ID: TC_FILTER_001 - Verify Name (A to Z) sorting
Test Steps:
Step 1: Login successfully
Step 2: Select "Name (A to Z)" filter
Step 3: Verify displayed products
Expected Results:
Products should be sorted alphabetically in ascending order.
Severity: Medium
Priority: Medium

TestCase_ID: TC_FILTER_002 - Verify Price (Low to High) sorting
Test Steps:
Step 1: Login successfully
Step 2: Select "Price (Low to High)"
Step 3: Verify product prices
Expected Results:
Products should be sorted from lowest to highest price.
Severity: Medium
Priority: Medium

TestCase_ID: TC_CART_001 - Verify add product to cart
Test Steps:
Step 1: Login successfully
Step 2: Click Add to Cart for a product
Step 3: Check cart badge
Expected Results:
Selected product should be added to cart and cart count should increase.
Severity: Critical
Priority: High

TestCase_ID: TC_CART_002 - Verify add multiple products to cart
Test Steps:
Step 1: Login successfully
Step 2: Add multiple products
Step 3: Open cart page
Expected Results:
All selected products should be present in cart.
Severity: Critical
Priority: High

TestCase_ID: TC_CART_003 - Verify remove product from cart
Test Steps:
Step 1: Add product to cart
Step 2: Navigate to cart
Step 3: Click Remove button
Expected Results:
Product should be removed from cart successfully.
Severity: High
Priority: High

TestCase_ID: TC_CART_004 - Verify cart badge update after removing product
Test Steps:
Step 1: Add product to cart
Step 2: Remove product
Step 3: Verify cart badge
Expected Results:
Cart count should decrease accordingly.
Severity: Medium
Priority: Medium

TestCase_ID: TC_CART_005 - Verify Continue Shopping button
Test Steps:
Step 1: Add product to cart
Step 2: Open cart page
Step 3: Click Continue Shopping
Expected Results:
User should be redirected to Products page.
Severity: Medium
Priority: Medium

TestCase_ID: TC_CHECKOUT_001 - Verify checkout with valid information
Test Steps:
Step 1: Add product to cart
Step 2: Click Checkout
Step 3: Enter valid First Name, Last Name and Zip Code
Step 4: Click Continue
Expected Results:
User should navigate to Checkout Overview page.
Severity: Critical
Priority: High

TestCase_ID: TC_CHECKOUT_002 - Verify checkout with blank First Name
Test Steps:
Step 1: Open Checkout Information page
Step 2: Leave First Name blank
Step 3: Click Continue
Expected Results:
First Name required validation message should be displayed.
Severity: Medium
Priority: High

TestCase_ID: TC_CHECKOUT_003 - Verify checkout with blank Last Name
Test Steps:
Step 1: Leave Last Name blank
Step 2: Enter remaining details
Step 3: Click Continue
Expected Results:
Last Name required validation message should be displayed.
Severity: Medium
Priority: High

TestCase_ID: TC_CHECKOUT_004 - Verify checkout with blank Zip Code
Test Steps:
Step 1: Leave Zip Code blank
Step 2: Click Continue
Step 3: Observe validation
Expected Results:
Zip Code required validation message should be displayed.
Severity: Medium
Priority: High

TestCase_ID: TC_CHECKOUT_005 - Verify Cancel button on Checkout Information page
Test Steps:
Step 1: Open Checkout Information page
Step 2: Click Cancel
Step 3: Verify redirection
Expected Results:
User should be redirected back to Cart page.
Severity: Low
Priority: Medium

TestCase_ID: TC_OVERVIEW_001 - Verify Checkout Overview page
Test Steps:
Step 1: Complete Checkout Information
Step 2: Open Overview page
Step 3: Verify order details
Expected Results:
Product details, subtotal, tax and total amount should be displayed correctly.
Severity: High
Priority: High

TestCase_ID: TC_OVERVIEW_002 - Verify Finish button functionality
Test Steps:
Step 1: Reach Checkout Overview page
Step 2: Click Finish
Step 3: Observe confirmation page
Expected Results:
Order should be completed successfully.
Severity: Critical
Priority: High

TestCase_ID: TC_COMPLETE_001 - Verify order completion message
Test Steps:
Step 1: Complete checkout process
Step 2: Reach confirmation page
Step 3: Verify confirmation message
Expected Results:
Order confirmation message should be displayed.
Severity: High
Priority: High

TestCase_ID: TC_COMPLETE_002 - Verify Back Home button
Test Steps:
Step 1: Complete order
Step 2: Click Back Home
Step 3: Verify navigation
Expected Results:
User should return to Products page.
Severity: Medium
Priority: Medium

TestCase_ID: TC_E2E_001 - Verify complete end-to-end purchase flow
Test Steps:
Step 1: Login with valid credentials
Step 2: Apply product filter
Step 3: Add products to cart
Step 4: Remove one product
Step 5: Continue Shopping
Step 6: Add another product
Step 7: Proceed to Checkout
Step 8: Enter valid checkout information
Step 9: Verify Checkout Overview
Step 10: Click Finish
Expected Results:
User should successfully complete the purchase and view the order confirmation page.
Severity: Critical
Priority: High
Your thoughts:- 
● What you felt Suitable:-  
● What you felt Not suitable:- 
Final Test Case:- 
AI+Manual, Combine them and make a proper test case 
for Automation ready. 

My thoughts:- 

What I felt Suitable:
AI covered all major modules such as Login, Product Browsing, Product Filtering, Cart, Checkout, and Order Completion.
Test cases followed a structured format with Test Steps, Expected Results, Severity, and Priority.
Positive, Negative, Validation, and End-to-End scenarios were included.
Test cases were easy to understand and execute.
Severity and Priority helped in identifying business-critical functionalities.
What I felt Not Suitable:
Some test cases were too generic and lacked detailed validation steps.
Product detail page functionality was not covered separately.
Logout functionality was missing.
Menu/Hamburger navigation was not covered.
Some scenarios were repetitive and could be merged.
Test data and preconditions were not mentioned.
Test cases were not fully automation-ready due to lack of clear verification points.

