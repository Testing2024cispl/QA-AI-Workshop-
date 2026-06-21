
Member - Soumi Majumder 

Human thinking manual test cases 

TC_POS_01 Search for an existing product - 

1. Navigate to the GreenKart page. 
2. Type "Brocolli" into the search field. 
3. Press Enter.
4. Only products containing "Brocolli" are displayed.

TC_POS_02 Search using a partial keyword -

1. Navigate to the page. 
2. Type "tom" into the search field. 
3. Press Enter.
4. All products with names containing "tom" (e.g., Tomato) are displayed.

TC_POS_03 Add a single item to the cart - 

1. Navigate to the page. 
2. For "Brocolli - 1 Kg", click the + button to set the quantity to 2. 
3. Click the ADD TO CART button.
4. Cart count increments by 1 (e.g., 1 to 2). 
5. Cart price updates to 240.

TC_POS_04 Add multiple items to the cart - 

1. Navigate to the page. 
2. Add "Brocolli - 1 Kg" (Qty: 1) to the cart. 
3. Add "Cauliflower - 1 Kg" (Qty: 1) to the cart.
4. Cart count shows 2. 
5. Total price shows 180 (120 + 60).

TC_POS_05 Place a successful order - 

1. Add one or more items to the cart. 
2. Click on the Cart icon. 
3. Click the PROCEED TO CHECKOUT button.
4. Click the Place Order button.
5. Select the country from drop down
6. Check the checkbox Agree to the Terms & Conditions
7. Click on Proceed button
8. A confirmation message appears: "Thank you, your order has been placed successfully
You'll be redirected to the Home page shortly!!"

TC_NEG_01 Search for a non-existing product - 

1. Navigate to the page. 
2. Type "Pizza" into the search field. 
3. Press Enter.
4. No products are displayed. The product list becomes empty.

TC_NEG_02 Search with special characters - 

1. Navigate to the page. 
2. Type "@#$%" into the search field. 
3. Press Enter.
4. No products are displayed. The page should not crash or show errors.

TC_NEG_03 Search with empty string - 

1. Navigate to the page. 
2. Leave the search field blank. 
3. Press Enter.
4. All products should be displayed (default view).

TC_NEG_04 Search with a very long string - 

1. Navigate to the page. 
2. Type a 100+ character string into the search field. 
3. Press Enter.
4. No products displayed or page handles gracefully without crashing.

TC_NEG_05 Add item with quantity zero - 

1. Navigate to the page. 
2. For Broccoli, ensure the quantity is 0. by manually enter using keyboard
3. Click the ADD TO CART button.
4. Items should NOT be added to cart. Cart count remains unchanged.

TC_NEG_06 Add item with negative quantity - 

1. Navigate to the page. 
2. Try to manually enter -1 quantity using the keyboard. 
3. Click ADD TO CART.
4. The system should not allow negative quantities.

TC_NEG_07 Place an order with an empty cart - 

1. Ensure the cart is empty (0 items). 
2. Click on the Cart icon. 
3. Click the PROCEED TO CHECKOUT button.
4. The page should handle this gracefully. Button should be disabled OR show error: "Your cart is empty."

TC_NEG_08 Click PROCEED TO CHECKOUT multiple times rapidly - 

1. Add items to the cart. 
2. Click on the Cart icon. 
3. Click the PROCEED TO CHECKOUT button multiple times quickly.
4. Only one order should be placed. No duplicate orders or errors should occur.

Prompt -  

I need you to prepare all positive and negative functional test cases for the following website:
https://rahulshettyacademy.com/seleniumPractise/#/

**Requirements:**
1. Only functional test cases - NO security test cases, NO UI test cases
2. Include BOTH positive and negative test cases
3. Cover all major functionalities of the page

**Functionalities to cover:**
- Search functionality
- Cart management (adding items, removing items)
- Quantity updates (increase, decrease)
- Order placement
- Any other functional behavior on the page

**Format (strictly follow this format):**

TC_POS_01 [Test Case Title] - 

1. [Step 1]
2. [Step 2]
3. [Step 3]
4. [Expected Result]

TC_NEG_01 [Test Case Title] - 

1. [Step 1]
2. [Step 2]
3. [Step 3]
4. [Expected Result]

**Example format I want:**

TC_POS_01 Search for an existing product - 

1. Navigate to the GreenKart page.
2. Type "Brocolli" into the search field.
3. Press Enter.
4. Only products containing "Brocolli" are displayed.

TC_NEG_01 Search for a non-existing product - 

1. Navigate to the page.
2. Type "Pizza" into the search field.
3. Press Enter.
4. No products are displayed. The product list becomes empty.

**Deliverable:**
Provide all test cases in the EXACT same format as shown above with proper numbering (TC_POS_01, TC_POS_02... and TC_NEG_01, TC_NEG_02...). Only provide the test cases, no additional explanation or summary.



AI Manual Test Cases 

TC_POS_01 Search for an existing product -

Navigate to the GreenKart page.
Type "Brocolli" into the search field.
Press Enter.
Only products containing "Brocolli" are displayed.

TC_POS_02 Search using partial product name -

Navigate to the page.
Type "Tom" into the search field.
Press Enter.
Products containing "Tom" in their name are displayed.

TC_POS_03 Clear search and view all products -

Navigate to the page.
Type "Carrot" in the search field.
Clear the search field.
All products are displayed again.
TC_POS_04 Add product to cart -
Navigate to the page.
Click "ADD TO CART" for "Brocolli".
Observe the cart icon.
Product is added to cart and cart count increases.

TC_POS_05 Add multiple different products to cart -
Navigate to the page.
Add "Brocolli" and "Tomato" to the cart.
Click on the cart icon.
Both products are listed in the cart.

TC_POS_06 Increase product quantity before adding to cart -
Navigate to the page.
Click the "+" button for "Brocolli".
Click "ADD TO CART".
Selected quantity is added to the cart.

TC_POS_07 Decrease product quantity before adding to cart -
Navigate to the page.
Increase the quantity and then click the "-" button.
Click "ADD TO CART".
Updated reduced quantity is added to the cart.

TC_POS_08 View cart items -
Add items to cart.
Click on the cart icon.
Click "PROCEED TO CHECKOUT".
The cart page displays added items correctly.

TC_POS_09 Remove item from cart -
Add product to cart.
Go to the cart page.
Click "Remove".
Product is removed from cart.

TC_POS_10 Apply valid promo code -
Add items to cart and proceed to checkout.
Enter valid promo code.
Click "Apply".
Discount is applied successfully.

TC_POS_11 Place order successfully -
Add items to cart.
Proceed to checkout.
Click "Place Order".
Order placement page is displayed.

TC_POS_12 Select country and proceed -
Click "Place Order".
Select a country from the dropdown.
Agree to terms and click "Proceed".
Order is placed successfully.

TC_NEG_01 Search for a non-existing product -
Navigate to the page.
Type "Pizza" into the search field.
Press Enter.
No products are displayed.

TC_NEG_02 Search with special characters -
Navigate to the page.
Type "@#$%" in the search field.
Press Enter.
No products are displayed.

TC_NEG_03 Add to cart without selecting quantity (default 0 scenario check) -
Navigate to the page.
Decrease quantity to minimum if possible.
Click "ADD TO CART".
Product is not added or minimum quantity validation is enforced.

TC_NEG_04 Decrease quantity below 1 -
Navigate to the page.
Click "-" multiple times.
Observe quantity value.
Quantity does not go below 1.

TC_NEG_05 Proceed to checkout with empty cart -
Navigate to the page.
Click the cart icon without adding items.
Click "PROCEED TO CHECKOUT".
Checkout is not allowed or the cart remains empty.

TC_NEG_06 Apply invalid promo code -
Add items to cart.
Proceed to checkout.
Enter invalid promo code.
An error message is displayed and no discount applied.

TC_NEG_07 Place order without selecting country -
Add items to cart.
Click "Place Order".
Click "Proceed" without selecting the country.
Order is not placed and validation message is shown.

TC_NEG_08 Place order without agreeing to terms -
Add items to cart.
Click "Place Order".
Select country but do not check terms checkbox.
Order is not placed and validation message is shown.

TC_NEG_09 Add same product multiple times incorrectly -
Navigate to the page.
Click "ADD TO CART" multiple times for the same product.
Open cart.
Quantity should increment correctly without duplicate entries.

TC_NEG_10 Remove product not present in cart -
Navigate to the page.
Open cart without adding items.
Try to remove items.
No action occurs or proper handling of empty cart.

TC_NEG_11 Apply promo code multiple times -
Add items to cart.
Apply valid promo code once.
Try applying again.
Promo code is not applied again or appropriate message is shown.

TC_NEG_12 Checkout with zero quantity items -
Navigate to the page.
Attempt to add an item with invalid quantity.
Proceed to checkout.
Checkout is prevented or invalid items are not processed.

My thoughts:- 
What I felt Suitable:-  
From AI Generated Test Cases - Proper coverage of core functionalities (search, cart, checkout), Good focus on basic validations like invalid promo code, empty cart, etc and helps in quick test case creation when time is limited. 

What I felt Not suitable:- 
Lacks deep edge cases (e.g., browser refresh after adding to cart, network interruption) and some negative cases are too generic or assumption-based.

Final Test Case:- AI+Manual, Combined test case for Automation ready.

TC_01 Search for an existing product -
Navigate to the GreenKart application homepage
Enter "Brocolli" in the search input field
Press Enter
Verify that only products containing "Brocolli" are displayed
Classification: Positive

TC_02 Search using partial keyword -
Navigate to the homepage
Enter "tom" in the search input field
Press Enter
Verify that products containing "tom" (e.g., Tomato) are displayed
Classification: Positive

TC_03 Clear search and display all products -
Navigate to the homepage
Enter "Carrot" in the search field
Clear the search input field
Verify that all available products are displayed
Classification: Positive

TC_04 Search for non-existing product -
Navigate to the homepage
Enter "Pizza" in the search field
Press Enter
Verify that no products are displayed and no errors occur
Classification: Negative

TC_05 Search with special characters -
Navigate to the homepage
Enter "@#$%" in the search field
Press Enter
Verify that no products are displayed and application remains stable
Classification: Negative

TC_06 Search with empty input -
Navigate to the homepage
Leave the search field empty
Press Enter
Verify that all products are displayed (default state)
Classification: Negative

TC_07 Search with long string input -
Navigate to the homepage
Enter a string with more than 100 characters in the search field
Press Enter
Verify that system handles input gracefully without crash and shows no results
Classification: Negative

TC_08 Add single product to cart with quantity -
Navigate to the homepage
Locate "Brocolli - 1 Kg"
Click "+" to increase quantity to 2
Click "ADD TO CART"
Verify cart count increases and correct total price is updated
Classification: Positive

TC_09 Add multiple different products to cart -
Navigate to the homepage
Add "Brocolli - 1 Kg" (Qty:1) to cart
Add "Cauliflower - 1 Kg" (Qty:1) to cart
Click on cart icon
Verify both products are listed with correct total price
Classification: Positive

TC_10 Increase product quantity before adding to cart -
Navigate to the homepage
Click "+" button for a product
Click "ADD TO CART"
Verify selected quantity is added correctly in cart
Classification: Positive

TC_11 Decrease product quantity before adding to cart -
Navigate to the homepage
Increase quantity and then click "-" button
Click "ADD TO CART"
Verify reduced quantity is added correctly
Classification: Positive

TC_12 Prevent quantity below minimum limit -
Navigate to the homepage
Click "-" button multiple times
Observe quantity field
Verify quantity does not go below 1
Classification: Negative

TC_13 Add product with zero quantity -
Navigate to the homepage
Manually enter quantity as 0
Click "ADD TO CART"
Verify product is not added and validation is enforced
Classification: Negative

TC_14 Add product with negative quantity -
Navigate to the homepage
Enter negative value (e.g., -1) in quantity field
Click "ADD TO CART"
Verify system prevents invalid quantity entry
Classification: Negative

TC_15 Add same product multiple times -
Navigate to the homepage
Click "ADD TO CART" multiple times for same product
Open cart
Verify quantity increments correctly without duplicate entries
Classification: Negative

TC_16 View cart items -
Add products to cart
Click on cart icon
Click "PROCEED TO CHECKOUT"
Verify cart page displays correct items, quantities, and prices
Classification: Positive

TC_17 Remove product from cart -
Add product to cart
Navigate to cart page
Click "Remove" for a product
Verify product is removed and cart updates accordingly
Classification: Positive

TC_18 Remove product from empty cart -
Navigate to cart without adding products
Attempt to remove item
Verify system handles gracefully without error
Classification: Negative

TC_19 Apply valid promo code -
Add items to cart
Proceed to checkout
Enter valid promo code
Click "Apply"
Verify discount is applied to total amount
Classification: Positive

TC_20 Apply invalid promo code -
Add items to cart
Proceed to checkout
Enter invalid promo code
Click "Apply"
Verify error message is displayed and no discount applied
Classification: Negative

TC_21 Apply promo code multiple times -
Add items to cart
Apply valid promo code
Attempt to apply same promo code again
Verify system prevents duplicate application
Classification: Negative

TC_22 Proceed to checkout with items -
Add items to cart
Click cart icon
Click "PROCEED TO CHECKOUT"
Verify navigation to checkout page
Classification: Positive

TC_23 Proceed to checkout with empty cart -
Ensure cart is empty
Click cart icon
Click "PROCEED TO CHECKOUT"
Verify checkout is blocked or appropriate message displayed
Classification: Negative

TC_24 Prevent multiple checkout clicks -
Add items to cart
Navigate to cart
Click "PROCEED TO CHECKOUT" multiple times rapidly
Verify only one checkout process is initiated
Classification: Negative

TC_25 Place order successfully (End-to-End flow) -
Add items to cart
Proceed to checkout
Click "Place Order"
Select country from dropdown
Accept Terms & Conditions
Click "Proceed"
Verify success message is displayed and user is redirected
Classification: Positive

TC_26 Place order without selecting country -
Add items to cart
Proceed to checkout
Click "Place Order"
Click "Proceed" without selecting country
Verify validation message is displayed and order is not placed
Classification: Negative

TC_27 Place order without accepting terms -
Add items to cart
Proceed to checkout
Click "Place Order"
Select country
Do not accept Terms & Conditions
Click "Proceed"
Verify order is not placed and validation is shown
Classification: Negative

TC_28 Checkout with invalid quantity items -
Attempt to add product with invalid quantity
Proceed to checkout
Verify checkout is blocked or invalid items are ignored
Classification: Negative







