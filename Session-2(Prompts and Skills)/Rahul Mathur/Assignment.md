Manual Test Cases - Rahul Mathur  [ Manual Cognitive Validation Test Cases]

Module: Authentication & Login  

**TC_AUTH_001: Verify successful opening and UI layout of the Login Functionality**

Precondition: User is on the homepage and is not logged in.

Test Steps:
Navigate to advantageonlineshopping.com.
Click on the User Icon in the top navigation bar.
The Login modal should be displayed successfully.
The modal should contain:
Sign In with “Facebook” - social functionality
“Username” field
“Password” field
“Remember Me” checkbox
“Sign In” button
“Forgot Your Password?” hyperlink

**TC_AUTH_002 : Title: Verify "Sign In with Facebook" Button Redirects to Facebook Login.**

Steps:
Navigate to advantageonlineshopping.com.
Click the User icon.
Click the Sign In with Facebook button.
Expected Result:
User should be redirected to the Facebook authentication/login page.


**TC_AUTH_003 : Title: Verify "Forgot Your Password?" Link Navigates to Password Recovery Page.**

Steps:
Navigate to advantageonlineshopping.com.
Click the User icon.
Click the Forgot Your Password? link.
Expected Result:
The Password Recovery page should be displayed successfully.

**TC_AUTH_004 : Title: Verify Create New Account Button Navigates to Registration Page**

Steps:
Navigate to advantageonlineshopping.com.
Click the User icon.
Click the Create New Account button.
Expected Result:
User should be redirected to the Registration page.
URL should contain /#/register.
"Create Account" heading should be displayed.
The following sections should be visible:
Account Details
Personal Details
Address

**TC_AUTH_005 :  Title: Verify Successful User Registration with Valid Information**

Precondition: User is on the Registration page at advantageonlineshopping.com/#/register.

Steps:
Fill in account credentials — enter a unique Username, valid Email Address, Password, and re-enter the same password in the Confirm Password field.
Fill in personal details — enter First Name, Last Name, and a valid Phone Number, then select a Country.
Fill in address details — enter City, Address, State/Province, and Postal Code.
Check the "I agree to the Conditions of Use and Privacy Notice" checkbox, then click Register.
Expected Result:
Registration completes successfully and the user account is created.
User is automatically logged in, with their Username displayed in the header.

**TC_AUTH_006: Verify "Remember Me" Checkbox Toggle functionality.**

Precondition: The login pop-up is being open.

Steps:
Click the Remember Me checkbox to select it, then click it again to deselect it.
Expected Result:
On the first click, the checkbox displays a checkmark (selected state).
On the second click, the checkmark disappears (unselected state).

**TC_AUTH_006: Verify Successful User Login with Valid user Credentials.**

Precondition: A registered user account exists, and the Login modal is open.

Steps:
Enter a valid Username and corresponding Password, then click Sign In.
Expected Result:
The login modal closes and the user is authenticated successfully.
The user's Username appears in the header navigation bar, confirming the active session.

**TC_AUTH_007: Verify Successful User Logout.**

Precondition: User is actively logged into the application.

Steps:
Click on the Username in the header navigation bar to open the User Menu, then select Sign Out.
Expected Result:
The user session is terminated and the user is logged out successfully.
The Username in the header is replaced by the generic User Icon, and login options become accessible again.

Module: User Registration  

**TC_REG_003: Verify Successful Registration Using Mandatory Fields Only**

Precondition: User is on the registration page (register).

Steps:
Enter a unique Username and a valid Email Address, then set a valid Password and re-enter it in the Confirm Password field.
Leave all optional fields blank (Personal Details and Address sections), check the I Agree to the Conditions of Use and Privacy Notice checkbox, and click Register.
Expected Result:
Registration completes successfully, confirming that the Personal Details and Address sections are optional.
The user is automatically logged in and their Username is displayed in the header.

**TC_REG_004: Verify Registration with Promotional Subscription Preference Enabled**

Precondition: User is on the registration page (register).

Steps:
Fill in all mandatory fields with valid data and check the Receive Exclusive Offers and Promotions from Advantage checkbox.
Check the I Agree to the Conditions of Use and Privacy Notice checkbox and click Register.
Expected Result:
The account is created successfully.
The promotional subscription preference is saved to the user profile, confirming the opt-in was recorded.

**TC_REG_005: Verify Country Dropdown Population and Selection Behavior functionality.**

Precondition: User is on the registration page (register).

Steps:
Click on the Country dropdown and select any country from the list.
Expected Result:
The dropdown expands and displays a list of valid, selectable countries.
The selected country name is correctly populated and displayed within the Country field.

**TC_REG_006: Verify "Already Have an Account?" Link Redirects to Login functionality.**

Precondition: User is on the registration page (Register).

Steps:
Click the Already Have an Account? link.
Expected Result:
The user is redirected to the homepage and the Login modal is automatically displayed, allowing the user to sign in.

**TC_REG_007: Verify Navigation and Notice Banner Visibility in all aspects .**

Precondition: User is on the registration page (register).

Steps:
Observe the breadcrumb trail and the Notice banner displayed on the page.
Click the Home link within the breadcrumb trail.
Expected Result:
The breadcrumb correctly reads HOME / CREATE ACCOUNT, with Create Account visually highlighted as the active page.
A Notice banner reading "This is a demo site. Do not use real data." is clearly visible on the page.
Clicking Home successfully redirects the user back to the homepage without any errors.

**TC_REG_008: Verify Validation Error When Registering with a Duplicate Username**

Precondition: User is on the registration page. An existing account with the username TestUser123 is already registered.

Steps:
Enter TestUser123 in the Username field, fill in all remaining mandatory fields with valid data, and click Register.
Expected Result:
Registration fails and the form is not submitted.
An inline or banner validation error message is displayed, indicating that the Username is already taken.

**TC_REG_009: Verify Validation Error When Registering with a Duplicate Email Address.**

Precondition: User is on the registration page. An existing account with the email test01@mailinator.com is already registered.

Steps:
Enter a unique Username, enter test01@mailinator.com in the Email field, complete all remaining mandatory fields with valid data, and click Register.
Expected Result:
Registration fails and the form is not submitted.
A validation error message is displayed, indicating that the email address is already associated with an existing account.

**TC_REG_010: Verify Validation Errors Are Displayed When All Mandatory Fields Are Left Blank.**

Precondition: User is on the registration page (/#/register).

Steps:
Leave all mandatory fields blank and click Register.
Expected Result:
Registration fails and the form is not submitted.
Inline validation error messages appear beneath each mandatory field, clearly indicating which fields are required.

**TC_REG_011: Verify Validation Error When Password and Confirm Password Do Not Match.**

Precondition: User is on the registration page (/#/register).

Steps:
Enter Password123 in the Password field and Password321 in the Confirm Password field, complete all remaining mandatory fields with valid data, and click Register.
Expected Result:
Registration fails and the form is not submitted.
A validation error message is displayed, indicating that the passwords do not match.

Module: Search, Navigation & E-Commerce Flow and add to cart  

**TC_NAV_001: Verify Global Product Search Functionality.**

Precondition: User is on the homepage.

Steps:
Click the Search icon in the header, type Tablet into the search bar, and submit the query.
Expected Result:
The search results page loads and displays all products matching the keyword "Tablet", confirming the search function returns relevant results.

**TC_NAV_002: Verify Homepage Category Navigation to Product Details Page.**

Precondition: User is on the homepage.

Steps:
Click the Tablets category block and from the listing page, click on the HP ElitePad 1000 G2 Tablet product card.
Expected Result:
The Tablets category listing page opens, displaying the correct product inventory for that category.
The Product Details page loads, accurately showing the item's image, name, description, and price.

**TC_CART_001: Verify Adding an Item to the Shopping Cart.**

Precondition: User is on the Product Details page for the HP ElitePad 1000 G2 Tablet.

Steps:
Select an available Color swatch, set the Quantity field to 1, and click Add to Cart.
Expected Result:
The product is successfully added to the cart.
The cart icon in the header increments by 1, reflecting the newly added item.

**TC_ORDER_001: Verify Initiating Checkout from the Shopping Cart.**

Precondition: At least one item has been added to the shopping cart.

Steps:
Open the Shopping Cart, verify that the Product Name, Quantity, and Price are correct, then click Checkout.
Expected Result:
The cart displays the correct product details and pricing.
The user is redirected to the Order Payment wizard page to proceed with checkout.

**TC_ORDER_002: Verify Shipping Details Auto-Population and Checkout Step Progression**

Precondition: User is logged in and on the Order Payment page.

Steps:
Observe the active tab step and confirm that the shipping information panel is pre-populated with the user's registered profile data.
Verify the Order Summary totals and calculations are accurate, then click Next.
Expected Result:
The Shipping Details tab is highlighted as the active step upon landing on the page.
Shipping information is automatically populated using the user's registration profile data, requiring no manual entry.
Clicking Next successfully advances the wizard to the Payment Method tab.

**TC_ORDER_003: Verify Successful Checkout Completion Using SafePay Payment Method.**

Precondition: User is on the Payment Method step of the checkout wizard.

Steps:
Select the SafePay payment option, enter valid credentials into the SafePay Username and Password fields, and click Pay Now.
Expected Result:
The transaction is processed successfully without any errors.
The Order Confirmation page is displayed, showing a "Thank You" message along with an auto-generated Tracking Number, Order Number, and a full cost summary breakdown.

**TC_ORDER_004: Verify Newly Placed Order Appears in Order History.**

Precondition: User has successfully completed TC_ORDER_003 and has noted the generated Order Number.

Steps:
Click the User Profile Menu in the header, select My Orders, and locate the Order Number from the recently completed transaction.
Expected Result:
The user is redirected to the My Orders history page listing all past purchases.
The newly placed order is present in the list, with the Order Date, Product Name, Quantity, and Total Price exactly matching the details from the completed purchase.

EDGE CASES 
EC_01  **Title : Browser back after order confirmation!**

Pre-conditions : 
Order placed , on confirmation page.
Steps : 
1. Click browser back button.
2. Observe resulting page and cart state.

EC_02 : 
title : Cart sync across two browser tabs.
steps : 
1. Add item to cart in Tab 1.
2. Switch to Tab 2.
3. Click the cart icon.

EC_03 :
title : Rapid repeated clicks on Add to Cart!
Pre-conditions : Product detail page open.
steps : 
1. Click "Add to Cart" 5 times rapidly.



==================================================================================================================================================================
**AI GENERATED TESTCASES BELOW : LLM USED : CLAUDE,GEMINI**
🔐 LOGIN & REGISTRATION

LR-01 — Successful New User Registration

Steps:

Navigate to advantageonlineshopping.com
Click the person icon → "Create New Account"
Enter First Name: John, Last Name: Doe
Enter Username: johndoe01
Enter Email: john@test.com
Enter Password: Test@1234, Confirm Password: Test@1234
Click "Register"

Expected: Account created. User auto-logged in. Username johndoe01 visible in header.

LR-02 — Registration with Duplicate Username

Steps:

Open registration form
Enter Username: johndoe01 (already exists)
Fill all other fields with valid unique data
Click "Register"

Expected: Error — "Username already exists". User stays on registration page.

LR-03 — Registration with Duplicate Email

Steps:

Open registration form
Enter Email: john@test.com (already registered)
Use a different unique username
Fill remaining fields and click "Register"

Expected: Error — "Email address already in use". Registration blocked.

LR-04 — Password and Confirm Password Mismatch

Steps:

Open registration form
Fill all fields with valid data
Enter Password: Test@1234
Enter Confirm Password: Test@5678
Click "Register"

Expected: Inline error — "Passwords do not match". Form not submitted.

LR-05 — Register with All Fields Empty

Steps:

Open registration form
Leave every field blank
Click "Register"

Expected: Validation error messages appear under all mandatory fields.

LR-06 — Register with Invalid Email Format

Steps:

Open registration form
Enter Email: notanemail (no @ symbol)
Fill all other fields correctly
Click "Register"

Expected: Email field shows — "Please enter a valid email address". Submission blocked.

LR-07 — Password Below Minimum Length

Steps:

Open registration form
Enter Password: Ab1 (only 3 characters)
Fill all other fields correctly
Click "Register"

Expected: Error on password field — "Password must be at least N characters".

LR-08 — Valid Login with Correct Credentials

Steps:

Click the login icon in the header
Enter Username: johndoe01
Enter Password: Test@1234
Click "Sign In"

Expected: Login successful. Username displayed in header. Access to account features granted.

LR-09 — Login with Incorrect Password

Steps:

Open login dialog
Enter Username: johndoe01
Enter Password: WrongPass99
Click "Sign In"

Expected: Error — "Incorrect username or password". User stays on login dialog.

LR-10 — Login with Non-Existent Username

Steps:

Open login dialog
Enter Username: ghostuser999
Enter any password
Click "Sign In"

Expected: Error — "Incorrect username or password".

LR-11 — Login with Blank Fields

Steps:

Open login dialog
Leave username and password fields empty
Click "Sign In"

Expected: Validation — "Username is required", "Password is required".

LR-12 — SQL Injection in Login Username Field ⚠️ Edge Case

Steps:

Open login dialog
Enter Username: ' OR 1=1 --
Enter any password
Click "Sign In"

Expected: Login fails gracefully. No SQL error exposed. No unauthorized access.

LR-13 — Successful Logout

Steps:

Ensure user is logged in
Click the username in the header
Click "Sign Out" from the dropdown
Observe the header

Expected: User logged out. Header shows login icon. Session terminated.

LR-14 — Session Persists After Browser Refresh

Steps:

Log in successfully
Press F5 to refresh the browser

Expected: User remains logged in. Username still visible in header after refresh.

LR-15 — Login with Leading/Trailing Whitespace in Username ⚠️ Edge Case

Steps:

Open login dialog
Enter Username:  johndoe01  (with spaces before and after)
Enter correct password: Test@1234
Click "Sign In"

Expected: Either whitespace is trimmed and login succeeds, OR a clear validation error is shown.

🏠 PRODUCT BROWSING

PB-01 — Homepage Loads with Featured Products

Steps:

Open https://advantageonlineshopping.com/#/
Wait for full page load
Observe the layout

Expected: Homepage loads without errors. Featured products visible. Navigation bar and category links displayed.

PB-02 — Navigate to Tablets Category

Steps:

From homepage, click "Tablets" in the top navigation
Observe the product listing page

Expected: Tablet products listed with images, names, and prices.

PB-03 — Navigate to Laptops Category

Steps:

Click "Laptops" in the top navigation

Expected: Laptop products displayed correctly with images and prices.

PB-04 — Navigate to Mice Category

Steps:

Click "Mice" in the top navigation

Expected: Mouse products listed correctly with images and prices.

PB-05 — Navigate to Speakers Category

Steps:

Click "Speakers" in the top navigation

Expected: Speaker products listed correctly with images and prices.

PB-06 — Product Detail Page Opens Correctly

Steps:

Go to any category listing
Click on any product image or name

Expected: Product detail page opens showing: name, description, price, images, color/option selector, quantity field, and "Add to Cart" button.

PB-07 — Product Image Gallery Thumbnail Click

Steps:

Open any product detail page with multiple images
Note the current main image
Click each thumbnail image below the main image

Expected: Main display image updates to match whichever thumbnail is clicked.

PB-08 — Color Selector Updates Selection State

Steps:

Open a product detail page with multiple color options
Note the default selected color
Click a different color option

Expected: Clicked color becomes visually highlighted/selected. Price or image updates if variants differ.

PB-09 — Quantity Field Accepts Valid Numeric Input

Steps:

Open any product detail page
Click inside the quantity input field
Clear the default value
Type 3

Expected: Field shows 3. No validation error for a valid number.

PB-10 — Product Reviews and Star Rating Displayed

Steps:

Open any product detail page
Scroll down to the reviews section

Expected: Star rating (1–5) and written reviews visible. If no reviews exist — "No reviews yet" message shown.

PB-11 — Breadcrumb Navigation Returns to Category

Steps:

Open a product detail page
Locate the breadcrumb at the top (e.g., Home > Speakers > HP Speaker)
Click the category link in the breadcrumb

Expected: User navigated back to the correct category listing page.

PB-12 — Out-of-Stock Product Disables Add to Cart ⚠️ Edge Case

Steps:

Navigate to a product that is out of stock
Observe the Add to Cart button state

Expected: "Add to Cart" button is disabled or hidden. "Out of Stock" label is visible.

PB-13 — Product Count on Category Page

Steps:

Navigate to any category (e.g., Tablets)
Count the visible products on the listing page
Check if a product count label is displayed

Expected: Visible product count matches any displayed result count label.

🛒 ADD TO CART

ATC-01 — Add Single Product as Guest User

Steps:

Do NOT log in — remain as guest
Navigate to any product detail page (e.g., HP Bluetooth Speaker)
Select a color option if available
Ensure quantity is set to 1
Click "Add to Cart"

Expected: Toast — "Product Added Successfully". Cart badge increments to 1.

ATC-02 — Add Single Product as Logged-In User

Steps:

Log in with valid credentials
Navigate to any product detail page
Select options if applicable
Set quantity to 1
Click "Add to Cart"

Expected: Toast — "Product Added Successfully". Cart badge updates correctly.

ATC-03 — Add Multiple Different Products to Cart

Steps:

Navigate to HP Bluetooth Speaker detail page → click "Add to Cart"
Navigate to HP Wireless Mouse detail page → click "Add to Cart"
Click the cart icon to open the cart

Expected: Both products listed in cart with correct names, selected options, quantity 1 each, and individual prices.

ATC-04 — Add Same Product in Two Different Colors

Steps:

Open HP Tablet detail page
Select color Black → click "Add to Cart"
Go back to the same product detail page
Select color Silver → click "Add to Cart"
Open the cart

Expected: Two separate line items — one Black, one Silver — appear in the cart.

ATC-05 — Add Product with Quantity = 2

Steps:

Open any product detail page
Set quantity field to 2
Click "Add to Cart"
Open the cart

Expected: Product shows with qty 2. Line total = unit price × 2.

ATC-06 — Cart Badge Count Updates Correctly

Steps:

Start with an empty cart
Add Product A with qty 1
Add Product B with qty 2
Observe the cart icon badge number

Expected: Badge shows the correct total count (3 units or 2 items depending on AOS logic).

ATC-07 — Cart Icon Navigates to Cart Page

Steps:

Ensure at least 1 item is in the cart
Click the cart icon in the header

Expected: User navigated to /shoppingCart page showing all cart items.

ATC-08 — Increase Item Quantity Inside Cart

Steps:

Open the cart page
Locate an item with quantity 1
Click the + button or edit the quantity field to 3

Expected: Quantity updates to 3. Subtotal recalculates to unit price × 3. Cart total updates.

ATC-09 — Decrease Item Quantity Inside Cart

Steps:

Open the cart page with an item at quantity 3
Click the − button or reduce quantity to 1

Expected: Quantity updates to 1. Subtotal and cart total recalculate correctly.

ATC-10 — Remove a Single Item from Cart

Steps:

Add 2 different products to the cart
Open the cart page
Click the delete/remove icon on one of the items

Expected: That item is removed. Cart total recalculates. Remaining item still displayed.

ATC-11 — Remove Last Item — Empty Cart State

Steps:

Ensure cart has exactly 1 item
Open the cart page
Click the remove icon on that item

Expected: Cart shows empty state message — "Your cart is empty". Badge shows 0.

ATC-12 — Cart Total Calculates Correctly

Steps:

Add HP Speaker ($89.99) with qty 2
Add HP Pavilion Laptop ($649.00) with qty 1
Open cart and check the total

Expected: Cart total = (89.99 × 2) + 649.00 = $828.98 exactly.

ATC-13 — Cart Items Persist After Navigating Away

Steps:

Add any product to the cart
Navigate to the homepage
Browse to a different category
Click the cart icon

Expected: All previously added items still in cart with unchanged quantities.

ATC-14 — Add to Cart with Quantity = 0 ⚠️ Edge Case

Steps:

Open any product detail page
Clear the quantity field and type 0
Click "Add to Cart"

Expected: Validation error — "Quantity must be at least 1". Product NOT added to cart.

ATC-15 — Add to Cart with Negative Quantity ⚠️ Edge Case

Steps:

Open any product detail page
Enter -1 in the quantity field
Click "Add to Cart"

Expected: Validation error shown. Negative quantity rejected. Cart unchanged.

ATC-16 — Add to Cart with Very Large Quantity (9999) ⚠️ Edge Case

Steps:

Open any product detail page
Enter 9999 in the quantity field
Click "Add to Cart"

Expected: Either accepted (if no stock cap) OR an error about max quantity. No crash or unhandled error.

ATC-17 — Add to Cart with Decimal Quantity (1.5) ⚠️ Edge Case

Steps:

Open any product detail page
Enter 1.5 in the quantity field
Click "Add to Cart"

Expected: Field rejects decimals inline OR rounds to nearest integer. No broken state.

ATC-18 — Add to Cart with Alphabetic Input ⚠️ Edge Case

Steps:

Open any product detail page
Clear the quantity field and type abc
Click "Add to Cart"

Expected: Validation error — "Please enter a valid number". Non-numeric input rejected.

ATC-19 — Add to Cart Without Selecting Required Color ⚠️ Edge Case

Steps:

Open a product that requires a color selection
Do NOT click any color option
Click "Add to Cart"

Expected: Prompt — "Please select a color before adding to cart". Product NOT added.

ATC-20 — Add Same Product Twice in Separate Actions ⚠️ Edge Case

Steps:

Start with an empty cart
Add Product A (qty 1)
Navigate back to the same Product A detail page
Add Product A again (qty 1)
Open the cart

Expected: Either quantity becomes 2 (merged) OR two separate line items appear. Document whichever behavior occurs.

ATC-21 — Set Quantity to 0 Directly in Cart ⚠️ Edge Case

Steps:

Open the cart page
Manually type 0 in the quantity field of an existing item

Expected: Either item is automatically removed OR validation error — "Minimum quantity is 1".

💳 CHECKOUT & PAYMENT

CO-01 — Proceed to Checkout from Cart

Steps:

Add at least 1 item to the cart
Open the cart page
Click the "Checkout" button

Expected: Checkout page opens. Order summary panel shows correct items and prices.

CO-02 — Fill and Submit Valid Billing Details

Steps:

On the checkout billing step, enter:

First Name: John, Last Name: Doe
Email: john@test.com
Address: 123 Main St, City: Kolkata
Country: India
Postal Code: 700001, Phone: 9876543210


Click "Next"

Expected: Billing step validated. User advances to the next step.

CO-03 — Complete Payment with Valid Credit Card

Steps:

Complete billing and shipping steps
Select payment method "Credit Card"
Enter Card Number: 4111111111111111
Enter Cardholder: John Doe, Expiry: 12/27, CVV: 123
Click "Pay Now"

Expected: Order placed. Confirmation page shown with order number.

CO-04 — Complete Payment with SafePay

Steps:

Complete billing step
Select "SafePay" as the payment method
Enter SafePay username and password
Click "Pay"

Expected: Order placed. Confirmation page shown with order number and summary.

CO-05 — Order Summary Matches Cart Items

Steps:

Add 2 products to cart and note their names, prices, and quantities
Proceed to checkout
Compare the checkout order summary panel with the noted cart items

Expected: Product names, quantities, unit prices, and order total all match exactly.

CO-06 — Back Button Retains Filled Billing Data

Steps:

Fill all billing details and advance to the payment step
Click "Back" on the payment step
Observe the billing form fields

Expected: Billing form still shows all previously entered data — nothing cleared.

CO-07 — Cart Cleared After Successful Order

Steps:

Place an order successfully
After the confirmation page, click the cart icon

Expected: Cart is empty. Badge shows 0.

CO-08 — Order Confirmation Page Shows Correct Content

Steps:

Complete a successful order
Observe the order confirmation page

Expected: Page shows: order number, list of ordered items, grand total, and estimated delivery info.

CO-09 — Checkout with Empty Cart ⚠️ Edge Case

Steps:

Ensure the cart is empty
Navigate directly to the checkout URL

Expected: Redirect to cart page OR message — "Your cart is empty". No blank checkout displayed.

CO-10 — Credit Card with Expired Expiry Date ⚠️ Edge Case

Steps:

Reach the payment step
Enter Card Expiry: 01/20 (a past date)
Fill other card fields correctly
Click "Pay Now"

Expected: Payment rejected — "Card has expired".

CO-11 — Credit Card with Invalid CVV ⚠️ Edge Case

Steps:

Reach the payment step
Enter CVV: 12 (only 2 digits) or ABCD (non-numeric)
Click "Pay Now"

Expected: Validation error — "Invalid CVV". Payment blocked.

CO-12 — Credit Card with Wrong Digit Count ⚠️ Edge Case

Steps:

Reach the payment step
Enter Card Number: 41111111 (only 8 digits)
Click "Pay Now"

Expected: Error — "Invalid card number". Payment not processed.

CO-13 — Blank Mandatory Billing Fields ⚠️ Edge Case

Steps:

On the billing step, leave all fields empty
Click "Next"

Expected: Validation errors shown under all required fields. Step does not advance.

CO-14 — Invalid Postal Code Format ⚠️ Edge Case

Steps:

On the billing step, enter Postal Code: ABCDE
Fill all other fields correctly
Click "Next"

Expected: Validation error — "Invalid postal code".

CO-15 — Double-Click Pay Button (Duplicate Order Prevention) ⚠️ Edge Case

Steps:

Fill all checkout details correctly
On the payment step, double-click "Pay Now" rapidly

Expected: Only one order is placed. Duplicate submission prevented.

👤 USER ACCOUNT

UA-01 — View Profile Page

Steps:

Log in with valid credentials
Click the username in the header
Select "My Account" or the profile link

Expected: Account page opens showing username, email, and saved profile details.

UA-02 — Update Profile First Name

Steps:

Log in and navigate to the account/profile page
Click "Edit" on the profile section
Change First Name to Johnny
Save changes

Expected: Success message shown. Updated name reflected on the profile page.

UA-03 — View Order History with Previous Orders

Steps:

Log in with an account that has at least one past order
Navigate to "My Orders" in the account section

Expected: Previous orders shown with order number, date, items list, and total per order.

UA-04 — Order History Empty State

Steps:

Log in with a brand-new account (no orders placed)
Navigate to "My Orders"

Expected: Empty state message — "No orders yet" or similar.

UA-05 — Change Password with Correct Current Password

Steps:

Log in and navigate to the change password section
Enter current password: Test@1234
Enter new password: NewPass@99
Confirm: NewPass@99
Click Save

Expected: Password changed successfully. Success message displayed.

UA-06 — Change Password with Wrong Current Password

Steps:

Navigate to the change password section
Enter wrong current password: WrongOld@1
Enter new password and confirm
Click Save

Expected: Error — "Current password is incorrect". Password not changed.

UA-07 — Access Account Page While Logged Out ⚠️ Edge Case

Steps:

Ensure user is NOT logged in
Manually navigate to the account/profile URL

Expected: Redirect to login page OR access denied error. Account content not visible.

UA-08 — Update Email to an Already-Used Email ⚠️ Edge Case

Steps:

Log in and go to profile edit
Change Email to other@test.com (used by another account)
Save

Expected: Error — "Email address is already in use". Email not updated.

UA-09 — Special Characters in Name Field ⚠️ Edge Case

Steps:

Go to profile edit page
Set First Name to José O'Brien
Save

Expected: Name saved correctly with special characters preserved exactly as entered.

UA-10 — Excessive Length in Name Field (500 chars) ⚠️ Edge Case

Steps:

Go to profile edit page
Paste 500 characters into the First Name field
Click Save

Expected: Field enforces max character limit. Excess characters rejected or trimmed with user feedback.

🔍 SEARCH

SR-01 — Search for Existing Product by Exact Name

Steps:

Click the search icon in the header
Type HP Pavilion
Press Enter or click the search button

Expected: Results page shows products matching "HP Pavilion".

SR-02 — Search with Partial Keyword

Steps:

Click the search icon
Type speak (partial word)
Submit the search

Expected: Speaker products appear in results. Partial match is supported.

SR-03 — Search is Case-Insensitive

Steps:

Search HP SPEAKER — note results
Search hp speaker — note results
Compare both result sets

Expected: Both searches return identical results.

SR-04 — Search Returns No Results for Unknown Term

Steps:

Click the search icon
Type xyznonexistent123
Submit the search

Expected: "No products found" or empty state message displayed.

SR-05 — Search with Empty String ⚠️ Edge Case

Steps:

Click the search icon
Do NOT type anything
Press Enter or click the search button

Expected: All products shown OR message — "Please enter a search term". No crash.

SR-06 — XSS Attempt in Search Field ⚠️ Edge Case

Steps:

Click the search icon
Type: <script>alert("XSS")</script>
Submit the search

Expected: No JavaScript executes. No alert dialog. Input treated as plain text. No crash.

SR-07 — Search with Numeric Input ⚠️ Edge Case

Steps:

Click the search icon
Type 15 (a number)
Submit the search

Expected: Relevant products shown OR empty results. No crash or unhandled error.

SR-08 — Click Product from Search Results

Steps:

Perform a search that returns results (e.g., HP)
Click any product from the results list

Expected: Product detail page opens correctly for the selected product.

SR-09 — Search Result Count Matches Visible Products

Steps:

Search for a broad term like HP
Count visible products on the results page
Check if a result count label is shown

Expected: Visible products count matches the displayed result count label.

SR-10 — Search Works from Product Detail Page

Steps:

Open any product detail page
Use the search bar in the header while on that page
Search for mouse

Expected: Search works from any page. Results load correctly without needing to go to the homepage first.

🧪 CROSS-MODULE EDGE CASES

EC-01 — Browser Back Button After Order Confirmation

Steps:

Complete a full order and land on the confirmation page
Click the browser back button
Observe the resulting page and cart state

Expected: Redirected to cart or homepage. Order is NOT duplicated. Cart remains empty.

EC-02 — Cart Sync Across Two Browser Tabs

Steps:

Log in on Tab 1 and add a product to cart
Open Tab 2 (same browser, same session)
Click the cart icon on Tab 2

Expected: Cart on Tab 2 reflects the item added in Tab 1 (at latest after refresh/navigation).

EC-03 — Session Expires Mid-Checkout

Steps:

Log in and navigate to the payment step of checkout
Leave the page idle until the session expires
Try to click "Pay Now"

Expected: Prompt to log in again. Cart items retained if possible. Order NOT partially placed.

EC-04 — Direct URL Access to Checkout with Empty Cart

Steps:

Ensure the cart is empty
Manually type the checkout URL in the browser address bar

Expected: Redirect to cart page OR message — "Your cart is empty". No blank checkout page.

EC-05 — Mobile Viewport Responsiveness (375px) ⚠️ Edge Case

Steps:

Open DevTools (F12)
Set viewport to 375 × 812 (mobile)
Browse homepage → category page → product detail → cart → checkout

Expected: All pages adapt to mobile viewport. Navigation usable. No clipped text or broken buttons at any step.

EC-06 — XSS Attempt in Product Review Text ⚠️ Edge Case

Steps:

Log in and navigate to any product detail page
Submit a review with text: <img src=x onerror=alert(1)>
Save and reload the page to view the review

Expected: Review text rendered as plain text. No JavaScript executes. HTML is escaped in output.

EC-07 — Very Long Text in Checkout Address Field ⚠️ Edge Case

Steps:

On the checkout billing step, paste 500 characters into the Street Address field
Click "Next"

Expected: Field enforces a max character limit. Excess characters rejected or trimmed with user feedback.

EC-08 — Network Interruption During Add to Cart ⚠️ Edge Case

Steps:

Open any product detail page
Open DevTools → Network tab → set to Offline mode
Click "Add to Cart"

Expected: Appropriate network error message shown. App does not crash. Cart state not corrupted.

EC-09 — Rapid Repeated Clicks on Add to Cart ⚠️ Edge Case

Steps:

Open any product detail page
Click "Add to Cart" 5 times rapidly in quick succession
Open the cart

Expected: Product added only ONCE (or qty incremented correctly). No duplicate line items from rapid clicking.

EC-10 — Page Reload Mid Cart Edit ⚠️ Edge Case

Steps:

Open the cart page
Change the quantity of an item
Before confirming, press F5 to reload the page

Expected: Cart reverts to the last saved/confirmed state. No corrupted data or negative quantities.
