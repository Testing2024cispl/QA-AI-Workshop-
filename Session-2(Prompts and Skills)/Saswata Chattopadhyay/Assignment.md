AI Manual Test Cases:- 
Member:-Saswata Chattopadhyay 

Prompt 1:- Write test cases for (https://v0-e-commerce-lunchbox-site.vercel.app/) 

Suppose, you are a manual Tester,

This is a ecommerce website where currently users have to add products to cart , go to checkout, and they can add promocode LUNCH20  which will apply 20% discount on listing price and then proceed to checkout . Now generate only the testcases for this particular flow. Make a table of three columns as testcase number, positive and negative testcases

Prompt 2: Vibe coding: Also in the cart page there are address section as well where the prospect fields included Street address, City and zip code and also a payment prospect field with card number, expiry year and CVV so now refine the tescases and please note that for the timebeing the website accepts only these test data for card details such as : number: 4242 4242 4242 4242 Expiry: 12/29 CVV: 100

# Human Written Test Cases

## Positive Test Cases

### TestCases_001

Checking if the the provided url is opening properly or not

Test Steps:

1. Go to https://v0-e-commerce-lunchbox-site.vercel.app/
2. Verify the website loads successfully.
3. Verify all sections are displayed properly.
4. Verify no broken images are present.
5. Verify no console errors are displayed.

---

### TestCases_002

User should be able to add products in the cart by clicking on add to cart

Test Steps:

1. Go to https://v0-e-commerce-lunchbox-site.vercel.app/
2. Select any product.
3. Click on Add to Cart.
4. Verify the product is added to the cart.
5. Verify the cart count is updated.

---

### TestCases_003

Users can add products multiple number of times which should reflect in the cart bubble counter

Test Steps:

1. Open the website.
2. Select any product.
3. Click Add to Cart multiple times.
4. Observe the cart bubble counter.
5. Verify the quantity matches the number of additions.

---

### TestCases_004

By clicking on the cart icon users should be able to land on to the cart page

Test Steps:

1. Open the website.
2. Add at least one product to the cart.
3. Click on the Cart icon.
4. Verify navigation to the cart page.

---

### TestCases_005

Validating each product prices properly with their respective product details pages

Test Steps:

1. Open the website.
2. Select a product.
3. Note the product price from the product details page.
4. Add the product to the cart.
5. Open the cart page.
6. Compare the prices displayed on both pages.

---

### TestCases_006

Checking quantity adder buttons by adding or removing quantities of a product

Test Steps:

1. Add a product to the cart.
2. Open the cart page.
3. Click the quantity increase button.
4. Verify the quantity increases.
5. Click the quantity decrease button.
6. Verify the quantity decreases.

---

### TestCases_007

In the address field validating zipcode field by giving proper credentials

Test Steps:

1. Add products to the cart.
2. Proceed to checkout.
3. Enter shipping details.
4. Enter a valid zip code.
5. Continue with the checkout process.

---

### TestCases_008

Validating if auto suggestions are appearing after user gives certain inputs into address field

Test Steps:

1. Proceed to checkout.
2. Click on the address field.
3. Enter partial address information.
4. Observe the auto-suggestion list.
5. Select a suggested address.

---

### TestCases_009

Validating card prospect fields by giving valid card number, expiry year and CVV

Test Steps:

1. Proceed to the payment section.
2. Enter a valid card number.
3. Enter a valid expiry month and year.
4. Enter a valid CVV.
5. Continue with payment.

---

### TestCases_010

Validating promocode by giving valid promo code (LUNCH20) to the promocode field

Test Steps:

1. Add products to the cart.
2. Proceed to checkout.
3. Enter promo code LUNCH20.
4. Click on Apply.
5. Verify the discount is applied.

---

### TestCases_011

Validating discounted price by manually calculating

Test Steps:

1. Add products to the cart.
2. Note the total amount before discount.
3. Apply promo code LUNCH20.
4. Calculate the discount manually.
5. Compare the manual calculation with the displayed discount.

---

### TestCases_012

Validating the submit CTA button label text where the total product price is showing and tally the total amount with products sum price which is present in the cart

Test Steps:

1. Add multiple products to the cart.
2. Note the individual product prices.
3. Calculate the total amount manually.
4. Proceed to checkout.
5. Verify the amount displayed on the Submit CTA button.

---

### TestCases_013

Validating the if the submit button is working properly or not

Test Steps:

1. Add products to the cart.
2. Complete all mandatory checkout details.
3. Enter valid payment information.
4. Click on the Submit button.
5. Verify the order submission process.

---

### TestCases_014

Verifying all the order details such as product prices, discounted prices etc and manual checking the price calculations

Test Steps:

1. Add multiple products to the cart.
2. Apply a valid promo code.
3. Proceed to checkout.
4. Review the order summary section.
5. Verify product prices, discounts and final amount calculations.

## Negative Test Cases

### TestCases_015

Try to attempt checkout by clearing out all the products from the cart

Test Steps:

1. Add products to the cart.
2. Open the cart page.
3. Remove all products from the cart.
4. Attempt to proceed to checkout.
5. Verify system behavior.

---

### TestCases_016

Try to get discount by applying an invalid promocode

Test Steps:

1. Add products to the cart.
2. Proceed to checkout.
3. Enter an invalid promo code.
4. Click Apply.
5. Verify system behavior.

---

### TestCases_017

Try to place order by giving invalid zip code, card number, CVV etc.

Test Steps:

1. Add products to the cart.
2. Proceed to checkout.
3. Enter an invalid zip code.
4. Enter an invalid card number.
5. Enter an invalid CVV.
6. Click Submit.

---

### TestCases_018

Try to place order by leaving address field empty

Test Steps:

1. Add products to the cart.
2. Proceed to checkout.
3. Leave the address field empty.
4. Fill other required fields.
5. Click Submit.

---

### TestCases_019

Try to place order by leaving card prospect field empty

Test Steps:

1. Add products to the cart.
2. Proceed to checkout.
3. Leave cardholder name empty.
4. Leave card number or CVV empty.
5. Click Submit.

---

### TestCases_020

Checking character length validation where user should not be able give more than 10 digits for phone number

Test Steps:

1. Proceed to checkout.
2. Enter more than 10 digits in the phone number field.
3. Attempt to continue.
4. Verify system behavior.

---

### TestCases_021

Checking character length validation where user should not be able give more than 16 digits for card number

Test Steps:

1. Proceed to payment section.
2. Enter more than 16 digits in the card number field.
3. Attempt to continue.
4. Verify system behavior.

---

### TestCases_022

Checking character length validation in CVV field where if amex card is present user should be able to give four digits

Test Steps:

1. Proceed to payment section.
2. Enter a valid American Express card number.
3. Enter a 4-digit CVV.
4. Continue with the payment process.
5. Verify system behavior.

---

### TestCases_023

Checking Expiry year validation where users should not be able to give invalid month or year

Test Steps:

1. Proceed to payment section.
2. Enter an invalid expiry month.
3. Enter an invalid expiry year.
4. Click Submit.
5. Verify system behavior.

---

### TestCases_024

Checking if multiple ajax is not firing from console in dev tools when users clicks on CTA button of submit while placing order

Test Steps:

1. Open browser Developer Tools.
2. Navigate to the Network tab.
3. Complete the checkout process.
4. Click the Submit CTA button once.
5. Observe the network requests generated.

---

### TestCases_025

Checking if any certain pages are getting 404 error from the backend when doing certain operations

Test Steps:

1. Navigate through all major pages of the website.
2. Add products to the cart.
3. Apply promo codes.
4. Proceed to checkout.
5. Monitor network requests and page navigation for any 404 errors.


AI Driven Test Cases

Positive Test Cases

TC-001
Add a product to cart successfully.

Test Steps:
1. Open website.
2. Perform the action described in the title.
3. Verify the behavior.

TC-002
Add multiple products to cart successfully.

Test Steps:
1. Open website.
2. Perform the action described in the title.
3. Verify the behavior.

TC-003
Update product quantity in cart and verify total updates correctly.

Test Steps:
1. Open website.
2. Perform the action described in the title.
3. Verify the behavior.

TC-004
Apply promo code LUNCH20 successfully.

Test Steps:
1. Open website.
2. Perform the action described in the title.
3. Verify the behavior.

TC-005
Verify 20% discount is calculated correctly on listing price.

Test Steps:
1. Open website.
2. Perform the action described in the title.
3. Verify the behavior.

TC-006
Verify discount amount is shown in order summary.

Test Steps:
1. Open website.
2. Perform the action described in the title.
3. Verify the behavior.

TC-007
Verify promo code remains applied after quantity change.

Test Steps:
1. Open website.
2. Perform the action described in the title.
3. Verify the behavior.

TC-008
Verify promo code remains applied after page refresh (if designed to persist).

Test Steps:
1. Open website.
2. Perform the action described in the title.
3. Verify the behavior.

TC-009
Enter valid Street Address and proceed.

Test Steps:
1. Open website.
2. Perform the action described in the title.
3. Verify the behavior.

TC-010
Enter valid City and proceed.

Test Steps:
1. Open website.
2. Perform the action described in the title.
3. Verify the behavior.
TC-011
Enter valid Zip Code and proceed.

Test Steps:
1. Open website.
2. Perform the action described in the title.
3. Verify the behavior.

TC-012
Enter alphanumeric address successfully.

Test Steps:
1. Open website.
2. Perform the action described in the title.
3. Verify the behavior.

TC-013
Enter city names with spaces (e.g., New York).

Test Steps:
1. Open website.
2. Perform the action described in the title.
3. Verify the behavior.

TC-014
Enter valid zip code format accepted by system.

Test Steps:
1. Open website.
2. Perform the action described in the title.
3. Verify the behavior.

TC-015
Verify address fields retain values after validation errors.

Test Steps:
1. Open website.
2. Perform the action described in the title.
3. Verify the behavior.

TC-016
Verify user can edit address before placing order.

Test Steps:
1. Open website.
2. Perform the action described in the title.
3. Verify the behavior.

TC-017
Enter valid card number 4242 4242 4242 4242.

Test Steps:
1. Open website.
2. Perform the action described in the title.
3. Verify the behavior.

TC-018
Enter valid expiry 12/29.

Test Steps:
1. Open website.
2. Perform the action described in the title.
3. Verify the behavior.

TC-019
Enter valid CVV 100.

Test Steps:
1. Open website.
2. Perform the action described in the title.
3. Verify the behavior.

TC-020
Complete payment using valid test card details.

Test Steps:
1. Open website.
2. Perform the action described in the title.
3. Verify the behavior.

TC-021
Verify order is placed successfully after valid payment.

Test Steps:
1. Open website.
2. Perform the action described in the title.
3. Verify the behavior.

TC-022
Verify final charged amount equals discounted total.

Test Steps:
1. Open website.
2. Perform the action described in the title.
3. Verify the behavior.

TC-023
Verify order confirmation page is displayed.

Test Steps:
1. Open website.
2. Perform the action described in the title.
3. Verify the behavior.

TC-024
Verify order summary displays product details correctly.

Test Steps:
1. Open website.
2. Perform the action described in the title.
3. Verify the behavior.

TC-025
Verify order summary displays address correctly.

Test Steps:
1. Open website.
2. Perform the action described in the title.
3. Verify the behavior.

TC-026
Verify order summary displays discount correctly.

Test Steps:
1. Open website.
2. Perform the action described in the title.
3. Verify the behavior.

TC-027
Verify successful checkout on Chrome.

Test Steps:
1. Open website.
2. Perform the action described in the title.
3. Verify the behavior.

TC-028
Verify successful checkout on mobile viewport.

Test Steps:
1. Open website.
2. Perform the action described in the title.
3. Verify the behavior.

TC-029
Verify successful checkout after changing address.

Test Steps:
1. Open website.
2. Perform the action described in the title.
3. Verify the behavior.

TC-030
Verify successful checkout after modifying cart quantity.

Test Steps:
1. Open website.
2. Perform the action described in the title.
3. Verify the behavior.

TC-031
Verify successful checkout with multiple products.

Test Steps:
1. Open website.
2. Perform the action described in the title.
3. Verify the behavior.

TC-032
Verify cart is cleared after successful order placement.

Test Steps:
1. Open website.
2. Perform the action described in the title.
3. Verify the behavior.

TC-033
Verify thank-you/order confirmation page loads correctly.

Test Steps:
1. Open website.
2. Perform the action described in the title.
3. Verify the behavior.

Negative Test Cases

TC-001
Attempt checkout with an empty cart.

Test Steps:
1. Open website.
2. Perform the invalid scenario.
3. Verify system behavior.
TC-002
Remove all products and attempt checkout.

Test Steps:
1. Open website.
2. Perform the invalid scenario.
3. Verify system behavior.
TC-003
Enter quantity beyond allowed limit (if applicable).

Test Steps:
1. Open website.
2. Perform the invalid scenario.
3. Verify system behavior.
TC-004
Enter invalid promo code.

Test Steps:
1. Open website.
2. Perform the invalid scenario.
3. Verify system behavior.
TC-005
Enter blank promo code and click Apply.

Test Steps:
1. Open website.
2. Perform the invalid scenario.
3. Verify system behavior.
TC-006
Apply promo code multiple times and verify discount is not stacked.

Test Steps:
1. Open website.
2. Perform the invalid scenario.
3. Verify system behavior.
TC-007
Verify discount is not greater than 20% after quantity changes.

Test Steps:
1. Open website.
2. Perform the invalid scenario.
3. Verify system behavior.
TC-008
Attempt to modify discount value through browser DevTools.

Test Steps:
1. Open website.
2. Perform the invalid scenario.
3. Verify system behavior.
TC-009
Leave Street Address blank.

Test Steps:
1. Open website.
2. Perform the invalid scenario.
3. Verify system behavior.
TC-010
Leave City blank.

Test Steps:
1. Open website.
2. Perform the invalid scenario.
3. Verify system behavior.
TC-011
Leave Zip Code blank.

Test Steps:
1. Open website.
2. Perform the invalid scenario.
3. Verify system behavior.
TC-012
Enter only special characters in Street Address.

Test Steps:
1. Open website.
2. Perform the invalid scenario.
3. Verify system behavior.
TC-013
Enter numeric values only in City field.

Test Steps:
1. Open website.
2. Perform the invalid scenario.
3. Verify system behavior.
TC-014
Enter zip code shorter than minimum length.

Test Steps:
1. Open website.
2. Perform the invalid scenario.
3. Verify system behavior.
TC-015
Enter zip code longer than maximum length.

Test Steps:
1. Open website.
2. Perform the invalid scenario.
3. Verify system behavior.
TC-016
Enter special characters in zip code if not allowed.

Test Steps:
1. Open website.
2. Perform the invalid scenario.
3. Verify system behavior.
TC-017
Enter invalid card number.

Test Steps:
1. Open website.
2. Perform the invalid scenario.
3. Verify system behavior.
TC-018
Leave card number blank.

Test Steps:
1. Open website.
2. Perform the invalid scenario.
3. Verify system behavior.
TC-019
Leave expiry blank.

Test Steps:
1. Open website.
2. Perform the invalid scenario.
3. Verify system behavior.
TC-020
Leave CVV blank.

Test Steps:
1. Open website.
2. Perform the invalid scenario.
3. Verify system behavior.
TC-021
Enter CVV with less than 3 digits.

Test Steps:
1. Open website.
2. Perform the invalid scenario.
3. Verify system behavior.
TC-022
Enter CVV with more than 3 digits.

Test Steps:
1. Open website.
2. Perform the invalid scenario.
3. Verify system behavior.
TC-023
Enter alphabetic characters in CVV.

Test Steps:
1. Open website.
2. Perform the invalid scenario.
3. Verify system behavior.
TC-024
Enter expired card date.

Test Steps:
1. Open website.
2. Perform the invalid scenario.
3. Verify system behavior.
TC-025
Enter invalid expiry format (e.g., 13/29).

Test Steps:
1. Open website.
2. Perform the invalid scenario.
3. Verify system behavior.
TC-026
Enter card number with incorrect length.

Test Steps:
1. Open website.
2. Perform the invalid scenario.
3. Verify system behavior.
TC-027
Enter card number containing alphabets.

Test Steps:
1. Open website.
2. Perform the invalid scenario.
3. Verify system behavior.
TC-028
Attempt payment with only partial card number entered.

Test Steps:
1. Open website.
2. Perform the invalid scenario.
3. Verify system behavior.
TC-029
Enter spaces only in payment fields.

Test Steps:
1. Open website.
2. Perform the invalid scenario.
3. Verify system behavior.
TC-030
Refresh page during payment submission.

Test Steps:
1. Open website.
2. Perform the invalid scenario.
3. Verify system behavior.
TC-031
Double-click Place Order and verify duplicate orders are not created.

Test Steps:
1. Open website.
2. Perform the invalid scenario.
3. Verify system behavior.
TC-032
Simulate payment gateway failure and verify proper error handling.

Test Steps:
1. Open website.
2. Perform the invalid scenario.
3. Verify system behavior.
TC-033
Disconnect internet during payment submission and verify recovery behavior.

Test Steps:
1. Open website.
2. Perform the invalid scenario.
3. Verify system behavior.



Your thoughts:- 
● What you felt Suitable:- For generating the edge cases the LLM's are much sufficient to perform properly 
● What you felt Not suitable:- The usual chatbots can't go through the url itself and generate url specific testcases if there are special cases as every ecommerce websites does.


Final Test Cases:-

Positive Test Cases

TC-001

Checking if the the provided url is opening properly or not
1. Go to https://v0-e-commerce-lunchbox-site.vercel.app/
2. Navigate to the relevant page or section.
3. Perform the action related to: Checking if the the provided url is opening properly or not
4. Verify the displayed information and calculations.
5. Proceed through checkout if applicable.
6. Confirm the behavior matches the intended flow.

TC-002
User should be able to add products in the cart by clicking on add to cart
1. Go to https://v0-e-commerce-lunchbox-site.vercel.app/
2. Navigate to the relevant page or section.
3. Perform the action related to: User should be able to add products in the cart by clicking on add to cart
4. Verify the displayed information and calculations.
5. Proceed through checkout if applicable.
6. Confirm the behavior matches the intended flow.

TC-003
They can add products multiple number of times which should reflect in the cart bubble counter
1. Go to https://v0-e-commerce-lunchbox-site.vercel.app/
2. Navigate to the relevant page or section.
3. Perform the action related to: They can add products multiple number of times which should reflect in the cart bubble counter
4. Verify the displayed information and calculations.
5. Proceed through checkout if applicable.
6. Confirm the behavior matches the intended flow.

TC-004
By clicking on the cart icon users should be able to land on to the cart page
1. Go to https://v0-e-commerce-lunchbox-site.vercel.app/
2. Navigate to the relevant page or section.
3. Perform the action related to: By clicking on the cart icon users should be able to land on to the cart page
4. Verify the displayed information and calculations.
5. Proceed through checkout if applicable.
6. Confirm the behavior matches the intended flow.

TC-005
Validating each product prices properly with their respective product details pages
1. Go to https://v0-e-commerce-lunchbox-site.vercel.app/
2. Navigate to the relevant page or section.
3. Perform the action related to: Validating each product prices properly with their respective product details pages
4. Verify the displayed information and calculations.
5. Proceed through checkout if applicable.
6. Confirm the behavior matches the intended flow.

TC-006
Checking quantity adder buttons by adding or removing quantities of a product
1. Go to https://v0-e-commerce-lunchbox-site.vercel.app/
2. Navigate to the relevant page or section.
3. Perform the action related to: Checking quantity adder buttons by adding or removing quantities of a product
4. Verify the displayed information and calculations.
5. Proceed through checkout if applicable.
6. Confirm the behavior matches the intended flow.

TC-007
In the address field validating zipcode field by giving proper credentials
1. Go to https://v0-e-commerce-lunchbox-site.vercel.app/
2. Navigate to the relevant page or section.
3. Perform the action related to: In the address field validating zipcode field by giving proper credentials
4. Verify the displayed information and calculations.
5. Proceed through checkout if applicable.
6. Confirm the behavior matches the intended flow.

TC-008
Validating if auto suggestions are appearing after user gives certain inputs into address field
1. Go to https://v0-e-commerce-lunchbox-site.vercel.app/
2. Navigate to the relevant page or section.
3. Perform the action related to: Validating if auto suggestions are appearing after user gives certain inputs into address field
4. Verify the displayed information and calculations.
5. Proceed through checkout if applicable.
6. Confirm the behavior matches the intended flow.

TC-009
Validating card prospect fields by giving vaid card number, expiry year and CVV
1. Go to https://v0-e-commerce-lunchbox-site.vercel.app/
2. Navigate to the relevant page or section.
3. Perform the action related to: Validating card prospect fields by giving vaid card number, expiry year and CVV
4. Verify the displayed information and calculations.
5. Proceed through checkout if applicable.
6. Confirm the behavior matches the intended flow.

TC-010
Validating promocode by giving valid promo code(LUNCH20) to the promocode field
1. Go to https://v0-e-commerce-lunchbox-site.vercel.app/
2. Navigate to the relevant page or section.
3. Perform the action related to: Validating promocode by giving valid promo code(LUNCH20) to the promocode field
4. Verify the displayed information and calculations.
5. Proceed through checkout if applicable.
6. Confirm the behavior matches the intended flow.

TC-011
Validating discounted price by manually calculating
1. Go to https://v0-e-commerce-lunchbox-site.vercel.app/
2. Navigate to the relevant page or section.
3. Perform the action related to: Validating discounted price by manually calculating
4. Verify the displayed information and calculations.
5. Proceed through checkout if applicable.
6. Confirm the behavior matches the intended flow.

TC-012
Validating the submit CTA button label text where the total product price is showing and tally the total amount with products sum price which is present in the cart
1. Go to https://v0-e-commerce-lunchbox-site.vercel.app/
2. Navigate to the relevant page or section.
3. Perform the action related to: Validating the submit CTA button label text where the total product price is showing and tally the total amount with products sum price which is present in the cart
4. Verify the displayed information and calculations.
5. Proceed through checkout if applicable.
6. Confirm the behavior matches the intended flow.

TC-013
Validating the if the submit button is working properly or not
1. Go to https://v0-e-commerce-lunchbox-site.vercel.app/
2. Navigate to the relevant page or section.
3. Perform the action related to: Validating the if the submit button is working properly or not
4. Verify the displayed information and calculations.
5. Proceed through checkout if applicable.
6. Confirm the behavior matches the intended flow.

TC-014
Verify order summary displays product details correctly.
1. Go to https://v0-e-commerce-lunchbox-site.vercel.app/
2. Navigate to the relevant page or section.
3. Perform the action related to: Verify order summary displays product details correctly.
4. Verify the displayed information and calculations.
5. Proceed through checkout if applicable.
6. Confirm the behavior matches the intended flow.

TC-015
Verify order summary displays address correctly.
1. Go to https://v0-e-commerce-lunchbox-site.vercel.app/
2. Navigate to the relevant page or section.
3. Perform the action related to: Verify order summary displays address correctly.
4. Verify the displayed information and calculations.
5. Proceed through checkout if applicable.
6. Confirm the behavior matches the intended flow.

TC-016
Verify order summary displays discount correctly.
1. Go to https://v0-e-commerce-lunchbox-site.vercel.app/
2. Navigate to the relevant page or section.
3. Perform the action related to: Verify order summary displays discount correctly.
4. Verify the displayed information and calculations.
5. Proceed through checkout if applicable.
6. Confirm the behavior matches the intended flow.

TC-017
Verify successful checkout on Chrome.
1. Go to https://v0-e-commerce-lunchbox-site.vercel.app/
2. Navigate to the relevant page or section.
3. Perform the action related to: Verify successful checkout on Chrome.
4. Verify the displayed information and calculations.
5. Proceed through checkout if applicable.
6. Confirm the behavior matches the intended flow.

TC-018
Verify cart is cleared after successful order placement.
1. Go to https://v0-e-commerce-lunchbox-site.vercel.app/
2. Navigate to the relevant page or section.
3. Perform the action related to: Verify cart is cleared after successful order placement.
4. Verify the displayed information and calculations.
5. Proceed through checkout if applicable.
6. Confirm the behavior matches the intended flow.

TC-019
Verify thank-you/order confirmation page loads correctly.
1. Go to https://v0-e-commerce-lunchbox-site.vercel.app/
2. Navigate to the relevant page or section.
3. Perform the action related to: Verify thank-you/order confirmation page loads correctly.
4. Verify the displayed information and calculations.
5. Proceed through checkout if applicable.
6. Confirm the behavior matches the intended flow.

TC-020
Verifying all the order summary details such as product prices, discounted prices etc and manuall checking the price calculations
1. Go to https://v0-e-commerce-lunchbox-site.vercel.app/
2. Navigate to the relevant page or section.
3. Perform the action related to: Verifying all the order summary details such as product prices, discounted prices etc and manuall checking the price calculations
4. Verify the displayed information and calculations.
5. Proceed through checkout if applicable.
6. Confirm the behavior matches the intended flow.

Negative Test Cases

TC-001
Try to attempt checkout by clearing out all the products from the cart
1. Go to https://v0-e-commerce-lunchbox-site.vercel.app/
2. Navigate to the relevant checkout or payment section.
3. Perform the invalid scenario: Try to attempt checkout by clearing out all the products from the cart
4. Observe validation messages and application behavior.
5. Monitor browser console/network requests if applicable.
6. Verify the application handles the scenario appropriately.

TC-002
Try to get discount by applying an invalid promocode
1. Go to https://v0-e-commerce-lunchbox-site.vercel.app/
2. Navigate to the relevant checkout or payment section.
3. Perform the invalid scenario: Try to get discount by applying an invalid promocode
4. Observe validation messages and application behavior.
5. Monitor browser console/network requests if applicable.
6. Verify the application handles the scenario appropriately.

TC-003
Try to place order by giving invalid zip code, card number, CVV etc.
1. Go to https://v0-e-commerce-lunchbox-site.vercel.app/
2. Navigate to the relevant checkout or payment section.
3. Perform the invalid scenario: Try to place order by giving invalid zip code, card number, CVV etc.
4. Observe validation messages and application behavior.
5. Monitor browser console/network requests if applicable.
6. Verify the application handles the scenario appropriately.

TC-004
Try to place order by leaving address field empty
1. Go to https://v0-e-commerce-lunchbox-site.vercel.app/
2. Navigate to the relevant checkout or payment section.
3. Perform the invalid scenario: Try to place order by leaving address field empty
4. Observe validation messages and application behavior.
5. Monitor browser console/network requests if applicable.
6. Verify the application handles the scenario appropriately.

TC-005
Try to place order by leaving card prospect field empty
1. Go to https://v0-e-commerce-lunchbox-site.vercel.app/
2. Navigate to the relevant checkout or payment section.
3. Perform the invalid scenario: Try to place order by leaving card prospect field empty
4. Observe validation messages and application behavior.
5. Monitor browser console/network requests if applicable.
6. Verify the application handles the scenario appropriately.

TC-006
Checking character length validation where user should not be able give more and less than 10 digits for phone number
1. Go to https://v0-e-commerce-lunchbox-site.vercel.app/
2. Navigate to the relevant checkout or payment section.
3. Perform the invalid scenario: Checking character length validation where user should not be able give more and less than 10 digits for phone number
4. Observe validation messages and application behavior.
5. Monitor browser console/network requests if applicable.
6. Verify the application handles the scenario appropriately.

TC-007
Checking character length validation where user should not be able give more and less than 16 digits for card number
1. Go to https://v0-e-commerce-lunchbox-site.vercel.app/
2. Navigate to the relevant checkout or payment section.
3. Perform the invalid scenario: Checking character length validation where user should not be able give more and less than 16 digits for card number
4. Observe validation messages and application behavior.
5. Monitor browser console/network requests if applicable.
6. Verify the application handles the scenario appropriately.

TC-008
Checking character length validation in CVV field where if amex card is present user should be able to give four digits
1. Go to https://v0-e-commerce-lunchbox-site.vercel.app/
2. Navigate to the relevant checkout or payment section.
3. Perform the invalid scenario: Checking character length validation in CVV field where if amex card is present user should be able to give four digits
4. Observe validation messages and application behavior.
5. Monitor browser console/network requests if applicable.
6. Verify the application handles the scenario appropriately.

TC-009
Checking Expiry year validation where users should not be able to give invalid month or year
1. Go to https://v0-e-commerce-lunchbox-site.vercel.app/
2. Navigate to the relevant checkout or payment section.
3. Perform the invalid scenario: Checking Expiry year validation where users should not be able to give invalid month or year
4. Observe validation messages and application behavior.
5. Monitor browser console/network requests if applicable.
6. Verify the application handles the scenario appropriately.

TC-010
Checking if multiple ajax is not firing from console in dev tools when users clicks on CTA button of submit while placing order
1. Go to https://v0-e-commerce-lunchbox-site.vercel.app/
2. Navigate to the relevant checkout or payment section.
3. Perform the invalid scenario: Checking if multiple ajax is not firing from console in dev tools when users clicks on CTA button of submit while placing order
4. Observe validation messages and application behavior.
5. Monitor browser console/network requests if applicable.
6. Verify the application handles the scenario appropriately.

TC-011
Checking if any certain pages are getting 404 error from the backend when doing certain operations
1. Go to https://v0-e-commerce-lunchbox-site.vercel.app/
2. Navigate to the relevant checkout or payment section.
3. Perform the invalid scenario: Checking if any certain pages are getting 404 error from the backend when doing certain operations
4. Observe validation messages and application behavior.
5. Monitor browser console/network requests if applicable.
6. Verify the application handles the scenario appropriately.

TC-012
Enter card number containing alphabets.
1. Go to https://v0-e-commerce-lunchbox-site.vercel.app/
2. Navigate to the relevant checkout or payment section.
3. Perform the invalid scenario: Enter card number containing alphabets.
4. Observe validation messages and application behavior.
5. Monitor browser console/network requests if applicable.
6. Verify the application handles the scenario appropriately.

TC-013
Attempt payment with only partial card number entered.
1. Go to https://v0-e-commerce-lunchbox-site.vercel.app/
2. Navigate to the relevant checkout or payment section.
3. Perform the invalid scenario: Attempt payment with only partial card number entered.
4. Observe validation messages and application behavior.
5. Monitor browser console/network requests if applicable.
6. Verify the application handles the scenario appropriately.

TC-014
Enter spaces only in payment fields.
1. Go to https://v0-e-commerce-lunchbox-site.vercel.app/
2. Navigate to the relevant checkout or payment section.
3. Perform the invalid scenario: Enter spaces only in payment fields.
4. Observe validation messages and application behavior.
5. Monitor browser console/network requests if applicable.
6. Verify the application handles the scenario appropriately.

TC-015
Refresh page during payment submission.
1. Go to https://v0-e-commerce-lunchbox-site.vercel.app/
2. Navigate to the relevant checkout or payment section.
3. Perform the invalid scenario: Refresh page during payment submission.
4. Observe validation messages and application behavior.
5. Monitor browser console/network requests if applicable.
6. Verify the application handles the scenario appropriately.

TC-016
Double-click Place Order and verify duplicate orders are not created.
1. Go to https://v0-e-commerce-lunchbox-site.vercel.app/
2. Navigate to the relevant checkout or payment section.
3. Perform the invalid scenario: Double-click Place Order and verify duplicate orders are not created.
4. Observe validation messages and application behavior.
5. Monitor browser console/network requests if applicable.
6. Verify the application handles the scenario appropriately.

TC-017
Simulate payment gateway failure and verify proper error handling.
1. Go to https://v0-e-commerce-lunchbox-site.vercel.app/
2. Navigate to the relevant checkout or payment section.
3. Perform the invalid scenario: Simulate payment gateway failure and verify proper error handling.
4. Observe validation messages and application behavior.
5. Monitor browser console/network requests if applicable.
6. Verify the application handles the scenario appropriately.

TC-018
Disconnect internet during payment submission and verify recovery behavior.
1. Go to https://v0-e-commerce-lunchbox-site.vercel.app/
2. Navigate to the relevant checkout or payment section.
3. Perform the invalid scenario: Disconnect internet during payment submission and verify recovery behavior.
4. Observe validation messages and application behavior.
5. Monitor browser console/network requests if applicable.
6. Verify the application handles the scenario appropriately.

TC-019
Apply promo code multiple times and verify discount is not stacked.
1. Go to https://v0-e-commerce-lunchbox-site.vercel.app/
2. Navigate to the relevant checkout or payment section.
3. Perform the invalid scenario: Apply promo code multiple times and verify discount is not stacked.
4. Observe validation messages and application behavior.
5. Monitor browser console/network requests if applicable.
6. Verify the application handles the scenario appropriately.

TC-020
Verify discount is not greater than 20% after quantity changes.
1. Go to https://v0-e-commerce-lunchbox-site.vercel.app/
2. Navigate to the relevant checkout or payment section.
3. Perform the invalid scenario: Verify discount is not greater than 20% after quantity changes.
4. Observe validation messages and application behavior.
5. Monitor browser console/network requests if applicable.
6. Verify the application handles the scenario appropriately.

TC-021
Attempt to modify discount value through browser DevTools.
1. Go to https://v0-e-commerce-lunchbox-site.vercel.app/
2. Navigate to the relevant checkout or payment section.
3. Perform the invalid scenario: Attempt to modify discount value through browser DevTools.
4. Observe validation messages and application behavior.
5. Monitor browser console/network requests if applicable.
6. Verify the application handles the scenario appropriately.

TC-022
Enter only special characters in Street Address.
1. Go to https://v0-e-commerce-lunchbox-site.vercel.app/
2. Navigate to the relevant checkout or payment section.
3. Perform the invalid scenario: Enter only special characters in Street Address.
4. Observe validation messages and application behavior.
5. Monitor browser console/network requests if applicable.
6. Verify the application handles the scenario appropriately.

===================================================================================

# QA Skill File — Ecommerce Project Test Case Generation

## Purpose
This skill file defines a strict, reusable format for generating consistent test cases across any module (login, cart, checkout, payment, API, etc.).

---

## AI INSTRUCTION (STRICT RULES)
- Output ONLY the test case table.
- Do NOT add explanations, notes, or extra text.
- Use the exact column structure defined below.
- Ensure each test case is atomic and independently executable.
- Include both positive and negative scenarios when applicable.
- Maintain consistent naming conventions for Test Case IDs.

---

## TEST CASE FORMAT (DO NOT MODIFY STRUCTURE)

| Test Case ID | Scenario | Preconditions | Test Steps | Test Data | Expected Result | Priority | Type |
|--------------|----------|---------------|------------|-----------|-----------------|----------|------|

---

## COLUMN DEFINITIONS

- Test Case ID → Unique identifier (TC-001, TC-002...)
- Scenario → What is being tested (single line)
- Preconditions → Required setup before execution
- Test Steps → Step-by-step actions (use <br> for line breaks)
- Test Data → Input values used in test
- Expected Result → System behavior after execution
- Priority → High / Medium / Low
- Type → Positive / Negative / Edge / Regression

---

## EXAMPLE (FOR REFERENCE ONLY — DO NOT OUTPUT DURING GENERATION)

| Test Case ID | Scenario | Preconditions | Test Steps | Test Data | Expected Result | Priority | Type |
|--------------|----------|---------------|------------|-----------|-----------------|----------|------|
| TC-001 | Verify user login with valid credentials | User must be registered | 1. Open login page<br>2. Enter username<br>3. Enter password<br>4. Click login | user=test, pass=1234 | User should login successfully | High | Positive |

---

## REUSABILITY
This format applies to:
- Login Module
- Signup Module
- Cart Module
- Checkout Module
- Payment Module
- API Testing
- Admin Panels
- Any future feature modules


