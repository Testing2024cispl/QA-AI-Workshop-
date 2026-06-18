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

## Positive Test Scenarios

| Test Case ID | Scenario | Steps | Expected Result |
|---|---|---|---|
| TC_POS_01 | Sort products by Name (A to Z) | 1. Navigate to inventory page.<br>2. Click sort dropdown.<br>3. Select **Name (A to Z)**. | Products should be sorted alphabetically. |
| TC_POS_02 | Sort products by Name (Z to A) | 1. Navigate to inventory page.<br>2. Click sort dropdown.<br>3. Select **Name (Z to A)**. | Products should be sorted in descending alphabetical order. |
| TC_POS_03 | Sort products by Price (Low to High) | 1. Navigate to inventory page.<br>2. Select **Price (low to high)**.<br>3. Observe product prices. | Products should be sorted by ascending price. |
| TC_POS_04 | Sort products by Price (High to Low) | 1. Navigate to inventory page.<br>2. Select **Price (high to low)**.<br>3. Observe prices. | Products should be sorted by descending price. |
| TC_POS_05 | Add product to cart | 1. Navigate to inventory page.<br>2. Click **Add to Cart** for a product.<br>3. Observe cart badge. | Cart count should increase. |
| TC_POS_06 | Add multiple products to cart | 1. Add multiple products.<br>2. Open cart page.<br>3. Observe cart items. | All selected products should appear. |
| TC_POS_07 | Remove product from inventory page | 1. Add product to cart.<br>2. Click **Remove** from inventory page.<br>3. Observe cart badge. | Product should be removed. |
| TC_POS_08 | View cart items | 1. Add products to cart.<br>2. Click cart icon.<br>3. Observe cart page. | Items, quantity, and price should display correctly. |
| TC_POS_09 | Checkout with valid information | 1. Add products to cart.<br>2. Click **Checkout**.<br>3. Enter valid details. | User should reach overview page. |
| TC_POS_10 | View order overview | 1. Complete checkout information.<br>2. Click **Continue**.<br>3. Observe overview page. | Payment, shipping, and total price should display. |
| TC_POS_11 | Complete order successfully | 1. Reach overview page.<br>2. Click **Finish**.<br>3. Observe confirmation page. | Success message should display. |
| TC_POS_12 | Return to home page | 1. Complete order.<br>2. Click **Back Home**.<br>3. Observe page. | User should return to inventory page. |

---

## Negative Test Scenarios

| Test Case ID | Scenario | Steps | Expected Result |
|---|---|---|---|
| TC_NEG_01 | Open cart without adding products | 1. Login to application.<br>2. Click cart icon.<br>3. Observe cart. | Cart should be empty. |
| TC_NEG_02 | Remove item from empty cart | 1. Open empty cart.<br>2. Attempt remove action.<br>3. Observe response. | No crash should occur. |
| TC_NEG_03 | Checkout with empty cart | 1. Keep cart empty.<br>2. Click **Checkout**.<br>3. Observe behavior. | Checkout should be blocked or handled gracefully. |
| TC_NEG_04 | Submit checkout with empty fields | 1. Open checkout page.<br>2. Leave all fields blank.<br>3. Click **Continue**. | Validation message should display. |
| TC_NEG_05 | Missing First Name | 1. Leave First Name empty.<br>2. Fill other fields.<br>3. Click **Continue**. | Error should display. |
| TC_NEG_06 | Missing Last Name | 1. Leave Last Name empty.<br>2. Fill remaining fields.<br>3. Click **Continue**. | Validation should display. |
| TC_NEG_07 | Missing Zip Code | 1. Leave Zip Code empty.<br>2. Click **Continue**.<br>3. Observe response. | Error message should display. |
| TC_NEG_08 | Invalid Zip Code format | 1. Enter alphabetic zip code.<br>2. Click **Continue**.<br>3. Observe validation. | Invalid zip code should be rejected. |
| TC_NEG_09 | Rapid multiple clicks on Add to Cart | 1. Click **Add to Cart** rapidly multiple times.<br>2. Open cart.<br>3. Observe cart items. | Duplicate invalid entries should not occur. |
| TC_NEG_10 | Rapid multiple clicks on Finish | 1. Reach overview page.<br>2. Click **Finish** repeatedly.<br>3. Observe result. | Only one order should be processed. |
| TC_NEG_11 | Refresh browser during checkout | 1. Add products to cart.<br>2. Reach checkout page.<br>3. Refresh browser. | Cart state should remain consistent. |
| TC_NEG_12 | Browser Back during checkout | 1. Reach overview page.<br>2. Click browser back.<br>3. Observe workflow. | Application should handle navigation properly. |
| TC_NEG_13 | Checkout after removing all items | 1. Add products to cart.<br>2. Remove all products.<br>3. Attempt checkout. | Checkout should not proceed. |
| TC_NEG_14 | Finish order without completing checkout | 1. Attempt to bypass checkout steps.<br>2. Try accessing finish flow directly.<br>3. Observe response. | Order should not complete without required steps. |

---

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


