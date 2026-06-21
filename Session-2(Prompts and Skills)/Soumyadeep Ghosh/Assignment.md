**QA Manual Test Cases:-**

**Member 1:**- Soumyadeep Ghosh
**Query/Test cases:**- Write test cases for GreenKart

Human Thinking Test Cases


MODULE 1: Home Page & Navigation

TestCases_001:-

1. Verify GreenKart Home Page Load
2. Open browser
3. Navigate to https://rahulshettyacademy.com/seleniumPractise/#/
4. Observe the page title and layout
5. Page loads successfully. 'GreenKart' logo visible, top navigation with search bar, Cart icon, and product listing visible.

TestCases_002:-

1. Verify Page Title
2. Navigate to the GreenKart home page
3. Check the browser tab title
4. Browser tab shows 'GreenKart - veg and fruits kart'

TestCases_003:-

1. Verify Logo Visibility & Navigation
2. Navigate to GreenKart home page
3. Check if GreenKart logo is displayed
4. Click on the logo
5. Logo is visible at the top left. Clicking logo navigates back to the home page / product listing.

TestCases_004:-

1. Verify Navigation Menu Items
2. Navigate to GreenKart home page
3. Observe all nav menu links 
4. Click each navigation link
5. All nav links are visible and clickable. Each link navigates to the respective page.

MODULE 2: Product Listing & Display



TestCases_005:-

1. Verify Product Name is Displayed
2. Navigate to home page
3. Observe each product card
4. Count the number of visible products
5. Each product card displays the product name clearly (e.g., Brocolli, Cauliflower, Cucumber, etc.).


TestCases_006:-

1. Verify Product Price is Displayed
2. Navigate to home page
3. Observe each product card's price
4. Each product displays a numeric price value (e.g., Rs.15, Rs.35, etc.).


TestCases_007:-

1. Verify 'ADD TO CART' Button on Each Product
2. Navigate to home page
3. Check each product card for the ADD TO CART button
4. Every product card has a visible 'ADD TO CART' button.


TestCases_008:-

1. Verify Product Image is Displayed
2. Navigate to home page
3. Observe the top navigation area
4. Each product displays a relevant thumbnail image.

TestCases_009:-

1. Verify Search Bar is Visible
2. Navigate to home page
3. Observe the top navigation area
4. A search input field is visible in the navigation bar.

MODULE 3: Search Functionality


TestCases_010:-

1. Search with Valid Product Name
2. Navigate to home page
3. Click on the search bar
4. Type 'Broc'4. Observe the search results
5. Products matching 'Broc' (e.g., Brocolli) are displayed in filtered results.


TestCases_011:-

1. Search with Full Product Name
2. Navigate to home page
3. Type 'Cauliflower' in the search bar
4. Observe results
5. Only 'Cauliflower' product is shown in the result.


TestCases_012:-

1. Search with Partial Name (Case Insensitive)
2. Navigate to home page
3. Type 'cau' in lowercase in the search bar
4. Observe results
5. Search is case-insensitive; 'Cauliflower' is displayed in results.


TestCases_013:-

1. Search with Non-Existent Product Name
2. Navigate to home page
3. Type 'XYZ123' in the search bar
4. Observe the results
5. No products are displayed. A suitable 'No products found' message or empty list is shown.

TestCases_014:-

1. Clear Search Field and Verify All Products Return
2. Navigate to home page
3. Type 'Tom' in the search bar
4. Clear the search field4. Observe products
5. After clearing the search bar, all products are displayed again.




MODULE 4: Add to Cart


TestCases_015:-

1. Add Single Product to Cart
2. Navigate to home page
3. Click 'ADD TO CART' on 'Cucumber'
4. Observe the Cart icon and product row
5. Item is added to cart. Cart icon count increments by 1. The product row shows quantity controls.


TestCases_016:-

1. Verify Quantity Increment Button
2. Add a product to cart
3. Click the '+' button next to the product
4. Observe the quantity
5. Quantity increases by 1 with each click of the '+' button.


TestCases_017:-

1. Add Multiple Different Products to Cart
2. Navigate to home page
4. Observe cart icon count
5. All 3 products are added. Cart icon shows count 3.


TestCases_018:-

1. Verify Cart Icon Badge Count Updates
2. Navigate to home page
3. Add 3 different items
4. Observe the cart icon badge
5. Cart badge count updates dynamically as items are added.

MODULE 5: Cart Review & Management

TestCases_019:-

1. Navigate to Cart Page
2. Add at least one product
3. Click the Cart icon in the navigation
4. Observe the cart page
5. Cart page opens showing all added products with name, unit price, quantity, and subtotal.


TestCases_020:-

1. Verify Cart Displays Correct Product Names
2. Add 'Cauliflower' and 'Cucumber'
2. Open cart
3. Check product names listed
5. Cart lists 'Cauliflower' and 'Cucumber' correctly.



TestCases_021:-

1. Verify Cart Subtotal Calculation
2. Add 'Cucumber' (Rs.40) x2
3. Open cart
4. Check subtotal
5. Subtotal for Cucumber = Rs.80 (40 x 2). Total amount is correctly calculated.


TestCases_022:-

1. Increase Quantity from Cart Page
2. Open cart with 1 item
3. Click '+' to increase quantity
4. Observe total
5. Quantity increases and total is recalculated correctly.



TestCases_023:-

1. Remove Item from Cart (Decrease to 0)
2. Open cart with 1 item at qty 1
3. Click '-'
4. Observe cart
5. Item is removed from the cart. Cart becomes empty or shows remaining items.


TestCases_024:-

1. Verify 'PROCEED TO CHECKOUT' Button is Present
2. Add items to cart
3. Open cart
4. Look for checkout button
5. 'PROCEED TO CHECKOUT' button is visible and clickable.



TestCases_025:-

1. Verify Empty Cart Message
2. Navigate to cart with no items added
3. Observe cart page
4. Cart page displays an appropriate empty cart message.

MODULE 6: Checkout Process

TestCases_026:-

1. Proceed to Checkout from Cart
2. Add items to cart
3. Click cart icon
4. Click 'PROCEED TO CHECKOUT'
5. Observe next screen
6. User is navigated to the checkout / order summary page.

TestCases_027:-

1. Verify Coupon Code Field Exists on Checkout
2. Proceed to checkout
3. Observe for coupon / promo code input field
4. A coupon code input field is visible on the checkout page.

TestCases_028:-

1. Apply Valid Coupon Code
2. Proceed to checkout
3. Enter a valid coupon code (e.g., 'rahulshettyacademy')
4. Click Apply
5. Observe discount
6. User is navigated to the checkout / order summary page.

TestCases_029:-

1. Apply Invalid Coupon Code
2. Proceed to checkout
3. Enter an invalid code (e.g., 'INVALID123')
4. Click Apply4. Observe
5. An error message is displayed: 'Invalid coupon code' or similar. No discount applied.





TestCases_030:-

1. Apply Empty Coupon Code
2. Proceed to checkout
3. Leave coupon field blank
4. Click Apply
5. An appropriate validation message is shown. No discount applied.

TestCases_031:-

1. Verify Order Total With Valid Coupon
2. Add products
3. Proceed to checkout
4. Apply valid coupon4. Observe discounted total
5. Total is reduced by the discount percentage/amount specified by the coupon.



TestCases_032:-

1. Click 'Place Order' / Proceed to Payment
2. Complete checkout form
3. Click 'Place Order' or equivalent button
4. Observe result
5. Order is placed successfully. Confirmation message or order ID is displayed.

MODULE 7: Offers Page

TestCases_033:-

1. Navigate to Offers Page
2. Navigate to home page
3. Click on 'Offers' in the navigation menu
4. Observe page
5. Offers page loads and displays current deals or discount information.

TestCases_034:-

1. Verify Offers Page Content
2. Navigate to Offers page
3. Observe the content displayed
4. Offers page shows a list of products with special pricing or discount badges.

TestCases_035:-

1. Add Offer Product to Cart
2. Navigate to Offers page
3. Click ADD TO CART on an offer product
4. Verify cart
5. Offer product is added to cart. Cart count updates and offer price is reflected.





MODULE 9: End-to-End Purchase Flow

TestCases_036:-

1. E2E: Search → Add to Cart → Checkout → Place Order
2. Navigate to GreenKart home
3. Search for 'Carrot'
4. Click ADD TO CART
5. Increase quantity to 5
6. Click Cart icon
7. Verify items and total
8. Click PROCEED TO CHECKOUT
9. Apply coupon code
10. Verify discounted total
11. Click Place Order
12. Observe confirmation
13.Full purchase flow completes: product searched and found, added to cart, cart shows correct total, discount applied, order placed and confirmed.

TestCases_037:-

1. E2E: Add Multiple Products → Review Cart → Modify Qty → Checkout
2. Navigate to home page
3. Add Brocolli x1, Cauliflower x2, Cucumber x1
4. Open cart
5. Change Cucumber qty to 3
6. Verify updated total
7. Click PROCEED TO CHECKOUT
8. Confirm order summary
9. Place order
10. All quantities and totals update correctly. Order is placed with updated quantities.


TestCases_038:-

1. E2E: Navigate Away from Cart and Return
2. Add items to cart
3. Click on Offers page
4. Navigate back to Home
5. Click cart icon
6. Cart still shows previously added items after navigating away and back.


MODULE 10: UI, Accessibility & Responsiveness

TestCases_039:-

1. Verify Page Layout on Desktop (1920x1080)
2. Open GreenKart on desktop browser at 1920x10802. Check layout alignment
3. All elements are properly aligned, no overflow, and layout is aesthetically correct.

TestCases_040:-

1. Verify Page Layout on Tablet (768px)
2. Open GreenKart in responsive/tablet mode (768px width)
3. Observe layout
4. Page adapts responsively. Navigation and product grid are usable without horizontal scroll.





TestCases_041:-

1. Verify Page Layout on Mobile (375px)
2. Open GreenKart in mobile view (375px width)
3. Observe layout
4. Page is mobile-friendly. Cart, search, and product listing are functional.

TestCases_042:-

1. Verify Footer Links and Content
2. Scroll to bottom of home page
3. Observe footer
4. Footer is present with appropriate links and copyright text.


TestCases_043:-

1. Verify Broken Images or Missing Content
2. Navigate through all pages
3. Look for broken image icons
4. No broken images. All product thumbnails load correctly.

TestCases_044:-

1. Verify Console Has No Critical JavaScript Errors
2. Open browser DevTools (F12)
3. Navigate all pages
4. Check console tab
5. No critical JS errors shown in the browser console.



**AI Manual Test Cases:-**

**Member 1:**- Soumyadeep Ghosh
**Prompt:**- Write test cases for GreenKart


MODULE 1: Home Page & Navigation

TestCases_001:-

1. Verify GreenKart Home Page Load
2. Open browser
3. Navigate to https://rahulshettyacademy.com/seleniumPractise/#/
4. Observe the page title and layout
5. Page loads successfully. 'GreenKart' logo visible, top navigation with search bar, Cart icon, and product listing visible.

TestCases_002:-

1. Verify Page Title
2. Navigate to the GreenKart home page
3. Check the browser tab title
4. Browser tab shows 'GreenKart - veg and fruits kart'

TestCases_003:-

1. Verify Logo Visibility & Navigation
2. Navigate to GreenKart home page
3. Check if GreenKart logo is displayed
4. Click on the logo
5. Logo is visible at the top left. Clicking logo navigates back to the home page / product listing.

TestCases_004:-

1. Verify Navigation Menu Items
2. Navigate to GreenKart home page
3. Observe all nav menu links (Home, Offers, Sign In)
4. Click each navigation link
5. All nav links are visible and clickable. Each link navigates to the respective page.

MODULE 2: Product Listing & Display

TestCases_005:-

1. Verify Products Are Displayed on Home Page
2. Navigate to home page
3. Observe the product grid/list
4. Count the number of visible products
5. Multiple products (vegetables & fruits) are displayed with Name, Price, and 'ADD TO CART' button.

TestCases_006:-

1. Verify Product Name is Displayed
2. Navigate to home page
3. Observe each product card
4. Count the number of visible products
5. Each product card displays the product name clearly (e.g., Brocolli, Cauliflower, Cucumber, etc.).


TestCases_007:-

1. Verify Product Price is Displayed
2. Navigate to home page
3. Observe each product card's price
4. Each product displays a numeric price value (e.g., Rs.15, Rs.35, etc.).


TestCases_008:-

1. Verify 'ADD TO CART' Button on Each Product
2. Navigate to home page
3. Check each product card for the ADD TO CART button
4. Every product card has a visible 'ADD TO CART' button.


TestCases_009:-

1. Verify Product Image is Displayed
2. Navigate to home page
3. Observe the top navigation area
4. Each product displays a relevant thumbnail image.

TestCases_010:-

1. Verify Search Bar is Visible
2. Navigate to home page
3. Observe the top navigation area
4. A search input field is visible in the navigation bar.

MODULE 3: Search Functionality


TestCases_011:-

1. Search with Valid Product Name
2. Navigate to home page
3. Click on the search bar
4. Type 'Broc'4. Observe the search results
5. Products matching 'Broc' (e.g., Brocolli) are displayed in filtered results.


TestCases_012:-

1. Search with Full Product Name
2. Navigate to home page
3. Type 'Cauliflower' in the search bar
4. Observe results
5. Only 'Cauliflower' product is shown in the result.


TestCases_013:-

1. Search with Partial Name (Case Insensitive)
2. Navigate to home page
3. Type 'cau' in lowercase in the search bar
4. Observe results
5. Search is case-insensitive; 'Cauliflower' is displayed in results.


TestCases_014:-

1. Search with Non-Existent Product Name
2. Navigate to home page
3. Type 'XYZ123' in the search bar
4. Observe the results
5. No products are displayed. A suitable 'No products found' message or empty list is shown.

TestCases_015:-

1. Clear Search Field and Verify All Products Return
2. Navigate to home page
3. Type 'Tom' in the search bar
4. Clear the search field4. Observe products
5. After clearing the search bar, all products are displayed again.


TestCases_016:-

1. Search with Special Characters
2. Navigate to home page
3. Type '@#$%' in the search bar
4. Observe results
5. No products displayed. Application handles special characters gracefully without errors.

MODULE 4: Add to Cart

TestCases_017:-

1. Search with Special Characters
2. Navigate to home page
3. Type '@#$%' in the search bar
4. Observe results
5. No products displayed. Application handles special characters gracefully without errors.


TestCases_018:-

1. Add Single Product to Cart
2. Navigate to home page
3. Click 'ADD TO CART' on 'Brocolli'
4. Observe the Cart icon and product row
5. Item is added to cart. Cart icon count increments by 1. The product row shows quantity controls.


TestCases_019:-

1. Verify Quantity Increment Button
2. Add a product to cart
3. Click the '+' button next to the product
4. Observe the quantity
5. Quantity increases by 1 with each click of the '+' button.


TestCases_020:-

1. Add Multiple Different Products to Cart
2. Navigate to home page
3. Add 'Brocolli', 'Cauliflower', and 'Cucumber' to cart
4. Observe cart icon count
5. All 3 products are added. Cart icon shows count 3.

TestCases_021:-

1. Add Same Product Multiple Times via '+'
2. Add 'Tomato' to cart
3. Click '+' 4 times
4. Observe quantity
5. Quantity of Tomato increases to 5 total.

TestCases_022:-

1. Verify Cart Icon Badge Count Updates
2. Navigate to home page
3. Add 3 different items
4. Observe the cart icon badge
5. Cart badge count updates dynamically as items are added.

MODULE 5: Cart Review & Management

TestCases_023:-

1. Navigate to Cart Page
2. Add at least one product
3. Click the Cart icon in the navigation
4. Observe the cart page
5. Cart page opens showing all added products with name, unit price, quantity, and subtotal.


TestCases_024:-

1. Verify Cart Displays Correct Product Names
2. Add 'Cauliflower' and 'Cucumber'
2. Open cart
3. Check product names listed
5. Cart lists 'Cauliflower' and 'Cucumber' correctly.


TestCases_025:-

1. Verify Cart Displays Correct Quantities
2. Add 'Brocolli' with qty 3
3. Open cart
4. Observe quantity
5. Cart shows quantity 3 for Brocolli.



TestCases_026:-

1. Verify Cart Subtotal Calculation
2. Add 'Cucumber' (Rs.40) x2
3. Open cart
4. Check subtotal
5. Subtotal for Cucumber = Rs.80 (40 x 2). Total amount is correctly calculated.


TestCases_027:-

1. Increase Quantity from Cart Page
2. Open cart with 1 item
3. Click '+' to increase quantity
4. Observe total
5. Quantity increases and total is recalculated correctly.

TestCases_028:-

1. Decrease Quantity from Cart Page
2. Open cart with item qty 2
3. Click '-'
4. Observe qty and total
5. Quantity decreases to 1. Total updates accordingly.

TestCases_029:-

1. Remove Item from Cart (Decrease to 0)
2. Open cart with 1 item at qty 1
3. Click '-'
4. Observe cart
5. Item is removed from the cart. Cart becomes empty or shows remaining items.


TestCases_030:-

1. Verify 'PROCEED TO CHECKOUT' Button is Present
2. Add items to cart
3. Open cart
4. Look for checkout button
5. 'PROCEED TO CHECKOUT' button is visible and clickable.



TestCases_031:-

1. Verify Empty Cart Message
2. Navigate to cart with no items added
3. Observe cart page
4. Cart page displays an appropriate empty cart message.

MODULE 6: Checkout Process

TestCases_032:-

1. Proceed to Checkout from Cart
2. Add items to cart
3. Click cart icon
4. Click 'PROCEED TO CHECKOUT'
5. Observe next screen
6. User is navigated to the checkout / order summary page.

TestCases_033:-

1. Verify Coupon Code Field Exists on Checkout
2. Proceed to checkout
3. Observe for coupon / promo code input field
4. A coupon code input field is visible on the checkout page.

TestCases_034:-

1. Apply Valid Coupon Code
2. Proceed to checkout
3. Enter a valid coupon code (e.g., 'rahulshettyacademy')
4. Click Apply4. Observe discount
5. User is navigated to the checkout / order summary page.

TestCases_035:-

1. Apply Invalid Coupon Code
2. Proceed to checkout
3. Enter an invalid code (e.g., 'INVALID123')
4. Click Apply4. Observe
5. An error message is displayed: 'Invalid coupon code' or similar. No discount applied.





TestCases_036:-

1. Apply Empty Coupon Code
2. Proceed to checkout
3. Leave coupon field blank
4. Click Apply
5. An appropriate validation message is shown. No discount applied.

TestCases_037:-

1. Verify Order Total With Valid Coupon
2. Add products
3. Proceed to checkout
4. Apply valid coupon4. Observe discounted total
5. Total is reduced by the discount percentage/amount specified by the coupon.

TestCases_038:-

1. Verify Order Total Without Coupon
2. Add products totaling a known amount
3. Proceed to checkout
4. Observe order total
5. Total amount shown matches sum of all item subtotals without any discount.


TestCases_039:-

1. Verify Checkout Shows Item Summary
2. Add 2 items
3. Proceed to checkout
4. Observe product list on checkout page
5. Checkout page lists all items with name, quantity, and price.

TestCases_040:-

1. Click 'Place Order' / Proceed to Payment
2. Complete checkout form
3. Click 'Place Order' or equivalent button
4. Observe result
5. Order is placed successfully. Confirmation message or order ID is displayed.

MODULE 7: Offers Page

TestCases_041:-

1. Navigate to Offers Page
2. Navigate to home page
3. Click on 'Offers' in the navigation menu
4. Observe page
5. Offers page loads and displays current deals or discount information.

TestCases_042:-

1. Verify Offers Page Content
2. Navigate to Offers page
3. Observe the content displayed
4. Offers page shows a list of products with special pricing or discount badges.

TestCases_043:-

1. Add Offer Product to Cart
2. Navigate to Offers page
3. Click ADD TO CART on an offer product
4. Verify cart
5. Offer product is added to cart. Cart count updates and offer price is reflected.

MODULE 8: Sign In / Authentication

TestCases_044:-

1. Navigate to Sign In Page
2. Navigate to home page
3. Click 'Sign In' in the navigation
4. Observe page
5. Sign In page opens with username and password input fields.

TestCases_045:-

1. Sign In with Valid Credentials
2. Go to Sign In page
3. Enter valid username
4. Enter valid password4. Click Sign In
5. User is logged in successfully. Navigation shows user name or logout option.


TestCases_046:-

1. Sign In with Invalid Username
2. Go to Sign In page
3. Enter invalid username
4. Enter any password
5. Click Sign In
6. Login fails. Error message displayed: 'Incorrect username or password'.


TestCases_047:-

1. Sign In with Invalid Password
2. Go to Sign In page
3. Enter valid username
4. Enter wrong password
5. Click Sign In
6. Login fails. Error message displayed: 'Incorrect username or password'.


TestCases_048:-

1. Sign In with Empty Fields
2. Go to Sign In page
3. Leave both fields blank
4. Click Sign In
5. Validation error is shown. User is not logged in.

TestCases_049:-

1. Sign In with Empty Username Only
2. Go to Sign In page
3. Leave username blank
4. Enter password4. Click Sign In
5. Validation error shown for username field.

TestCases_050:-

1. Sign In with Empty Password Only
2. Go to Sign In page
3. Enter username
4. Leave password blank
5. Click Sign In
6. Validation error shown for password field.





TestCases_051:-

1. Verify Password Field Masks Input
2. Navigate to Sign In page
3. Click on password field
4. Type any text
5. Observe field display
6. Characters in the password field are masked (shown as dots or asterisks).

MODULE 9: End-to-End Purchase Flow

TestCases_052:-

1. E2E: Search → Add to Cart → Checkout → Place Order
2. Navigate to GreenKart home
3. Search for 'Tomato'
4. Click ADD TO CART
5. Increase quantity to 3
6. Click Cart icon
7. Verify items and total
8. Click PROCEED TO CHECKOUT
9. Apply coupon code 'rahulshettyacademy'
10. Verify discounted total
11. Click Place Order
12. Observe confirmation
13.Full purchase flow completes: product searched and found, added to cart, cart shows correct total, discount applied, order placed and confirmed.

TestCases_053:-

1. E2E: Add Multiple Products → Review Cart → Modify Qty → Checkout
2. Navigate to home page
3. Add Brocolli x1, Cauliflower x2, Cucumber x1
4. Open cart
5. Change Cauliflower qty to 3
6. Verify updated total
7. Click PROCEED TO CHECKOUT
8. Confirm order summary
9. Place order
10. All quantities and totals update correctly. Order is placed with updated quantities.


TestCases_054:-

1. E2E: Cart Persistence After Browser Refresh
2. Add 2 products to cart
3. Refresh the browser (F5)
4. Open cart
5. Verify items
6. Cart retains added items after page refresh (if session storage is used).

TestCases_055:-

1. E2E: Navigate Away from Cart and Return
2. Add items to cart
3. Click on Offers page
4. Navigate back to Home
5. Click cart icon
6. Cart still shows previously added items after navigating away and back.


TestCases_056:-

1. E2E: Sign In → Add Products → Checkout
2. Sign in with valid credentials
3. Search and add 2 products
4. Open cart
5. Proceed to checkout
6. Apply coupon
7. Place order
8. Logged-in user can complete full purchase flow. Order is confirmed.

MODULE 10: UI, Accessibility & Responsiveness

TestCases_057:-

1. Verify Page Layout on Desktop (1920x1080)
2. Open GreenKart on desktop browser at 1920x10802. Check layout alignment
3. All elements are properly aligned, no overflow, and layout is aesthetically correct.

TestCases_058:-

1. Verify Page Layout on Tablet (768px)
2. Open GreenKart in responsive/tablet mode (768px width)
3. Observe layout
4. Page adapts responsively. Navigation and product grid are usable without horizontal scroll.





TestCases_059:-

1. Verify Page Layout on Mobile (375px)
2. Open GreenKart in mobile view (375px width)
3. Observe layout
4. Page is mobile-friendly. Cart, search, and product listing are functional.

TestCases_060:-

1. Verify Footer Links and Content
2. Scroll to bottom of home page
3. Observe footer
4. Footer is present with appropriate links and copyright text.


TestCases_061:-

1. Verify Broken Images or Missing Content
2. Navigate through all pages
3. Look for broken image icons
4. No broken images. All product thumbnails load correctly.

TestCases_062:-

1. Verify Console Has No Critical JavaScript Errors
2. Open browser DevTools (F12)
3. Navigate all pages
4. Check console tab
5. No critical JS errors shown in the browser console.











