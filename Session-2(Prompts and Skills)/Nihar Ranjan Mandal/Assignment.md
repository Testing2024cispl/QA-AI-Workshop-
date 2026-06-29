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

