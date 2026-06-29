# Saucedemo Test Scenarios And Traceability Matrix

## Application Under Test

- URL: https://www.saucedemo.com/
- Username: `standard_user`
- Password: `secret_sauce`

## Scope

This document covers positive, negative, and edge test scenarios for the Saucedemo application after logging in with a valid standard user account. It also includes a traceability matrix for better test case coverage.

---

## Positive Test Scenarios

### P01 - Login With Valid Credentials

**Scenario:** Verify that a user can log in with valid credentials.

**Test Data:**
- Username: `standard_user`
- Password: `secret_sauce`

**Expected Result:**
- User should successfully log in.
- User should be redirected to the Products page.
- URL should contain `inventory.html`.

---

### P02 - Verify Product Listing After Login

**Scenario:** Verify that all products are displayed on the Products page after login.

**Expected Result:**
- Products page should be displayed.
- Six products should be visible.
- Each product should show:
  - Product image
  - Product name
  - Product description
  - Product price
  - Add to cart button

---

### P03 - Add Single Product To Cart

**Scenario:** Verify that a user can add one product to the cart.

**Expected Result:**
- Product should be added to the cart.
- Cart badge should display `1`.
- Add to cart button should change to Remove.

---

### P04 - Add Multiple Products To Cart

**Scenario:** Verify that a user can add multiple products to the cart.

**Expected Result:**
- All selected products should be added to the cart.
- Cart badge should show the correct number of added products.
- Added product buttons should change to Remove.

---

### P05 - Remove Product From Inventory Page

**Scenario:** Verify that a user can remove an added product from the Products page.

**Expected Result:**
- Product should be removed from the cart.
- Cart badge count should decrease.
- Remove button should change back to Add to cart.

---

### P06 - Open Cart With Added Products

**Scenario:** Verify that the cart displays selected products correctly.

**Expected Result:**
- Cart page should open.
- Selected products should be displayed.
- Each cart item should show:
  - Quantity
  - Product name
  - Product description
  - Product price
  - Remove button

---

### P07 - Continue Shopping From Cart

**Scenario:** Verify that the Continue Shopping button works from the cart page.

**Expected Result:**
- User should be redirected back to the Products page.
- Previously added cart items should remain in the cart.

---

### P08 - Checkout With Valid User Information

**Scenario:** Verify that checkout continues when valid information is entered.

**Test Data:**
- First Name: `John`
- Last Name: `Doe`
- Postal Code: `12345`

**Expected Result:**
- User should navigate to the Checkout Overview page.
- Entered information should be accepted.

---

### P09 - Verify Checkout Overview

**Scenario:** Verify that the Checkout Overview page displays correct order details.

**Expected Result:**
- Selected products should be displayed.
- Payment information should be displayed.
- Shipping information should be displayed.
- Item total, tax, and final total should be displayed correctly.

**Observed Example:**
- Products: Sauce Labs Backpack and Sauce Labs Bike Light
- Item Total: `$39.98`
- Tax: `$3.20`
- Total: `$43.18`

---

### P10 - Complete Checkout

**Scenario:** Verify that the user can finish checkout successfully.

**Expected Result:**
- Checkout should complete successfully.
- Confirmation message should be displayed:
  - `Thank you for your order!`
- Cart badge should be cleared.

---

### P11 - Back Home After Order Completion

**Scenario:** Verify that the Back Home button works after order completion.

**Expected Result:**
- User should be redirected back to the Products page.

---

### P12 - Sort Products By Name A To Z

**Scenario:** Verify that products can be sorted by Name A to Z.

**Expected Result:**
- Products should be displayed in ascending alphabetical order.

---

### P13 - Sort Products By Name Z To A

**Scenario:** Verify that products can be sorted by Name Z to A.

**Expected Result:**
- Products should be displayed in descending alphabetical order.

---

### P14 - Sort Products By Price Low To High

**Scenario:** Verify that products can be sorted by price from low to high.

**Expected Result:**
- Products should be displayed from lowest price to highest price.
- Lowest observed price: `$7.99`
- Highest observed price: `$49.99`

---

### P15 - Sort Products By Price High To Low

**Scenario:** Verify that products can be sorted by price from high to low.

**Expected Result:**
- Products should be displayed from highest price to lowest price.
- Highest observed price: `$49.99`
- Lowest observed price: `$7.99`

---

### P16 - Open Product Detail Page

**Scenario:** Verify that clicking a product opens the product detail page.

**Expected Result:**
- Product detail page should open.
- Product name, description, price, and image should be displayed.
- Add to cart button should be available.
- Back to Products button should be available.

---

### P17 - Open Side Menu

**Scenario:** Verify that the side menu opens correctly.

**Expected Result:**
- Side menu should open.
- The following options should be visible:
  - All Items
  - About
  - Logout
  - Reset App State

---

### P18 - Logout From Application

**Scenario:** Verify that a logged-in user can logout successfully.

**Expected Result:**
- User should be logged out.
- User should be redirected to the login page.

---

## Negative Test Scenarios

### N01 - Login With Empty Username And Password

**Scenario:** Verify login validation when both username and password are empty.

**Expected Result:**
- Login should fail.
- Error message should be displayed:
  - `Epic sadface: Username is required`

---

### N02 - Login With Empty Username

**Scenario:** Verify login validation when username is empty and password is entered.

**Test Data:**
- Username: blank
- Password: `secret_sauce`

**Expected Result:**
- Login should fail.
- Error message should be displayed:
  - `Epic sadface: Username is required`

---

### N03 - Login With Empty Password

**Scenario:** Verify login validation when username is entered and password is empty.

**Test Data:**
- Username: `standard_user`
- Password: blank

**Expected Result:**
- Login should fail.
- Error message should be displayed:
  - `Epic sadface: Password is required`

---

### N04 - Login With Invalid Password

**Scenario:** Verify login validation when invalid credentials are entered.

**Test Data:**
- Username: `standard_user`
- Password: `bad_password`

**Expected Result:**
- Login should fail.
- Error message should be displayed:
  - `Epic sadface: Username and password do not match any user in this service`

---

### N05 - Login With Locked Out User

**Scenario:** Verify login behavior for locked out user.

**Test Data:**
- Username: `locked_out_user`
- Password: `secret_sauce`

**Expected Result:**
- Login should fail.
- Error message should be displayed:
  - `Epic sadface: Sorry, this user has been locked out.`

---

### N06 - Checkout With Empty First Name

**Scenario:** Verify checkout validation when first name is missing.

**Expected Result:**
- Checkout should not continue.
- Error message should be displayed:
  - `Error: First Name is required`

---

### N07 - Checkout With Empty Last Name

**Scenario:** Verify checkout validation when last name is missing.

**Expected Result:**
- Checkout should not continue.
- Error message should be displayed:
  - `Error: Last Name is required`

---

### N08 - Checkout With Empty Postal Code

**Scenario:** Verify checkout validation when postal code is missing.

**Expected Result:**
- Checkout should not continue.
- Error message should be displayed:
  - `Error: Postal Code is required`

---

### N09 - View Cart Without Adding Products

**Scenario:** Verify cart behavior when no product is added.

**Expected Result:**
- Cart page should open.
- No cart items should be displayed.
- Checkout button is still visible.

---

### N10 - Remove All Products Before Checkout

**Scenario:** Verify cart behavior after removing all selected products.

**Expected Result:**
- Cart should become empty.
- Cart badge should disappear.
- No products should be listed in the cart.

---

## Edge Test Scenarios

### E01 - Checkout With Empty Cart

**Scenario:** Verify behavior when user proceeds to checkout with an empty cart.

**Expected Result:**
- Checkout button is available even with an empty cart.
- User can navigate to the Checkout Information page.
- This should be reviewed as a possible business rule gap.

---

### E02 - Add All Products To Cart

**Scenario:** Verify cart behavior when all available products are added.

**Expected Result:**
- All six products should be added to the cart.
- Cart badge should show `6`.
- Cart page should display all six products.

---

### E03 - Remove All Products After Adding

**Scenario:** Verify that all added products can be removed.

**Expected Result:**
- All products should be removed successfully.
- Cart badge should disappear.
- Product buttons should return to Add to cart.

---

### E04 - Sort Products With Same Price

**Scenario:** Verify sorting behavior for products with the same price.

**Expected Result:**
- Products with the same price should remain visible.
- Sorting should not hide or duplicate products.

**Observed Same Price Products:**
- Sauce Labs Bolt T-Shirt: `$15.99`
- Test.allTheThings() T-Shirt (Red): `$15.99`

---

### E05 - Reset App State After Adding Products

**Scenario:** Verify Reset App State behavior from the side menu.

**Expected Result:**
- Cart should be cleared.
- Product buttons should reset to Add to cart.
- Cart badge should disappear.

---

### E06 - Direct Product Detail Navigation

**Scenario:** Verify behavior when navigating directly to a product detail page while logged in.

**Expected Result:**
- Product detail page should load successfully.
- Product information should be displayed correctly.

---

### E07 - Refresh Products Page After Login

**Scenario:** Verify session behavior after refreshing the Products page.

**Expected Result:**
- User should remain logged in.
- Products page should reload correctly.

---

### E08 - Enter Very Long Checkout Field Values

**Scenario:** Verify checkout form behavior with very long first name, last name, and postal code values.

**Expected Result:**
- Application should not crash.
- Layout should not break.
- Input should either be accepted or validated properly.

---

### E09 - Enter Special Characters In Checkout Fields

**Scenario:** Verify checkout form behavior with special characters.

**Test Data Examples:**
- First Name: `John@123`
- Last Name: `Doe#$%`
- Postal Code: `12@#45`

**Expected Result:**
- Application should handle input safely.
- No crash or layout issue should occur.
- Validation behavior should be consistent with requirements.

---

### E10 - Browser Back From Checkout Overview

**Scenario:** Verify behavior when user clicks browser Back from Checkout Overview.

**Expected Result:**
- User should return to Checkout Information page.
- Cart items should remain available.

---

## Traceability Matrix

### Authentication

**Covered By:**
- Positive: P01, P18
- Negative: N01, N02, N03, N04, N05
- Edge: E07

---

### Product Listing

**Covered By:**
- Positive: P02
- Edge: E04

---

### Product Detail

**Covered By:**
- Positive: P16
- Edge: E06

---

### Product Sorting

**Covered By:**
- Positive: P12, P13, P14, P15
- Edge: E04

---

### Cart Add And Remove

**Covered By:**
- Positive: P03, P04, P05, P06, P07
- Negative: N10
- Edge: E02, E03, E05

---

### Empty Cart Behavior

**Covered By:**
- Negative: N09
- Edge: E01

---

### Checkout Information Form

**Covered By:**
- Positive: P08
- Negative: N06, N07, N08
- Edge: E08, E09

---

### Checkout Overview

**Covered By:**
- Positive: P09
- Edge: E10

---

### Order Completion

**Covered By:**
- Positive: P10, P11

---

### Side Menu And Navigation

**Covered By:**
- Positive: P17, P18
- Edge: E05

---

## Verified Product Data

The following products were observed on the Products page:

1. Sauce Labs Backpack - `$29.99`
2. Sauce Labs Bike Light - `$9.99`
3. Sauce Labs Bolt T-Shirt - `$15.99`
4. Sauce Labs Fleece Jacket - `$49.99`
5. Sauce Labs Onesie - `$7.99`
6. Test.allTheThings() T-Shirt (Red) - `$15.99`

---

## Notes

- The application allows checkout navigation even when the cart is empty.
- Checkout form validates required fields one by one.
- Successful checkout displays the message `Thank you for your order!`.
- The side menu contains All Items, About, Logout, and Reset App State.

