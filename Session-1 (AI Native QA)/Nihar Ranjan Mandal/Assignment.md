Session-01 Assignment:

Google Doc Link: https://docs.google.com/document/d/1SlUg3LAJcB8xLaWcUyMEKOcwsPnGIuKEY0lZbtfFYoI/edit?usp=sharing

Test Cases For an E-Commerce Website:-

Project Name: DemoBlaze E2E Testing Flow
E-Commerce Website: https://www.demoblaze.com/

TestCases by Human Intelligence:

Positive Test Cases:

TC_001: Validating Elements in the Home webpage.
Step-01: Open Website https://www.demoblaze.com/.
Step-02: Verify the website redirection to “Home” page.
Step-03: Verify the redirection by clicking all the elements at the top such as Home, Contact, About us, Cart, Log in, Sign up.
Step-04: Verify the Elements in "Categories" by clicking such as Phones, Laptops, Monitors whether the clicked category items are displaying or not.

TC_002: Validating Product page functionality.
Step-01: Click on any product from the Home Page.
Step-02: Verify the redirection to selected product details page.
Step-03: Verify the selected_product_image, selected_product_name, selected_product_price and selected_product_description in the product details page.
Step-04: Verify by clicking on "Add to cart" button that a confirmation pop-up should display in the page.

TC_003: Validating Cart page functionality.
Step-01: Verify the cart page if the cart is empty.
Step-02: Verify the Pic, Title and Price of added cart products should display in cart page.
Step-03: Validate the delete button functionality
Step-04: Validate the "Total Price" amount for the selected product/products.
Step-05: Validate by clicking on "Place Order" button whether place order details is displaying or not.

TC_004: Validating "Place order" functionality.
Step-01: After clicking on "Place order" button from cart page "Place Order" page should open.
Step-02: Validate the total amount and fill the data in all the fields in the "Place Order" page.
Step-03: Validate the "close" and "purchase" buttons functionalities.
Step-04: Verify that after clicking on "purchase" button from the "place order" by filling all details that "ThankYou" page should open.
Step-05: Verify the order details in the "ThankYou" page.

TC_005: Validating "Log in" functionality.
Step-01: Open the "Log in" page by clicking on "Log in" button from the Home page Header.
Step-02: Enter the valid user_name and password and click on "Log in" button.

TC_006: Validating "Sign up" functionality.
Step-01: Open the "Sign up" page by clicking on "Sign up" button from the Home page Header.
Step-02: Enter the valid user_name and password and click on "Sign up" button.


Negative Test Cases:

TC_007: Validating by placing order with empty cart.
Step-01: Keep the cart page empty.
step-02: Go the cart page and click on place order.
step-03: In place order page fill the details and click on "purchase" button and check whether error pop-up is displaying or not.

TC_008: Validating by placing order with empty data in place order page.
Step-01: Keep the cart page non-empty.
step-02: Go the cart page and click on place order.
step-03: In place order page don't fill the details and click on "purchase" button and check whether error pop-up is displaying or not.

TC_009: Validating by placing order with empty cart and empty fields in purchase order page.
Step-01: Keep the cart page empty.
step-02: Go the cart page and click on place order.
step-03: In place order page don't fill the details and click on "purchase" button and check whether error pop-up is displaying or not.

TC_0010: Validating "Log in" functionality with Invalid data.
Step-01: Open the "Log in" page by clicking on "Log in" button from the Home page Header.
Step-02: Enter the invalid user_name & valid password and click on "Log in" button.
Step-02: Enter the valid user_name & invalid password and click on "Log in" button.
Step-02: Enter the invalid user_name & invalid password and click on "Log in" button.
Step-03: In all the cases an Error message should display in Login page.

TC_0011: Validating "Sign up" functionality with Empty fields.
Step-01: Open the "Sign up" page by clicking on "Sign up" button from the Home page Header.
Step-02: Keep the user_name and password fields empty and click on "Sign up" button ; an error pop-up should display in Sign up page.

TC_0012: Validating "Log in" functionality with empty fields.
Step-01: Open the "Log in" page by clicking on "Log in" button from the Home page Header.
Step-02: Keep the user_name and password fields empty and click on "Log in" button ; an error pop-up should display in Sign up page.


TestCases by AI:


Module: Home Page
TC_001: Verify Home page loads successfully 
TC_002: Verify navigation bar contains Home, Contact, About Us, Cart, Login, Sign Up 
TC_003: Verify product list is displayed 
TC_004: Verify clicking logo redirects to Home page 
TC_005: Verify page behavior on refresh 

Module: Sign Up
Positive Test Cases:
TC_001: Register with valid unique username and password 
TC_002: Verify success alert after registration 
TC_003: Verify newly registered user can login
Negative Test Cases:
TC_001: Register with existing username 
TC_002: Register with blank username 
TC_003: Register with blank password 
TC_004: Register with both fields blank 
TC_005: Close signup popup without registration

Module: Log in
Positive Test Cases:
TC_001: Login with valid credentials 
TC_002: Verify username appears after login 
TC_003: Verify Logout option displayed after login
Negative Test Cases:
TC_001: Login with invalid username 
TC_002: Login with invalid password 
TC_003: Login with blank username 
TC_004: Login with blank password 
TC_005: Login with both fields blank 

Module: Categories
TC_001: Click Phones category 
TC_002: Verify all displayed products belong to Phones category 
TC_003: Rapidly click Phones category multiple times 
TC_004: Click Laptops category 
TC_005: Verify laptop products shown correctly 
TC_006: Click Monitors category 
TC_007: Verify monitor products shown correctly 

Module: Product Details
Positive Test Cases:
TC_001: Open product details page 
TC_002: Verify product name displayed 
TC_003: Verify product price displayed 
TC_004: Verify product description displayed 
Negative Test Cases:
TC_001: Open invalid product URL 
TC_002: Refresh product page

Module: Add to Cart
Positive Test Cases:
TC_001: Add Phone/Laptop/Monitor product to cart 
TC_002: Add Laptop product to cart 
TC_003: Add Monitor product to cart 
TC_004: Add multiple products 
TC_005: Verify cart displays selected products 
Negative Test Cases:
TC_001: Add same product multiple times 
TC_002: Navigate away immediately after Add to Cart 
TC_003: Refresh cart page

Module: Cart
Positive Test Cases:
TC_001: Open cart page 
TC_002: Verify total amount calculation 
TC_003: Delete product from cart 
TC_004: Verify total updates after deletion 
Negative Test Cases:
TC_001: Delete last product 
TC_002: Open cart with no products

Module: Place Order
Positive Test Cases:
TC_001: Place order with all valid details 
TC_002: Verify order confirmation popup 
TC_003: Verify generated order ID 
TC_004: Verify cart is cleared after purchase 
Negative Test Cases:
TC_001: Place order with blank Name 
TC_002: Place order with blank Country 
TC_003: Place order with blank City 
TC_004: Place order with blank Credit Card 
TC_005: Place order with blank Month 
TC_006: Place order with blank Year 
TC_007: Submit order form with all fields blank
Module: Contact
Positive Test Cases:
TC_001: Submit contact form with valid email, name and message 
TC_002: Verify success alert displayed 
Negative Test Cases:
TC_001: Submit with blank email 
TC_002: Submit with blank name 
TC_003: Submit with blank message 
TC_004: Submit all fields blank 

Module: About Us
TC_001: Open About Us popup 
TC_002: Play embedded video 
TC_003: Close About Us popup 
TC_004: Open and close popup multiple times 


TestCases by AI+Human Intelligence:

Module: Home Page
TC_001: Verify Home page loads successfully 
TC_002: Verify navigation bar contains Home, Contact, About Us, Cart, Login, Sign Up 
TC_003: Verify product list is displayed 
TC_004: Verify clicking logo redirects to Home page 
TC_005: Verify page behavior on refresh 

Module: Sign Up
Positive Test Cases:
TC_001: Register with valid unique username and password 
TC_002: Verify success alert after registration 
TC_003: Verify newly registered user can login
Negative Test Cases:
TC_001: Register with existing username 
TC_002: Register with blank username 
TC_003: Register with blank password 
TC_004: Register with both fields blank 
TC_005: Close signup popup without registration

Module: Log in
Positive Test Cases:
TC_001: Login with valid credentials 
TC_002: Verify username appears after login 
TC_003: Verify Logout option displayed after login
Negative Test Cases:
TC_001: Login with invalid username 
TC_002: Login with invalid password 
TC_003: Login with blank username 
TC_004: Login with blank password 
TC_005: Login with both fields blank 

Module: Categories
TC_001: Click Phones category 
TC_002: Verify all displayed products belong to Phones category 
TC_003: Rapidly click Phones category multiple times 
TC_004: Click Laptops category 
TC_005: Verify laptop products shown correctly 
TC_006: Click Monitors category 
TC_007: Verify monitor products shown correctly 

Module: Product Details
Positive Test Cases:
TC_001: Open product details page 
TC_002: Verify product name displayed 
TC_003: Verify product price displayed 
TC_004: Verify product description displayed 
Negative Test Cases:
TC_001: Open invalid product URL 
TC_002: Refresh product page


Module: Product Details
Positive Test Cases:
TC_001: Open product details page 
TC_002: Verify product name, price and description displayed  
Negative Test Cases:
TC_001: Open invalid product URL 
TC_002: Refresh product page

Module: Add to Cart
Positive Test Cases:
TC_001: Add Phone/Laptop/Monitor product to cart 
TC_002: Add multiple products 
TC_003: Verify cart displays selected products 
Negative Test Cases:
TC_001: Add same product multiple times 
TC_002: Navigate away immediately after Add to Cart 
TC_003: Refresh cart page

Module: Cart
Positive Test Cases:
TC_001: Open cart page 
TC_002: Verify total amount calculation 
TC_003: Delete product from cart 
TC_004: Verify total updates after deletion 
Negative Test Cases:
TC_001: Open cart with no products

Module: Place Order
Positive Test Cases:
TC_001: Place order with all valid details 
TC_002: Verify order confirmation popup 
TC_003: Verify generated order ID 
TC_004: Verify cart is cleared after purchase 
Negative Test Cases:
TC_001: Place order with blank Name 
TC_002: Place order with blank Country 
TC_003: Place order with blank City 
TC_004: Place order with blank Credit Card 
TC_005: Place order with blank Month 
TC_006: Place order with blank Year 
TC_007: Submit order form with all fields blank

==================================================================================
Session-02 Assignment:

# Skill: Generate an e-commerce website end to end test

## Purpose

Generate comprehensive positive, negative, boundary end to end testcases for an e-commerce website, covering functionalities such as login, select product from home page, applying products filter, adding product(s) to cart, place order, payment page validation, ThankYou page validation.

## Inputs

* E-Commerce website URL
* Opening login page by clicking on page header
* Username field details
* Password field details
* Login button
* Applying product category filter
* Selecting product from home page
* Adding product(s) to cart
* Placing order
* Payment page validation
* Thank You page validation

## Instructions

Act as a Senior QA Engineer with 10+ years of experience in writing and maintaining Test Scenarios and Test Cases.

Generate test cases covering the following categories:

### 1. Positive Test Scenarios

* Login with valid username and password.
* Products should display on the basis of applied filter.
* Selecting a product from home page should navigate to product details page.
* Adding product(s) to cart should display in cart page.
* Placing order by clicking on "Place Order" button from cart page should redirect to payment page.
* Provide the required details on payment page and click on "Submit" button should redirect to Thankyou page.
* Validate the details on the Thankyou page after order placed successfully.

### 2. Negative Test Scenarios

* Invalid username and valid password in login page.
* Valid username and invalid password in login page.
* Invalid username and invalid password in login page.
* Blank username in login page.
* Blank password in login page.
* Both fields blank in login page.
* Keeping blank on payment page details and click "Submit" button.
* Invalid card number and CVV in payment page.
* Keeping blank the required mandatory fields in payment page.
* Adding products multiple times to cart and verify the number of products in cart.
* Attempting to place order without adding any product to cart.
* Validating the total amount in cart page by deleteing product(s) from cart.

### 3. Boundary Value Testing

* Minimum username length in login page.
* Maximum username length in login page.
* Minimum password length in login page.
* Maximum password length in login page.
* Minimum length in CVV Field in payment page.
* Maximum length in CVV Field in payment page.
* Minimum length in card number field in payment page.
* Maximum length in card number field in payment page.

### 4. Field Validation Testing

* Mandatory field validation in payment page.
* Leading/trailing spaces after entering payment details.

## Output Format

Generate a table with the following columns:

| TC ID | TestCase Description | Test Steps |

Include:

* Positive test cases
* Negative test cases
* Edge cases






