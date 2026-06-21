QA Manual Test Cases:-

Member 1:- Sourav Banik
Query/Test cases:- https://rahulshettyacademy.com/seleniumPractise/#/ 


Human Thinking Test Cases
TestCases_001:- Search Functionality for valid product. 
Click on the Search field. 
Type “Brocolli”. 



TestCases_002:- Search Functionality for invalid product. 
Click on the Search field. 
Type “123Bro#$”. 


TestCases_003:- Count checking for positive count. 
Click on the count field on the product section. 
Write “2” or “3” or “5” as count. 


TestCases_004:- Count checking for negative count. 
Click on the count field on the product section. 
Write “-2” or “-3” or “-5” as count. 



TestCases_005:- Count checking for alphabets and special characters.
Click on the count field on the product section. 
Write “a” or “#” or “a%”. 



TestCases_006:- Order process with valid count with Terms & Conditions checkbox checked . 
Click on the “+” button to increase the count. 
Click on Add to cart button. 
Click on the Cart button. 
Click on the Proceed to checkout button. 
Click on the place order button. 
Choose a country as “India”. 
Tick the checkbox of the Terms & Conditions. 
Click on the Proceed button. 




TestCases_007:- Order process with valid count with Terms & Conditions checkbox unchecked. 
Click on the “+” button to increase the count. 
Click on Add to cart button. 
Click on the Cart button. 
Click on the Proceed to checkout button. 
Click on the place order button. 
Choose a country as “India”. 
Untick the checkbox of the Terms & Conditions. 
Click on the Proceed button.



TestCases_008:- Order process with valid count with selecting Country . 
Click on the “+” button to increase the count. 
Click on Add to cart button. 
Click on the Cart button. 
Click on the Proceed to checkout button. 
Click on the place order button. 
Choose a country as “India”. 
Tick the checkbox of the Terms & Conditions. 
Click on the Proceed button.



TestCases_009:- Order process with valid count without selecting Country . 
Click on the “+” button to increase the count. 
Click on Add to cart button. 
Click on the Cart button. 
Click on the Proceed to checkout button. 
Click on the place order button. 
Do not Choose a country. 
Tick the checkbox of the Terms & Conditions. 
Click on the Proceed button.



TestCases_0010:- Order process with valid count with Terms & Conditions checkbox checked . 
Click on the “+” button to increase the count. 
Click on Add to cart button. 
Click on the Cart button. 
Click on the Proceed to checkout button. 
Click on the place order button. 
Choose a country as “India”. 
Tick the checkbox of the Terms & Conditions. 
Click on the Proceed button.


TestCases_0011:- Order process with invalid count(negative count) . 
Click on the count field on the product section. 
Write “-2” or “-3” or “-5” as count. 
Click on Add to cart button. 
Click on the Cart button. 
Click on the Proceed to checkout button. 
Click on the place order button. 
Choose a country as “India”. 
Tick the checkbox of the Terms & Conditions. 
Click on the Proceed button.



TestCases_0012:- Order process with invalid characters(alphabets & special characters)
Click on the count field on the product section. 
Write “a” or “#” or “a%”. 
Click on Add to cart button. 
Click on the Cart button. 
Click on the Proceed to checkout button. 
Click on the place order button. 
Choose a country as “India”. 
Tick the checkbox of the Terms & Conditions. 
Click on the Proceed button. 







AI Manual Test Cases:-

Member 1:- Sourav Banik
Prompt:- Act as a Senior QA Engineer. Analyze the application: https://rahulshettyacademy.com/seleniumPractise/#/ 
Generate all possible Functional Test Cases (Positive & Negative) with complete coverage of the application, excluding: 
Top Deals 
Flight Booking 

Include test cases for:
Product listing 
Search functionality 
Quantity increase/decrease 
Add to Cart 
Cart preview 
Cart updates 
Checkout Promo Code 
Price and discount calculations 
Country selection 
Place Order 
Success/Error messages 
Empty cart scenarios 

Requirements: 
Cover all valid, invalid, edge scenarios. 
Do not include UI, Security, Performance, Compatibility, or Accessibility test cases. 
Avoid duplicate test cases. 
Give in Document format, no in a tabular format. 


1. Product Listing
TC-PL-01: Verify all products are displayed on page load

Steps:

Launch the application.
Observe the product section. 


TC-PL-02: Verify each product displays name, quantity controls, and Add to Cart button

Steps:

Open the application.
Verify details of every listed product. 


TC-PL-03: Verify product names are unique

Steps:

Review all displayed products.
Check for duplicate product names.


TC-PL-04: Verify product listing loads successfully after page refresh

Steps:

Refresh the page.
Verify products are displayed correctly.


2. Search Functionality
TC-SR-01: Search using complete valid product name

Steps:

Enter the exact product name in the search field.
Verify matching products are displayed.



TC-SR-02: Search using partial product name

Steps:

Enter partial text.
Verify relevant products appear.

TC-SR-03: Search using lowercase characters

Steps:

Enter lowercase product name.
Verify results are displayed.


TC-SR-04: Search using uppercase characters

Steps:

Enter uppercase product name.
Verify matching results.


TC-SR-06: Search using single character

Steps:

Enter one character.
Verify relevant products appear.


TC-SR-07: Search with leading spaces

Steps:

Enter spaces before the product name.
Verify valid results.


TC-SR-09: Search with special characters only

Steps:

Enter special characters.
Verify no matching products.


TC-SR-10: Search with numeric values

Steps:

Enter numbers.
Verify no matching products.


TC-SR-11: Search with invalid product name

Steps:

Enter non-existing product name.
Verify no products displayed.



TC-SR-12: Search with blank input

Steps:

Clear search field.
Verify all products appear.



3. Quantity Increase / Decrease
TC-QT-01: Increase quantity by one

Steps:

Click '+' once.
Verify quantity becomes 2.


TC-QT-02: Increase quantity multiple times

Steps:

Click '+' repeatedly.
Verify quantity increments correctly.


TC-QT-03: Decrease quantity from value greater than 1

Steps:

Increase quantity.
Click '-'.
Verify quantity decreases.



TC-QT-04: Verify quantity cannot become zero

Steps:

Keep clicking '-'.
Verify minimum quantity remains 1.


TC-QT-05: Verify quantity cannot become negative

Steps:

Continue clicking '-'.
Verify negative values are not allowed.



TC-QT-06: Verify quantity selection remains before Add to Cart

Steps:

Set quantity.
Verify selected value remains displayed.



TC-QT-07: Verify large quantity selection

Steps:

Click '+' many times.
Verify quantity updates correctly.



4. Add to Cart
TC-AC-01: Add single product with default quantity

Steps:

Click Add to Cart.
Verify product added.


TC-AC-02: Add product with increased quantity

Steps:

Increase quantity.
Click Add to Cart.
Verify selected quantity added.



TC-AC-03: Add multiple different products

Steps:

Add different products.
Verify all appear in the cart.


TC-AC-04: Add same product multiple times

Steps:

Add same product repeatedly.
Verify cart updates correctly.



TC-AC-05: Verify cart count updates after addition

Steps:

Add products.
Verify cart count increases.


TC-AC-06: Add products after searching

Steps:

Search product.
Add product.
Verify successful addition.


5. Cart Preview
TC-CP-01: Open cart preview with one product

Steps:

Add a product.
Open cart preview.
Verify product details displayed.


TC-CP-02: Open cart preview with multiple products

Steps:

Add multiple products.
Open cart preview.
Verify all products listed.


TC-CP-03: Verify product quantity displayed correctly

Steps:

Add product with custom quantity.
Open cart.
Verify quantity.


TC-CP-04: Verify product price displayed correctly

Steps:

Add product.
Open cart.
Verify price information.




TC-CP-05: Verify total amount displayed correctly

Steps:

Add products.
Open cart.
Verify total amount.


TC-CP-06: Verify empty cart preview

Steps:

Open cart without adding products.
Verify empty state.



6. Cart Updates
TC-CU-01: Remove product from cart

Steps:

Add product.
Remove from cart.
Verify removal.



TC-CU-02: Remove one product from multiple products

Steps:

Add multiple products.
Remove one.
Verify remaining products exist.








TC-CU-03: Remove all products

Steps:

Remove all items.
Verify cart becomes empty.



TC-CU-04: Verify cart count updates after removal

Steps:

Remove product.
Verify cart count decreases.



TC-CU-05: Verify total amount updates after removal

Steps:

Remove product.
Verify re-calculated total.



7. Checkout
TC-CO-01: Proceed to checkout with one product

Steps:

Add product.
Click Proceed to Checkout.
Verify checkout page opens.



TC-CO-02: Proceed to checkout with multiple products

Steps:

Add products.
Proceed to checkout.
Verify all products displayed.



TC-CO-03: Verify product details on checkout page

Steps:

Open checkout.
Verify names, quantities, prices.



TC-CO-04: Verify total amount on checkout page

Steps:

Add products.
Open checkout.
Verify total amount.



TC-CO-05: Attempt checkout from empty cart

Steps:

Ensure the cart is empty.
Attempt checkout.
Verify expected behavior.



8. Promo Code
TC-PC-01: Apply valid promo code

Steps:

Enter valid promo code.
Click Apply.
Verify discount applied.



TC-PC-02: Apply invalid promo code

Steps:

Enter invalid code.
Click Apply.
Verify error message.



TC-PC-03: Apply blank promo code

Steps:

Leave the field empty.
Click Apply.
Verify validation/error message.



TC-PC-04: Apply same promo code multiple times

Steps:

Apply valid code.
Re-apply code.
Verify proper handling.



TC-PC-07: Verify discount reflected in total amount

Steps:

Apply valid code.
Verify total updates.


9. Price & Discount Calculations
TC-PD-01: Verify single product price calculation

Steps:

Add one product.
Verify total equals product price.



TC-PD-02: Verify multiple product total calculation

Steps:

Add multiple products.
Verify sum calculation.



TC-PD-03: Verify quantity-based calculation

Steps:

Increase quantity.
Add product.
Verify total.



TC-PD-04: Verify checkout total matches cart total

Steps:

Compare cart and checkout values.
Verify consistency.



TC-PD-05: Verify discounted total after promo code

Steps:

Apply promo.
Verify reduced total.






TC-PD-06: Verify discount amount calculation

Steps:

Apply promo.
Verify discount amount accuracy.


TC-PD-07: Verify total never becomes negative

Steps:

Apply available discounts.
Verify total remains valid.



10. Country Selection
TC-CS-01: Select valid country from dropdown

Steps:

Open country dropdown.
Select country.
Verify selection.


TC-CS-02: Change selected country

Steps:

Select one country.
Select another.
Verify updated value.



TC-CS-03: Attempt order without country selection

Steps:

Leave the country unselected.
Place order.
Verify validation.

11. Place Order
TC-PO-01: Place order with valid data

Steps:

Add products.
Select country.
Place order.
Verify success.



TC-PO-02: Place order with single product

Steps:

Add one product.
Complete order.
Verify success.



TC-PO-03: Place order with multiple products

Steps:

Add multiple products.
Complete order.
Verify success.



TC-PO-04: Attempt order without country selection

Steps:

Skip country.
Place order.
Verify validation.




TC-PO-05: Attempt order with empty cart

Steps:

Keep the cart empty.
Attempt order.
Verify prevention.



12. Success & Error Messages
TC-MSG-01: Verify success message after valid order

Steps:

Complete purchase.
Verify success confirmation.



TC-MSG-02: Verify message after valid promo code

Steps:

Apply valid code.
Verify the success message.



TC-MSG-03: Verify message after invalid promo code

Steps:

Apply invalid code.
Verify error message.



TC-MSG-04: Verify message for blank promo code

Steps:

Apply blank code.
Verify validation message.
TC-MSG-05: Verify message when no search result found

Steps:

Search invalid product.
Verify no-result indication.




13. Empty Cart Scenarios
TC-EC-01: Open cart when empty

Steps:

Open cart without products.
Verify empty state.




TC-EC-02: Verify order cannot be placed from empty cart

Steps:

Do not add products.
Attempt order.
Verify prevention.



TC-EC-03: Remove last product and verify empty cart state

Steps:

Add product.
Remove it.
Verify empty cart.






TC-EC-05: Verify cart count becomes zero after removing all products

Steps:

Remove all products.
Verify cart count resets.



TC-EC-06: Verify totals become zero after cart is emptied

Steps:

Remove all items.
Verify totals are cleared/reset.







Your thoughts:-

● What you felt Suitable:- 

AI gives so many edge cases. 
Gives extra scenarios. 
Reduces time. 


● What you felt Not suitable:- 
Gives few duplicate test cases. 
Gives few unnecessary test cases. 
Sometimes it hallucinates. 





Final Test Case:-

AI+Manual, Combine them and make a proper test case
for Automation ready.

AI+Manual, Combine them and make a proper test case for Automation ready
1. Product Listing
TC-PL-01: Verify all products are displayed on page load
Steps:
Launch the application.
Observe the product section.
Count the displayed products.
Expected Result:
All available products should be displayed successfully.

TC-PL-02: Verify each product displays mandatory details
Steps:
Open the application.
Check each product card.
Expected Result:
Each product should display:
Product Name
Quantity Controls (+/-)
Add to Cart Button

TC-PL-03: Verify product names are unique
Steps:
Review all displayed products.
Compare product names.
Expected Result:
No duplicate product names should exist.

TC-PL-04: Verify product listing after page refresh
Steps:
Refresh the page.
Observe the product section.
Expected Result:
All products should load successfully after refresh.

2. Search Functionality
TC-SR-01: Search using valid product name
Steps:
Click Search field.
Enter "Brocolli".
Expected Result:
Matching product should be displayed.

TC-SR-02: Search using partial product name
Steps:
Enter partial text such as "Broc".
Expected Result:
Relevant matching products should appear.

TC-SR-03: Search using uppercase/lowercase characters
Steps:
Search using uppercase text.
Search using lowercase text.
Expected Result:
Search should be case-insensitive.

TC-SR-04: Search using single character
Steps:
Enter a single alphabet.
Expected Result:
Relevant products should appear.

TC-SR-05: Search using invalid product name
Steps:
Enter "123Bro#$".
Expected Result:
No products should be displayed.

TC-SR-06: Search using numeric values
Steps:
Enter "12345".
Expected Result:
No matching products should appear.

TC-SR-07: Search using special characters
Steps:
Enter "@#$%^".
Expected Result:
No matching products should appear.

TC-SR-08: Search with leading/trailing spaces
Steps:
Enter spaces before or after a valid product name.
Expected Result:
Search should return valid results.

TC-SR-09: Search with blank input
Steps:
Clear search field.
Expected Result:
All products should be displayed.

3. Quantity Management
TC-QT-01: Increase quantity by one
Steps:
Click "+" once.
Expected Result:
Quantity should increase from 1 to 2.

TC-QT-02: Increase quantity multiple times
Steps:
Click "+" repeatedly.
Expected Result:
Quantity should be incremented correctly.

TC-QT-03: Decrease quantity
Steps:
Increase quantity.
Click "-".
Expected Result:
Quantity should decrease correctly.

TC-QT-04: Verify quantity cannot become zero
Steps:
Continuously click "-".
Expected Result:
Minimum quantity should remain 1.

TC-QT-05: Verify quantity cannot become negative
Steps:
Continue clicking "-".
Expected Result:
Negative quantities should not be allowed.

TC-QT-06: Verify invalid negative quantity input
Steps:
Enter "-2" or "-5" in the quantity field (if editable).
Expected Result:
Negative values should be rejected.

TC-QT-07: Verify alphabet input in quantity field
Steps:
Enter "abc".
Expected Result:
Alphabetic values should not be accepted.

TC-QT-08: Verify special character input in quantity field
Steps:
Enter "@#$".
Expected Result:
Special characters should not be accepted.

TC-QT-09: Verify large quantity selection
Steps:
Click "+" multiple times.
Expected Result:
Quantity should update correctly without errors.

4. Add To Cart
TC-AC-01: Add single product with default quantity
Steps:
Click Add to Cart.
Expected Result:
Product should be added successfully.

TC-AC-02: Add product with custom quantity
Steps:
Increase quantity.
Click Add to Cart.
Expected Result:
Selected quantities should be added.

TC-AC-03: Add multiple different products
Steps:
Add multiple products.
Expected Result:
All products should appear in the cart.

TC-AC-04: Add same product multiple times
Steps:
Add the same product repeatedly.
Expected Result:
Cart should update appropriately.

TC-AC-05: Add product after searching
Steps:
Search for a product.
Add it to the cart.
Expected Result:
Product should be added successfully.

TC-AC-06: Verify cart count updates
Steps:
Add products.
Expected Result:
Cart count should increase accordingly.

5. Cart Preview
TC-CP-01: Verify cart preview with single product
Steps:
Add one product.
Open cart.
Expected Result:
Correct product details should appear.

TC-CP-02: Verify cart preview with multiple products
Steps:
Add multiple products.
Open cart.
Expected Result:
All products should be displayed.

TC-CP-03: Verify product quantity in cart
Steps:
Add product with custom quantity.
Open cart.
Expected Result:
The correct quantity should be displayed.


TC-CP-04: Verify product price in cart
Steps:
Add product.
Open cart.
Expected Result:
The correct price should be displayed.

TC-CP-05: Verify total amount in cart
Steps:
Add products.
Open cart.
Expected Result:
The total amount should be calculated correctly.

TC-CP-06: Verify empty cart preview
Steps:
Open cart without adding products.
Expected Result:
Empty cart message/state should be displayed.

6. Cart Updates
TC-CU-01: Remove product from cart
Steps:
Add product.
Remove it.
Expected Result:
Product should be removed successfully.

TC-CU-02: Remove one product from multiple products
Steps:
Add multiple products.
Remove one.
Expected Result:
Remaining products should stay in the cart.

TC-CU-03: Remove all products
Steps:
Remove all products.
Expected Result:
The cart should become empty.

TC-CU-04: Verify cart count updates after removal
Steps:
Remove product.
Expected Result:
Cart count should decrease.

TC-CU-05: Verify total amount updates after removal
Steps:
Remove product.
Expected Result:
The total amount should be recalculated.

7. Checkout & Promo Code
TC-CO-01: Proceed to checkout with products
Steps:
Add product(s).
Click Proceed to Checkout.
Expected Result:
The checkout page should open successfully.

TC-CO-02: Verify checkout details
Steps:
Open checkout page.
Expected Result:
Product name, quantity and price should match cart details.

TC-CO-03: Attempt checkout with empty cart
Steps:
Keep the cart empty.
Attempt checkout.
Expected Result:
Checkout should not proceed.

TC-PC-01: Apply valid promo code
Steps:
Enter valid promo code.
Click Apply.
Expected Result:
Discount should be applied successfully.

TC-PC-02: Apply invalid promo code
Steps:
Enter invalid promo code.
Click Apply.
Expected Result:
An error message should be displayed.

TC-PC-03: Apply blank promo code
Steps:
Leave the field blank.
Click Apply.
Expected Result:
A validation message should appear.

TC-PC-04: Apply same promo code multiple times
Steps:
Apply promo code.
Apply again.
Expected Result:
The system should handle duplicate applications properly.

8. Price & Discount Calculation
TC-PD-01: Verify single product price calculation
TC-PD-02: Verify multiple product total calculation
TC-PD-03: Verify quantity-based calculation
TC-PD-04: Verify checkout total matches cart total
TC-PD-05: Verify discounted total after promo code
TC-PD-06: Verify discount amount calculation
TC-PD-07: Verify discounted total rounding
TC-PD-08: Verify total never becomes negative
Common Steps:
Add product(s).
Apply quantity/promotional changes if required.
Compare displayed values with calculated values.
Expected Result:
All price and discount calculations should be accurate.

9. Country Selection & Place Order
TC-CS-01: Select valid country
Steps:
Open country dropdown.
Select India.
Expected Result:
The country should be selected successfully.

TC-CS-02: Change selected country
Steps:
Select one country.
Select another country.
Expected Result:
The latest selected country should be displayed.

TC-CS-03: Attempt order without selecting country
Steps:
Skip country selection.
Click Proceed.
Expected Result:
A validation message should appear.

TC-PO-01: Place order successfully
Steps:
Add product.
Select country.
Accept Terms & Conditions.
Click Proceed.
Expected Result:
Order should be placed successfully.

TC-PO-02: Place order without accepting Terms & Conditions
Steps:
Add product.
Select country.
Do not check Terms & Conditions.
Click Proceed.
Expected Result:
Order should not proceed.

TC-PO-03: Attempt order with empty cart
Steps:
Keep cart empty.
Attempt order.
Expected Result:
Order should not be placed.

10. Success & Error Messages
TC-MSG-01: Verify success message after order placement
TC-MSG-02: Verify success message after valid promo code
TC-MSG-03: Verify error message after invalid promo code
TC-MSG-04: Verify validation message for blank promo code
TC-MSG-05: Verify no-result message for invalid search
Expected Result:
Appropriate success/error messages should be displayed for each scenario.

11. Empty Cart Scenarios
TC-EC-01: Open cart when empty
TC-EC-02: Verify checkout is not allowed for empty cart
TC-EC-03: Verify order cannot be placed from empty cart
TC-EC-04: Remove last product and verify empty cart state
TC-EC-05: Verify cart count becomes zero
TC-EC-06: Verify totals become zero after cart is emptied
Expected Result:
Application should correctly handle all empty cart scenarios.


