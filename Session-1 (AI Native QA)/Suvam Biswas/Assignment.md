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

