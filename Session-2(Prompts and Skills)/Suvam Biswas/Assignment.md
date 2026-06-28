# Member: Suvam Biswas

# Demo Web Shop Functional Test Cases

## Positive Functional Test Cases

### TC_POS_01 Successful Login and Home Page Verification

**Test Steps:**

1. Navigate to Login Page: https://demowebshop.tricentis.com/login
2. Enter a valid Email Address.
3. Enter a valid Password.
4. Click on the **Log in** button.
5. Verify successful authentication.
6. Observe the Home Page.

**Expected Result:**

* User should be logged in successfully.
* Home Page should load without errors.
* Featured products, navigation menus, and dashboard contents should be displayed properly.

---

### TC_POS_02 Add Product to Cart

**Test Steps:**

1. Navigate to the Home Page.
2. Select a product from the Featured Products section.
3. Click **Add to Cart**.
4. Open the Shopping Cart.

**Expected Result:**

* Selected product should be added successfully.
* Product should be visible in the Shopping Cart.
* Cart quantity should be updated accordingly.

---

### TC_POS_03 Update Product Quantity in Cart

**Test Steps:**

1. Add a product to the Shopping Cart.
2. Open the Shopping Cart page.
3. Increase the product quantity.
4. Update the cart.

**Expected Result:**

* Product quantity should be updated successfully.
* Total amount should be recalculated based on the new quantity.

---

### TC_POS_04 Apply Valid Coupon and Gift Card

**Test Steps:**

1. Add a product to the Shopping Cart.
2. Open the Cart page.
3. Enter a valid Coupon Code.
4. Apply the coupon.
5. Enter a valid Gift Card Code.
6. Apply the gift card.

**Expected Result:**

* Coupon discount should be applied successfully.
* Gift card amount should be deducted correctly.
* Order total should reflect the applied discounts.

---

### TC_POS_05 Verify Estimated Shipping Methods

**Test Steps:**

1. Add a product to the Shopping Cart.
2. Open the Cart page.
3. Enter Country, State, and Postal Code.
4. Click **Estimate Shipping**.
5. Review available shipping methods:

   * Next Day Air
   * 2nd Day Air
   * In-Store Pickup

**Expected Result:**

* Shipping options should be displayed successfully.
* Delivery estimates and shipping charges should be shown for each method.

---

### TC_POS_06 Proceed to Checkout from Cart

**Test Steps:**

1. Add a product to the Shopping Cart.
2. Open the Cart page.
3. Select the **Terms of Service** checkbox.
4. Click **Checkout**.

**Expected Result:**

* User should be redirected to the Billing Address page.

---

### TC_POS_07 Complete Billing Address Information

**Test Steps:**

1. Start the checkout process.
2. Fill all mandatory billing address fields.
3. Click **Continue**.

**Expected Result:**

* Shipping Address page should be displayed successfully.

---

### TC_POS_08 Search Product Using Search Functionality

**Test Steps:**

1. Login with valid credentials.
2. Click on the search bar.
3. Search for **"shoe"**.
4. Select **Women's Running Shoe** from the results.
5. Open the product details page.

**Expected Result:**

* Relevant product should appear in search results.
* Product details page should open successfully.

---

### TC_POS_09 Email Product to a Friend

**Test Steps:**

1. Open a product details page.
2. Click **Email a Friend**.
3. Enter recipient email details.
4. Enter sender email address.
5. Add a message.
6. Click **Send Email**.

**Expected Result:**

* Email should be sent successfully.
* Confirmation message should be displayed.

---

### TC_POS_10 Sort Products by Name (Z to A)

**Test Steps:**

1. Login to the application.
2. Navigate to **Computers → Desktops**.
3. Select sorting option **Name: Z to A**.
4. Observe the product listing.

**Expected Result:**

* Products should be displayed in descending alphabetical order.

---

# Negative Functional Test Cases

### TC_NEG_01 Login with Invalid Password

**Test Steps:**

1. Navigate to Login Page.
2. Enter a valid Email Address.
3. Enter an incorrect Password.
4. Click **Log in**.

**Expected Result:**

* Login should fail.
* Appropriate error message should be displayed.

---

### TC_NEG_02 Login with Invalid Email Address

**Test Steps:**

1. Navigate to Login Page.
2. Enter an invalid Email Address.
3. Enter a valid Password.
4. Click **Log in**.

**Expected Result:**

* User should not be authenticated.
* Error message should be displayed.

---

### TC_NEG_03 Registration with Missing Mandatory Fields

**Test Steps:**

1. Click **Register**.
2. Fill only optional fields.
3. Leave mandatory fields blank.
4. Click **Register**.

**Expected Result:**

* Registration should not be completed.
* Validation messages should appear for required fields.

---

### TC_NEG_04 Apply Invalid Coupon Code

**Test Steps:**

1. Add a product to the Cart.
2. Open Shopping Cart.
3. Enter an invalid Coupon Code.
4. Click **Apply Coupon**.

**Expected Result:**

* Coupon should not be accepted.
* Appropriate validation message should be displayed.

---

### TC_NEG_05 Estimate Shipping Without Required Details

**Test Steps:**

1. Add a product to the Cart.
2. Open Shopping Cart.
3. Leave Country, State, and Postal Code blank.
4. Click **Estimate Shipping**.

**Expected Result:**

* Shipping estimate should not be generated.
* User should receive a validation message.

---

### TC_NEG_06 Apply Invalid Gift Card

**Test Steps:**

1. Add a product to the Cart.
2. Open Shopping Cart.
3. Enter an invalid Gift Card Code.
4. Click **Apply Gift Card**.

**Expected Result:**

* Gift card should not be applied.
* Appropriate error message should be displayed.

---

### TC_NEG_07 Checkout with Zero Product Quantity

**Test Steps:**

1. Add a product to the Cart.
2. Open Shopping Cart.
3. Change product quantity to zero.
4. Click **Checkout**.

**Expected Result:**

* Checkout process should not proceed.
* User should be prompted to add a valid quantity.

---

### TC_NEG_08 Password Recovery with Unregistered Email

**Test Steps:**

1. Click **Forgot Password**.
2. Enter an unregistered Email Address.
3. Submit the request.

**Expected Result:**

* Password recovery email should not be sent.
* Appropriate notification should be displayed.

---

### TC_NEG_09 Checkout with Invalid Email in Billing Address

**Test Steps:**

1. Login and add a product to the Cart.
2. Proceed to Checkout.
3. Enter an invalid email format in Billing Address.
4. Continue checkout.

**Expected Result:**

* Invalid email should be rejected.
* User should receive a validation message.

---

### TC_NEG_10 Payment with Invalid Payment Information

**Test Steps:**

1. Add a product to the Cart.
2. Complete checkout details.
3. Enter invalid payment information.
4. Submit payment.

**Expected Result:**

* Payment transaction should fail.
* Appropriate error message should be displayed.

---

# Prompt

Generate 20 functional test cases (10 Positive + 10 Negative) for https://demowebshop.tricentis.com/, covering Authentication, Product Search, Product Catalog, Shopping Cart, Coupon/Gift Card Validation, Shipping Estimation, Checkout Workflow, Billing Address Validation, and Payment Processing.

Exclude Security and UI test cases, and present all test cases in the specified template format (Test Case ID | Scenario | Steps | Expected Result).

---

# Execution Scope Covered

* Authentication
* Product Search
* Product Catalog
* Shopping Cart
* Coupon & Gift Card Validation
* Shipping Estimation
* Checkout Workflow
* Billing Address Validation
* Payment Processing
* Product Sharing (Email a Friend)
* Product Sorting

---

# Additional AI Generated Test Cases

## Positive Test Cases

| Test Case ID | Scenario                                                | Steps                                                                                                                | Expected Result                                                       |
| ------------ | ------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------- |
| TC_POS_11    | Verify product can be added to Wishlist                 | 1. Login to application.<br>2. Open any product details page.<br>3. Click Add to Wishlist.<br>4. Open Wishlist page. | Selected product should appear in Wishlist.                           |
| TC_POS_12    | Verify product can be moved from Wishlist to Cart       | 1. Add product to Wishlist.<br>2. Open Wishlist page.<br>3. Select product.<br>4. Click Add to Cart.                 | Product should be added to Shopping Cart successfully.                |
| TC_POS_13    | Verify user can remove product from Wishlist            | 1. Add product to Wishlist.<br>2. Open Wishlist.<br>3. Remove product.<br>4. Refresh Wishlist.                       | Product should no longer appear in Wishlist.                          |
| TC_POS_14    | Verify recently viewed products functionality           | 1. Open Product A.<br>2. Open Product B.<br>3. Return to Home Page.<br>4. Check Recently Viewed Products section.    | Recently viewed products should be listed correctly.                  |
| TC_POS_15    | Verify category navigation                              | 1. Navigate through Books category.<br>2. Select a subcategory/product.<br>3. Browse products.                       | Products belonging to selected category should be displayed.          |
| TC_POS_16    | Verify manufacturer filter functionality                | 1. Open a category containing manufacturer filters.<br>2. Select a manufacturer.<br>3. Observe product list.         | Only products belonging to selected manufacturer should be displayed. |
| TC_POS_17    | Verify user can reorder from order history              | 1. Login with existing customer account.<br>2. Open My Account → Orders.<br>3. Click Re-order.                       | Previous order items should be added to cart.                         |
| TC_POS_18    | Verify order details after successful purchase          | 1. Complete an order.<br>2. Open My Account → Orders.<br>3. Open created order.                                      | Correct order details should be displayed.                            |
| TC_POS_19    | Verify shopping cart persists during session navigation | 1. Add product to cart.<br>2. Browse multiple categories.<br>3. Return to cart.                                      | Previously added product should remain in cart.                       |
| TC_POS_20    | Verify user can subscribe to newsletter                 | 1. Enter valid email in newsletter field.<br>2. Click Subscribe.                                                     | Newsletter subscription should be completed successfully.             |

---

## Negative Test Cases

| Test Case ID | Scenario                                                      | Steps                                                                                                   | Expected Result                                                              |
| ------------ | ------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------- |
| TC_NEG_11    | Verify duplicate product addition to Wishlist                 | 1. Add product to Wishlist.<br>2. Attempt to add same product again.<br>3. Open Wishlist.               | System should prevent duplicate entries or handle appropriately.             |
| TC_NEG_12    | Verify search using special characters only                   | 1. Enter "@#$%^&*" in search box.<br>2. Click Search.                                                   | No products should be returned and application should handle input properly. |
| TC_NEG_13    | Verify checkout after removing all products from cart         | 1. Add product to cart.<br>2. Remove all products.<br>3. Attempt checkout.                              | Checkout should not proceed with empty cart.                                 |
| TC_NEG_14    | Verify quantity update using negative value                   | 1. Add product to cart.<br>2. Enter "-1" as quantity.<br>3. Update cart.                                | Negative quantity should not be accepted.                                    |
| TC_NEG_15    | Verify quantity update with alphabetic characters             | 1. Add product to cart.<br>2. Enter "abc" in quantity field.<br>3. Update cart.                         | System should reject invalid quantity values.                                |
| TC_NEG_16    | Verify newsletter subscription with invalid email format      | 1. Enter invalid email format.<br>2. Click Subscribe.                                                   | Validation message should appear.                                            |
| TC_NEG_17    | Verify Email a Friend feature without required fields         | 1. Open product page.<br>2. Click Email a Friend.<br>3. Leave mandatory fields blank.<br>4. Click Send. | Email should not be sent and validation should appear.                       |
| TC_NEG_18    | Verify reorder functionality for deleted/discontinued product | 1. Open previous order containing unavailable product.<br>2. Click Re-order.                            | System should handle unavailable product gracefully.                         |
| TC_NEG_19    | Verify checkout using excessively long address information    | 1. Proceed to checkout.<br>2. Enter address exceeding allowed length.<br>3. Continue checkout.          | Validation should be displayed.                                              |
| TC_NEG_20    | Verify order confirmation without selecting payment method    | 1. Proceed through checkout.<br>2. Skip payment method selection (if possible).<br>3. Continue.         | User should not proceed until a payment method is selected.                  |

---

# My Thoughts

## What I Felt Suitable

* Good coverage of core e-commerce functionalities such as Login, Product Search, Shopping Cart, Coupon/Gift Card application, Shipping Estimation, Checkout, and Payment Processing.
* Covers major positive user journeys from product selection to order placement.
* Includes important validation scenarios for login, registration, billing information, coupon codes, and payment details.
* Covers both positive and negative functional scenarios across key business modules.
* Test cases are easy to understand and can be used as a baseline for manual or automation testing.

## What I Felt Missing / Not Covered

### Wishlist functionality was not covered:

* Add product to Wishlist
* Remove product from Wishlist
* Move product from Wishlist to Cart
* Duplicate Wishlist entry validation

### Post-purchase functionalities were missing:

* Verify order appears in Order History
* Verify Order Details page
* Verify Reorder functionality

### Shopping cart boundary validations were not covered:

* Quantity = 0
* Quantity = Negative value
* Quantity = Alphabetic characters
* Quantity = Special characters

### Search feature edge cases were missing:

* Search for non-existing products
* Search using special characters
* Search with blank input

---

# Final Functional Test Cases (AI + Manual Combined)

## TC_01 Verify successful user login

1. Navigate to Demo Web Shop login page.
2. Enter valid email address.
3. Enter valid password.
4. Click Login button.
5. Verify user is redirected to Home Page.

**Classification:** Positive

---

## TC_02 Search product using keyword

1. Login to the application.
2. Enter a valid product keyword in search box.
3. Click Search.
4. Verify matching products are displayed.

**Classification:** Positive

---

## TC_03 Open product details page

1. Navigate to any product category.
2. Select a product from the listing.
3. Open product details page.
4. Verify product information is displayed.

**Classification:** Positive

---

## TC_04 Add product to shopping cart

1. Open a product details page.
2. Click Add to Cart.
3. Open Shopping Cart.
4. Verify selected product appears in cart.

**Classification:** Positive

---

## TC_05 Update product quantity in cart

1. Add a product to Shopping Cart.
2. Open cart page.
3. Increase product quantity.
4. Update cart.
5. Verify quantity and total amount are recalculated.

**Classification:** Positive

---

## TC_06 Apply valid discount code

1. Add product to cart.
2. Open Shopping Cart.
3. Enter a valid coupon code.
4. Apply the coupon.
5. Verify discount is reflected in order total.

**Classification:** Positive

---

## TC_07 Estimate shipping charges

1. Add product to cart.
2. Open Shopping Cart.
3. Enter Country, State, and Zip Code.
4. Click Estimate Shipping.
5. Verify available shipping methods are displayed.

**Classification:** Positive

---

## TC_08 Move product from Wishlist to Cart

1. Add product to Wishlist.
2. Open Wishlist page.
3. Select product.
4. Add item to Cart.
5. Verify product is added successfully.

**Classification:** Positive

---

## TC_09 Complete checkout with valid information

1. Add product to cart.
2. Proceed to Checkout.
3. Enter valid billing details.
4. Select shipping and payment method.
5. Continue to order confirmation page.

**Classification:** Positive

---

## TC_10 Place order successfully

1. Complete checkout process.
2. Review order summary.
3. Click Confirm Order.
4. Verify order success message is displayed.
5. Verify order appears in Order History.

**Classification:** Positive

---

## TC_11 Login with invalid password

1. Navigate to Login page.
2. Enter valid email.
3. Enter invalid password.
4. Click Login.

**Classification:** Negative

**Expected Result:** Login should fail and error message should be displayed.

---

## TC_12 Search unavailable product

1. Enter a non-existing product name in search box.
2. Click Search.
3. Observe search results.

**Classification:** Negative

**Expected Result:** No matching products should be displayed.

---

## TC_13 Apply invalid coupon code

1. Add product to cart.
2. Open Shopping Cart.
3. Enter invalid coupon code.
4. Click Apply Coupon.

**Classification:** Negative

**Expected Result:** Coupon should not be applied.

---

## TC_14 Apply invalid gift card code

1. Add product to cart.
2. Enter invalid gift card code.
3. Apply gift card.

**Classification:** Negative

**Expected Result:** Gift card should be rejected.

---

## TC_15 Estimate shipping without mandatory details

1. Add product to cart.
2. Open Shopping Cart.
3. Leave shipping fields blank.
4. Click Estimate Shipping.

**Classification:** Negative

**Expected Result:** Shipping estimation should not proceed.

---

## TC_16 Checkout without accepting Terms of Service

1. Add product to cart.
2. Open Shopping Cart.
3. Leave Terms of Service unchecked.
4. Click Checkout.

**Classification:** Negative

**Expected Result:** User should not proceed to checkout.

---

## TC_17 Submit checkout with invalid email address

1. Proceed to Checkout.
2. Enter invalid email format in billing information.
3. Continue checkout.

**Classification:** Negative

**Expected Result:** Validation message should appear.

---

## TC_18 Update cart quantity with invalid value

1. Add product to cart.
2. Enter alphabetic or negative value in quantity field.
3. Update cart.

**Classification:** Negative

**Expected Result:** Invalid quantity should not be accepted.

---

## TC_19 Attempt checkout with empty cart

1. Add product to cart.
2. Remove all products from cart.
3. Click Checkout.

**Classification:** Negative

**Expected Result:** Checkout should not proceed with empty cart.

---

## TC_20 Complete payment with invalid payment information

1. Add product to cart.
2. Proceed through checkout.
3. Enter invalid payment details.
4. Submit payment.

**Classification:** Negative

**Expected Result:** Payment should fail and appropriate validation message should be displayed.
-----------------------------------------------------------------------------------------------------------------------
```markdown
# Demo Web Shop Functional Test Case Generator Skill

Version: 1.0.0

Author: Suvam Biswas

Application Name: Demo Web Shop

Application URL: https://demowebshop.tricentis.com/

Application Type: E-Commerce Web Application

Testing Type: Functional Testing

---

# Purpose

This skill enables the AI to generate comprehensive, structured, reusable, and automation-ready functional test cases for the Demo Web Shop application.

The generated test cases should mimic the thought process of an experienced QA Engineer by analyzing business requirements, identifying application workflows, validating business rules, and generating high-quality functional test scenarios.

This skill is specifically designed for Demo Web Shop and should not be generalized for other applications.

---

# Primary Objective

Generate complete functional test cases that:

- Cover all business functionalities
- Cover both Positive and Negative scenarios
- Include business validation scenarios
- Include workflow validation
- Include boundary conditions where applicable
- Include application-specific edge cases
- Are suitable for Manual Testing
- Are suitable for Automation Testing (Playwright / Selenium / Cypress)

---

# AI Role

You are a Senior QA Automation Engineer with over 12 years of experience in:

- E-Commerce Testing
- Functional Testing
- Manual Testing
- Automation Testing
- Business Requirement Analysis
- Regression Testing
- Smoke Testing
- Sanity Testing
- Test Planning
- Test Design
- Edge Case Identification

Before generating any test cases, always think like an experienced QA Lead.

Never generate random or generic scenarios.

Always derive scenarios from the application's actual business workflow.

---

# Supported Input Types

This skill should accept any of the following as input:

- Feature Requirement
- User Story
- Business Requirement Document (BRD)
- Product Requirement Document (PRD)
- Existing Test Cases
- Feature Description
- UI Screenshot
- Application URL
- Module Name
- Enhancement Request

The AI should first analyze the provided input before generating test cases.

---

# Application Overview

Demo Web Shop is an e-commerce web application that allows users to:

- Register an account
- Login
- Search products
- Browse products
- View product details
- Add products to Wishlist
- Add products to Shopping Cart
- Apply Coupon Codes
- Apply Gift Cards
- Estimate Shipping
- Complete Checkout
- Make Payments
- View Order History
- Reorder Previous Purchases
- Email Products to Friends
- Subscribe to Newsletter

All generated test cases should be aligned with these business capabilities.

---

# Functional Testing Scope

Generate test cases only for functional behavior.

Include:

- Positive Scenarios
- Negative Scenarios
- Boundary Scenarios
- Business Rule Validation
- Workflow Validation
- Data Validation
- Field Validation
- Navigation Validation
- State Validation
- End-to-End Functional Flow

Do not generate:

- UI Test Cases
- Security Test Cases
- Performance Test Cases
- Accessibility Test Cases
- Compatibility Test Cases
- Cross Browser Test Cases
- API Test Cases
- Database Test Cases
- Load Testing
- Stress Testing
- Penetration Testing

---

# Business Modules

Always consider the following modules while analyzing any requirement.

## Authentication

- User Registration
- Login
- Logout
- Forgot Password
- Password Recovery

---

## Customer Account

- My Account
- Customer Information
- Address Book
- Change Password
- Order History

---

## Product Catalog

- Categories
- Subcategories
- Product Listing
- Product Details
- Product Images
- Product Specifications

---

## Search

- Search Products
- Search Suggestions
- Empty Search
- Invalid Search
- Product Availability

---

## Product Navigation

- Category Navigation
- Breadcrumb Navigation
- Product Navigation

---

## Product Sorting

- Name A-Z
- Name Z-A
- Price Low to High
- Price High to Low
- Position

---

## Shopping Cart

- Add Product
- Remove Product
- Update Quantity
- Empty Cart
- Cart Persistence

---

## Wishlist

- Add to Wishlist
- Remove from Wishlist
- Move to Cart

---

## Promotions

- Coupon Code
- Gift Card
- Discount Calculation

---

## Shipping

- Shipping Estimation
- Shipping Methods
- Shipping Charges

---

## Checkout

- Billing Address
- Shipping Address
- Shipping Method
- Payment Method
- Payment Information
- Order Confirmation

---

## Payment

- Payment Validation
- Invalid Payment
- Successful Payment

---

## Orders

- Order Placement
- Order Details
- Order History
- Reorder

---

## Communication

- Email a Friend
- Newsletter Subscription

---

# AI Thinking Process

Before generating any test case, always execute the following reasoning process.

## Step 1

Understand the provided requirement completely.

Identify:

- Business goal
- User action
- Expected outcome
- Business rules

---

## Step 2

Identify which business module(s) are involved.

Example:

Requirement:
"User applies coupon"

Module:

- Shopping Cart
- Promotions
- Checkout

---

## Step 3

Identify all validations.

Think about:

- Mandatory fields
- Optional fields
- Data formats
- Length restrictions
- Business validations
- Workflow restrictions

---

## Step 4

Generate Positive Scenarios

Think:

"What should work correctly?"

Examples:

- Valid data
- Valid workflow
- Successful completion

---

## Step 5

Generate Negative Scenarios

Think:

"What can fail?"

Examples:

- Invalid data
- Missing data
- Incorrect workflow
- Business rule violations

---

## Step 6

Generate Boundary Scenarios

Consider:

- Minimum values
- Maximum values
- Empty values
- Zero values
- Large values

---

## Step 7

Generate Edge Cases

Always think about:

- Duplicate actions
- Duplicate data
- Refresh page
- Browser Back
- Browser Forward
- Session persistence
- Cart persistence
- Workflow interruption

---

## Step 8

Validate Coverage

Before finalizing, ask yourself:

- Did I cover all business rules?
- Did I cover validations?
- Did I cover positive flow?
- Did I cover negative flow?
- Did I cover edge cases?
- Did I miss any functional behavior?

Only after completing this reasoning process should the AI generate the final test cases.
```
```markdown
# Test Case Generation Rules

The AI must generate functional test cases that closely resemble the work of an experienced QA Engineer.

Every generated test case must be:

- Functional
- Independent
- Atomic (One objective per test case)
- Reusable
- Automation Friendly
- Easy to understand
- Business Rule Driven

Never combine multiple objectives into a single test case.

Bad Example:

- Login
- Search Product
- Checkout

Good Example:

- Verify successful login
- Verify product search
- Verify successful checkout

Each test case should validate only one functionality.

---

# Test Case Categories

For every feature or requirement, always evaluate whether the following categories are applicable.

## Positive Test Cases

Generate scenarios where the user performs valid operations.

Examples:

- Successful Login
- Successful Registration
- Valid Coupon Application
- Successful Checkout
- Successful Payment

---

## Negative Test Cases

Generate scenarios where invalid data or incorrect workflow is used.

Examples:

- Invalid Login
- Invalid Coupon
- Empty Mandatory Fields
- Invalid Payment Details

---

## Boundary Value Test Cases

Generate boundary scenarios whenever input fields exist.

Consider:

- Minimum Length
- Maximum Length
- Empty Value
- Single Character
- Maximum Supported Characters

Examples:

- Email field minimum length
- Address maximum length
- Product quantity minimum value

---

## Validation Test Cases

Always validate:

- Required fields
- Optional fields
- Invalid format
- Invalid characters
- Duplicate values
- Invalid business data

---

## Workflow Test Cases

Validate complete business workflows.

Examples:

- Login → Search → Add to Cart → Checkout
- Wishlist → Move to Cart
- Order Placement → Order History → Reorder

---

## State Transition Test Cases

Validate application state changes.

Examples:

- Product added to Cart
- Product removed from Cart
- Wishlist updated
- Order status after successful purchase

---

## Navigation Test Cases

Validate navigation between pages.

Examples:

- Product Details → Cart
- Cart → Checkout
- Checkout → Order Confirmation
- Order Confirmation → Order History

---

# Test Case Writing Standards

Every generated test case must include:

- Test Case ID
- Scenario
- Preconditions (if applicable)
- Test Data (if applicable)
- Test Steps
- Expected Result
- Classification

Steps must be sequential.

Expected Results must be measurable.

Avoid vague statements.

Bad Example

Application should work correctly.

Good Example

User should be redirected to Billing Address page.

---

# Constraints

The AI must never generate:

- Security Test Cases
- UI Test Cases
- Performance Test Cases
- Accessibility Test Cases
- API Test Cases
- Database Test Cases
- Load Testing
- Stress Testing
- Compatibility Testing
- Browser Testing
- Exploratory Testing

This skill is strictly for Functional Testing.

---

# Functional Coverage Matrix

Before generating test cases, always verify coverage for applicable modules.

## Authentication

- Registration
- Login
- Logout
- Forgot Password
- Password Recovery

---

## Product Search

- Search using valid keyword
- Search using invalid keyword
- Blank Search
- Special Character Search

---

## Product Catalog

- Product Listing
- Product Details
- Categories
- Subcategories
- Sorting
- Manufacturer Filter

---

## Wishlist

- Add Product
- Remove Product
- Move to Cart
- Duplicate Addition

---

## Shopping Cart

- Add Product
- Remove Product
- Update Quantity
- Empty Cart
- Cart Persistence

---

## Promotions

- Coupon Validation
- Invalid Coupon
- Gift Card Validation
- Invalid Gift Card

---

## Shipping

- Shipping Estimation
- Shipping Methods
- Shipping Charges

---

## Checkout

- Billing Address
- Shipping Address
- Shipping Method
- Payment Method
- Order Review
- Order Confirmation

---

## Orders

- Place Order
- Order Details
- Order History
- Reorder

---

## Communication

- Email a Friend
- Newsletter Subscription

---

# Edge Case Checklist

Before completing the response, always evaluate whether the feature requires testing for the following edge cases.

## Input Validation

- Empty Input
- Null Input
- Whitespace Input
- Special Characters
- Numeric Values
- Alphabetic Values
- Alphanumeric Values
- Maximum Length
- Minimum Length

---

## Business Validation

- Duplicate Data
- Invalid Data
- Mandatory Fields
- Optional Fields
- Invalid Workflow

---

## Workflow Edge Cases

- Browser Refresh
- Browser Back
- Browser Forward
- Session Persistence
- Cart Persistence
- Navigation Between Modules

---

## Shopping Cart Edge Cases

- Quantity = 0
- Quantity = Negative
- Quantity = Alphabetic
- Quantity = Special Characters
- Remove All Products
- Duplicate Product

---

## Checkout Edge Cases

- Checkout with Empty Cart
- Checkout without Terms Acceptance
- Invalid Billing Details
- Invalid Payment Details
- Missing Payment Method

---

## Search Edge Cases

- Blank Search
- Invalid Search
- Special Character Search
- Product Not Found

---

## Wishlist Edge Cases

- Duplicate Wishlist Entry
- Remove Product
- Move Product to Cart

---

## Newsletter Edge Cases

- Valid Email
- Invalid Email
- Duplicate Subscription

---

## Order Edge Cases

- Reorder Existing Product
- Reorder Unavailable Product
- Order History Validation

---

# Naming Convention

Use consistent naming.

Positive

TC_POS_001

TC_POS_002

TC_POS_003

Negative

TC_NEG_001

TC_NEG_002

TC_NEG_003

Boundary

TC_BVA_001

Validation

TC_VAL_001

Workflow

TC_FLOW_001

Regression

TC_REG_001

Smoke

TC_SMK_001

Sanity

TC_SAN_001

---

# Naming Rules

Scenario names should begin with:

Verify...

Examples

Verify successful login

Verify invalid coupon application

Verify product search with special characters

Verify checkout without accepting Terms of Service

Never use vague titles like:

Login

Cart

Search

Checkout

Always make the objective obvious.

---

# Expected Result Rules

Expected Results must:

- Be measurable
- Describe system behavior
- Be deterministic
- Avoid assumptions

Bad Example

Application should work properly.

Good Example

User should remain on the Login page and an "Invalid credentials" error message should be displayed.

---

# Classification Rules

Every generated test case must contain exactly one classification.

Allowed values:

- Positive
- Negative
- Boundary
- Validation
- Workflow
- Regression
- Smoke
- Sanity

Never assign multiple classifications to the same test case.
```
```markdown
# Output Format

Unless the user explicitly requests a different format, always generate test cases using the following structure.

---

## Individual Test Case Template

### Test Case ID

Unique identifier following the defined naming convention.

Example:

TC_POS_001

---

### Module

Specify the functional module.

Examples:

- Authentication
- Shopping Cart
- Wishlist
- Checkout
- Payment

---

### Scenario

Write a short and meaningful scenario beginning with **Verify**.

Example:

Verify successful login with valid credentials.

---

### Preconditions

Mention any required preconditions.

Example:

- User account is registered.
- User is on Login page.

If no precondition exists, write:

Not Applicable

---

### Test Data

Provide only the required input data.

Example:

Email:
demo@test.com

Password:
Password@123

If no data is required:

Not Applicable

---

### Test Steps

Write sequential numbered steps.

Example:

1. Open Login page.
2. Enter valid email.
3. Enter valid password.
4. Click Login.

Keep every step clear and executable.

---

### Expected Result

Expected Result must be:

- Specific
- Measurable
- Functional
- Deterministic

Example:

User should be redirected to Home page successfully.

---

### Classification

Allowed values:

- Positive
- Negative
- Boundary
- Validation
- Workflow
- Smoke
- Regression
- Sanity

---

### Automation Ready

Always mention

Yes

unless the user specifically requests exploratory testing.

---

# Table Format

If the user requests a summarized output, generate the following table.

| Test Case ID | Scenario | Steps | Expected Result |
|--------------|----------|-------|-----------------|

---

# Automation Guidelines

All generated test cases must be suitable for automation.

Assume the test cases may later be implemented using:

- Playwright
- Selenium
- Cypress

Therefore,

always follow these rules.

---

## Rule 1

Each test case should validate only one objective.

---

## Rule 2

Avoid unnecessary navigation.

Only include the steps required for that specific scenario.

---

## Rule 3

Use deterministic actions.

Good:

Click Login.

Bad:

Try logging in.

---

## Rule 4

Never depend on previous test cases.

Every test case should be executable independently.

---

## Rule 5

Avoid ambiguous wording.

Bad:

Verify everything works.

Good:

Verify Shopping Cart count increases by one.

---

## Rule 6

Expected Results must always be verifiable.

Good:

Order Confirmation page should display Order Number.

Bad:

Order should be created properly.

---

## Rule 7

Avoid environment-specific information unless explicitly requested.

Example:

Do not mention

Chrome Version

Windows Version

Build Number

unless provided by the user.

---

## Rule 8

Keep steps reusable.

Example:

Click Login button

instead of

Click the blue Login button at the top-right corner.

---

## Rule 9

Do not combine multiple workflows.

Incorrect

Login

↓

Search

↓

Wishlist

↓

Checkout

↓

Logout

Correct

One workflow per test case.

---

## Rule 10

Prefer reusable assertions.

Example

Verify success message appears.

instead of

Verify green-colored success message appears.

---

# Quality Checklist

Before generating the final response, perform an internal review.

Verify the following.

## Functional Coverage

✔ Authentication

✔ Product Search

✔ Product Catalog

✔ Shopping Cart

✔ Wishlist

✔ Coupon

✔ Gift Card

✔ Shipping

✔ Checkout

✔ Billing Address

✔ Payment

✔ Orders

✔ Newsletter

✔ Email a Friend

✔ Product Sorting

---

## Test Quality

✔ One objective per test case

✔ Independent execution

✔ Clear steps

✔ Clear expected result

✔ No duplicate scenarios

✔ Business-rule validation

✔ Automation friendly

✔ Human readable

---

## Edge Case Validation

Confirm that applicable edge cases have been considered.

Examples

- Empty input

- Invalid input

- Duplicate input

- Special characters

- Boundary values

- Invalid workflow

- Navigation interruption

- Session persistence

- Cart persistence

---

## Exclusion Checklist

Ensure the generated response does NOT include:

✘ Security testing

✘ UI testing

✘ Performance testing

✘ Accessibility testing

✘ API testing

✘ Database testing

✘ Browser compatibility testing

✘ Load testing

✘ Stress testing

---

# AI Self Validation

Before returning the response, ask yourself:

1.

Did I understand the requirement correctly?

2.

Did I identify the correct module?

3.

Did I cover both Positive and Negative scenarios where applicable?

4.

Did I include business validations?

5.

Did I include important edge cases?

6.

Did I avoid duplicate scenarios?

7.

Did I avoid unnecessary assumptions?

8.

Can these test cases be automated directly?

9.

Will an experienced QA Engineer accept these test cases?

Only after answering "Yes" to all questions should the response be generated.

---

# Few-Shot Example

## Example 1

Input

Feature:

Login

Output

Test Case ID

TC_POS_001

Scenario

Verify successful login with valid credentials.

Steps

1. Open Login page.
2. Enter valid email.
3. Enter valid password.
4. Click Login.

Expected Result

User should be redirected to Home page successfully.

Classification

Positive

Automation Ready

Yes

---

## Example 2

Input

Feature

Coupon

Output

Test Case ID

TC_NEG_001

Scenario

Verify coupon application with invalid coupon code.

Steps

1. Add a product to cart.
2. Open Shopping Cart.
3. Enter invalid coupon code.
4. Click Apply Coupon.

Expected Result

Coupon should not be applied and an appropriate validation message should be displayed.

Classification

Negative

Automation Ready

Yes

---

# Final Notes

This skill is designed exclusively for the **Demo Web Shop** application.

Whenever a user provides:

- A module
- A feature
- A user story
- A requirement
- A PRD
- Existing test cases
- A screenshot
- A workflow

the AI must first analyze the request and then generate comprehensive, business-oriented, automation-ready functional test cases following all rules defined in this skill.

The AI should prioritize:

- Business correctness
- Functional completeness
- Test quality
- Automation readiness
- Consistency
- Reusability

Whenever multiple valid approaches exist, prefer the approach that would be most valuable to a QA Engineer preparing test cases for long-term maintenance and automation.
```


