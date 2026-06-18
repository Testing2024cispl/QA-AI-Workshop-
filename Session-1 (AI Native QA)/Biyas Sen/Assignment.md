# Member - Biyas Sen

# Human Thinking Manual Test Cases

## TC_POS_01 View product inventory

1. Navigate to the Swag Labs inventory page.
2. Observe all listed products.
3. Verify product details like name, description , price.
4. All products should display correctly.

## TC_POS_02 Add single product to cart

1. Navigate to inventory page.
2. Click Add to Cart for one product.
3. Observe cart icon.
4. Cart count should increase by 1.

## TC_POS_03 Add multiple products to cart

1. Navigate to inventory page.
2. Add two products to cart.
3. Open cart page.
4. Both products should be visible in cart.

## TC_POS_04 Remove product from cart

1. Add products to cart.
2. Open cart page.
3. Click Remove for one product.
4. Selected product should be removed.

## TC_POS_05 Remove all product from cart

1. Add products to cart.
2. Open cart page.
3. Click Remove for all product.
4. All product should be remove and should show the rediction icon or button for revisit to the product listing page.


## TC_POS_06 Continue shopping from cart

1. Add product to cart.
2. Open cart page.
3. Click Continue Shopping.
4. User should return to inventory page.

## TC_POS_07 Proceed to checkout

1. Add products to cart.
2. Open cart page.
3. Click Checkout.
4. Checkout information page should open.

## TC_POS_08 Enter valid checkout information

1. Open checkout page.
2. Enter valid First Name.
3. Enter Last Name and Zip Code.
4. User should proceed to overview page.

## TC_POS_09 Complete order successfully

1. Complete checkout information.
2. Click Continue.
3. Click Finish.
4. Success message should be displayed.

## TC_NEG_01 Open cart without products

1. Login to application.
2. Click cart icon without adding items.
3. Observe cart page.
4. Cart should be empty.

## TC_NEG_02 Checkout with empty cart

1. Keep cart empty.
2. Open cart.
3. Click Checkout.
4. Checkout should be blocked or handled properly.

## TC_NEG_03 Submit checkout with empty fields

1. Open checkout information page.
2. Leave all fields empty.
3. Click Continue.
4. Validation message should appear.

## TC_NEG_04 Missing first name

1. Open checkout page.
2. Leave first name blank.
3. Fill other fields and continue.
4. Error message should display.

## TC_NEG_05 Missing last name

1. Open checkout page.
2. Leave last name blank.
3. Fill other fields and continue.
4. Error should display.

## TC_NEG_06 Missing zip code

1. Open checkout page.
2. Leave zip code blank.
3. Click Continue.
4. Validation should appear.

## TC_NEG_07 Invalid zip code

1. Open checkout page.
2. Enter alphabets in zip field.
3. Click Continue.
4. Invalid input should be rejected.

## TC_NEG_08 Multiple rapid clicks on Finish

1. Reach overview page.
2. Click Finish multiple times quickly.
3. Observe response.
4. Only one order should be created.

# Prompt

I need you to prepare all positive and negative functional test cases for the following website:

**https://www.saucedemo.com/**

## Requirements

1. Only functional test cases — NO security test cases, NO UI test cases
2. Include BOTH positive and negative test cases
3. Cover all major functionalities of the application

## Functionalities to cover

* Product inventory listing
* Product sorting
* Cart management (add/remove items)
* Checkout process
* Checkout form validation
* Order overview
* Order completion
* Any other functional behavior on the page


### TC_POS_01 [Test Case Title]

1. Step 1
2. Step 2
3. Step 3
4. Expected Result

### TC_NEG_01 [Test Case Title]

1. Step 1
2. Step 2
3. Step 3
4. Expected Result

# AI Generated Test Cases

## TC_POS_01 Sort products A-Z

1. Navigate to inventory page.
2. Select Name (A to Z) from dropdown.
3. Observe product order.
4. Products should be sorted alphabetically.

## TC_POS_02 Sort products by price low-high

1. Navigate to inventory page.
2. Select Price Low to High.
3. Observe prices.
4. Products should be sorted in ascending order.

## TC_POS_03 Add same product to cart

1. Navigate to inventory page.
2. Add product to cart.
3. Open cart.
4. Product should appear correctly.

## TC_POS_04 View checkout overview

1. Add products to cart.
2. Complete checkout info.
3. Click Continue.
4. Order summary should display.

## TC_POS_05 Back home after order

1. Complete order.
2. Click Back Home.
3. Observe page.
4. User should return to home page.

## TC_NEG_01 Remove item from empty cart

1. Open empty cart.
2. Attempt remove action.
3. Observe system.
4. No crash should occur.

## TC_NEG_02 Add same product multiple times rapidly

1. Navigate to inventory page.
2. Click Add to Cart multiple times rapidly.
3. Open cart.
4. Duplicate invalid entries should not occur.

## TC_NEG_03 Refresh browser during checkout

1. Add items to cart.
2. Reach checkout page.
3. Refresh browser.
4. Data should remain consistent.

# My Thoughts

## What I felt Suitable

* Good coverage of inventory, sorting, cart, and checkout
* Helpful in quickly generating baseline functional scenarios
* Covers edge cases like refresh and browser navigation

## What I felt Not Suitable

* Some scenarios are generic and need application-specific validation
* AI missed detailed field validations
* Some negative scenarios are assumption-based

# Final Test Cases (AI + Manual Combined for Automation Ready)

## TC_01 View product inventory

1. Navigate to Swag Labs inventory page
2. Observe product listing
3. Verify name, description, and price
4. All products should display correctly

**Classification:** Positive

## TC_02 Sort products alphabetically

1. Navigate to inventory page
2. Select Name (A-Z) sorting
3. Observe product order
4. Products should sort alphabetically

**Classification:** Positive

## TC_03 Add single product to cart

1. Click Add to Cart for a product
2. Observe cart badge
3. Open cart
4. Product should appear in cart

**Classification:** Positive

## TC_04 Remove product from cart

1. Add products to cart
2. Remove one product
3. Observe cart
4. Product should be removed

**Classification:** Positive

## TC_05 Checkout with valid information

1. Add products to cart
2. Click Checkout
3. Enter valid user information
4. User should reach overview page

**Classification:** Positive

## TC_06 Complete successful order

1. Reach overview page
2. Click Finish
3. Observe confirmation page
4. Success message should display

**Classification:** Positive

## TC_07 Submit empty checkout form

1. Open checkout page
2. Leave all fields empty
3. Click Continue
4. Validation error should display

**Classification:** Negative

## TC_08 Invalid zip code

1. Enter alphabetic zip code
2. Click Continue
3. Observe validation
4. Invalid input should be rejected

**Classification:** Negative

## TC_09 Rapid multiple Finish clicks

1. Reach order overview
2. Click Finish repeatedly
3. Observe order creation
4. Only one order should be processed

**Classification:** Negative


