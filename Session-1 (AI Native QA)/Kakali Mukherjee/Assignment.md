# Session 1
## Member 1:-Kakali Mukhopadhyay
## Query/Test cases:- https://demowebshop.tricentis.com/ 

Human Thinking Test Cases

# Test Scenarios 
# Manual Test Cases 
# TC 01
Open in any browser the given link https://demowebshop.tricentis.com/ 
Result :Website should open successfully
# TC 02
Click on ‘Register’ Link from the Top of the Page
After Registration Page opening Fill-up the personal details like Gender, First Name, Last name, email and password
(In case of password creation we have to maintain some options like Enter a valid alpha-numeric, case sensitive and length. Password will be verified after that we need to to Confirm Password with the same data
Click on Register Button
Result : Registration should be done successfully
# TC 03
Open in any Browser the mentioned link and click on the Login button from Top.
Enter the generated credentials and after click on Login button
Result : User should Logged in into the system
# TC 04
If someone Forgot Password then Click on Forgot Password Link, and reset the New Password in two text boxes like Password and Confirm Password. Click on Recover button 
Result : User should recover the account. 
# TC 05
Click on Category from the Links “Books / Computers / Electronics / Apparel & Shoes / Digital downloads / Jewelry / Gift Cards”tab from the left panel. 
User should check any sub-category remains or not 
Result : Desired page should be opened 
# TC 06
After clicking on the Product Detail Page, 
Click on the book name in a variable “book” as ${bookName}.
Click on the ${bookName}.
Verify that  Select from ‘Filter by price’ “Under 25.00”
User Choose any Category / Sub-Category / Filter Options / Sorting Options
Result : Selected Product should show  
# TC 07
Add any Product like ‘Book’ into Cart 
Select “Computing and Internet”
Choose the ‘Quantity’ 
In the Quantity field negative value is taken, no validation.. 
Press ‘Add to cart’
Press ‘Email a friend’
Add ‘Friend’s email’
Add ‘self email address’
Add personal message
Opt for ‘Send email’
Select  ‘Add to cart’
Select Shopping Cart click on ‘Go to Cart’
Click on ‘Apply Coupon’, if any Coupon remains
Click on ‘Add gift card’, if any Gift Card remains
Result : Desired  Product i.e. Book should be added in to cart 

AI Test Cases 
Kakali Mukhopadhyay : # AI-Generated Test Cases

## Module: Registration
### TC-REG-001 Successful user registration with valid data
#### Module Registration Type: Positive Priority: P1
#### Preconditions User is not registered. Browser open at homepage.
#### Test Steps
1. Navigate to demowebshop.tricentis.com
2. Click 'Register' link in header
3. Select gender (Male/Female)
4. Enter first name: John
5. Enter last name: Smith
6. Enter email: john.smith.test@qa.com
7. Enter password: Test@1234
8. Enter confirm password: Test@1234
9. Click 'Register' button


### TC-REG-002 Registration with already existing email
#### Module Registration Type: Negative Priority: P1
#### Preconditions User 'john.smith.test@qa.com' already registered.
#### Test Steps
1. Navigate to Register page
2. Fill all fields with same email as existing account
3. Click 'Register' button


### TC-REG-003 Registration with blank mandatory fields
#### Module Registration Type: Negative Priority: P1
#### Preconditions User is on the registration page.
#### Test Steps
1. Navigate to Register page
2. Leave all fields blank
3. Click 'Register' button


### TC-REG-004 Registration with invalid email format
#### Module Registration Type: Negative Priority: P2
#### Preconditions User is on the registration page.
#### Test Steps
1. Navigate to Register page
2. Enter first name, last name
3. Enter invalid email: 'notanemail'
4. Enter valid password and confirm
5. Click 'Register'


### TC-REG-005 Registration with mismatched passwords
#### Module Registration Type: Negative Priority: P1
#### Preconditions User is on the registration page.
#### Test Steps
1. Navigate to Register page
2. Fill all fields with valid data
3. Enter password: Test@1234
4. Enter confirm password: Different123
5. Click 'Register'


### TC-REG-006 Registration with password at minimum boundary (6 chars)
#### Module Registration Type: BVA Priority: P2
#### Preconditions User is on the registration page.
#### Test Steps
1. Navigate to Register page
2. Fill name and email fields
3. Enter password: 'Ab1234' (exactly 6 chars)
4. Enter confirm password: 'Ab1234'
5. Click 'Register'


### TC-REG-007 Registration with password below minimum (5 chars)
#### Module Registration Type: BVA Priority: P2
#### Preconditions User is on the registration page.
#### Test Steps
1. Navigate to Register page
2. Fill name and email fields
3. Enter password: 'Ab123' (5 chars)
4. Enter confirm password: 'Ab123'
5. Click 'Register'

### TC-REG-008 Registration with special characters in name fields
#### Module Registration Type: Exploratory Priority: P3
#### Preconditions User is on the registration page.
#### Test Steps
1. Navigate to Register page
2. Enter first name: "O'Brien"
3. Enter last name: 'St. Claire-Jones'
4. Enter valid email and password
5. Click 'Register'

## Module: Login
### TC-LOG-001 Successful login with valid credentials
#### Module Login Type: Positive Priority: P1
#### Preconditions Registered user account exists.
#### Test Steps
1. Navigate to demowebshop.tricentis.com
2. Click 'Log in' in header
3. Enter valid email address
4. Enter valid password
5. Click 'Log in' button


### TC-LOG-002 Login with invalid password
#### Module Login Type: Negative Priority: P1
#### Preconditions Registered user account exists.
#### Test Steps
1. Navigate to Login page
2. Enter valid email
3. Enter wrong password: 'WrongPass999'
4. Click 'Log in'


### TC-LOG-003 Login with unregistered email
#### Module Login Type: Negative Priority: P1
#### Preconditions No account exists for notexist@test.com.
#### Test Steps
1. Navigate to Login page
2. Enter email: notexist@test.com
3. Enter any password
4. Click 'Log in'


### TC-LOG-004 Login with blank email and password
#### Module Login Type: Negative Priority: P2
#### Preconditions User is on login page.
#### Test Steps
1. Navigate to Login page
2. Leave email field empty
3. Leave password field empty
4. Click 'Log in'
[6/29/2026 5:19 PM] Soumitra Dhar: ### TC-LOG-005 'Remember me' checkbox retains session
#### Module Login Type: Exploratory Priority: P3
#### Preconditions Registered user account exists.
#### Test Steps
1. Navigate to Login page
2. Enter valid credentials
3. Check 'Remember me' checkbox
4. Click 'Log in'
5. Close and reopen browser
6. Navigate to site


### TC-LOG-006 Forgot password — email sent for registered email
#### Module Login Type: Positive Priority: P2
#### Preconditions Registered user account exists.
#### Test Steps
1. Navigate to Login page
2. Click 'Forgot password?' link
3. Enter registered email address
4. Click 'Recover'


### TC-LOG-007 Forgot password — unregistered email
#### Module Login Type: Negative Priority: P2
#### Preconditions Email notexist@test.com is not registered.
#### Test Steps
1. Navigate to Forgot Password page
2. Enter unregistered email
3. Click 'Recover'


### TC-LOG-008 Logout clears session
#### Module Login Type: Positive Priority: P1
#### Preconditions User is logged in.
#### Test Steps
1. Verify user is logged in (name in header)
2. Click 'Log out' link
3. Observe page redirect
4. Try to access account page directly via URL



## Module: Search
### TC-SRC-001 Search with valid existing product keyword
#### Module Search Type: Positive Priority: P1
#### Preconditions User on homepage (logged in or guest).
#### Test Steps
1. Locate search bar in header
2. Type 'computer' in search field
3. Click search button or press Enter


### TC-SRC-002 Search with keyword returning no results
#### Module Search Type: Negative Priority: P2
#### Preconditions User on homepage.
#### Test Steps
1. Type 'xyznotexistproduct12345' in search bar
2. Press Enter or click Search


### TC-SRC-003 Search with empty string
#### Module Search Type: Negative Priority: P2
#### Preconditions User on homepage.
#### Test Steps
1. Click on search field without typing anything
2. Click search button


### TC-SRC-004 Search with XSS injection payload
#### Module Search Type: Negative Priority: P3
#### Preconditions User on homepage.
#### Test Steps
1. Type '<script>alert(1)</script>' in search bar
2. Click Search


### TC-SRC-005 Search results — sort by price ascending
#### Module Search Type: Positive Priority: P2
#### Preconditions Search results showing multiple products.
#### Test Steps
1. Perform a search for 'book'
2. Locate 'Sort by' dropdown
3. Select 'Price: Low to High'


### TC-SRC-006 Search results — change display per page to 12
#### Module Search Type: Positive Priority: P3
#### Preconditions Search results page with more than 4 results.
#### Test Steps
1. Perform search returning many products
2. Locate 'Display per page' dropdown
3. Select '12'


### TC-SRC-007 Category navigation — Books
#### Module Search Type: Positive Priority: P2
#### Preconditions User on homepage.
#### Test Steps
1. Click 'Books' in left navigation categories
2. Verify category page loads
3. Observe products displayed



## Module: Product
### TC-PRD-001 Product detail page loads with all required elements
#### Module Product Type: Positive Priority: P1
#### Preconditions User on homepage or search results.
#### Test Steps
1. Search for 'simple computer'
2. Click on the product name/image
3. Observe product detail page


### TC-PRD-002 Add to cart from product detail page
#### Module Product Type: Positive Priority: P1
#### Preconditions User on product detail page (logged in or guest).
#### Test Steps
1. Navigate to any product detail page
2. Set quantity to 1
3. Click 'Add to cart' button
4. Observe notification


### TC-PRD-003 Add to cart with quantity set to 0
#### Module Product Type: BVA Priority: P2
#### Preconditions User on product detail page.
#### Test Steps
1. Navigate to product detail page
2. Clear quantity field and enter '0'
3. Click 'Add to cart'
[6/29/2026 5:19 PM] Soumitra Dhar: ### TC-PRD-004 Add to cart with negative quantity
#### Module Product Type: Negative Priority: P2
#### Preconditions User on product detail page.
#### Test Steps
1. Navigate to product detail page
2. Enter '-1' in quantity field
3. Click 'Add to cart'


### TC-PRD-005 Add to cart with very large quantity (999999)
#### Module Product Type: BVA Priority: P3
#### Preconditions User on product detail page.
#### Test Steps
1. Navigate to product detail page
2. Enter '999999' in quantity field
3. Click 'Add to cart'


### TC-PRD-006 Add product to wishlist (logged in)
#### Module Product Type: Positive Priority: P2
#### Preconditions User is logged in. On product detail page.
#### Test Steps
1. Navigate to product detail page
2. Click 'Add to wishlist' button
3. Observe notification


### TC-PRD-007 Add to wishlist as guest (not logged in)
#### Module Product Type: Negative Priority: P2
#### Preconditions User is NOT logged in.
#### Test Steps
1. Navigate to product detail page as guest
2. Click 'Add to wishlist'


### TC-PRD-008 Product page breadcrumb navigation
#### Module Product Type: Positive Priority: P3
#### Preconditions User navigated to a product via category.
#### Test Steps
1. Click a category (e.g., Computers > Desktops)
2. Click on a product
3. Verify breadcrumb trail
4. Click each breadcrumb link



## Module: Cart
### TC-CART-001 View shopping cart with items
#### Module Cart Type: Positive Priority: P1
#### Preconditions At least one product added to cart.
#### Test Steps
1. Add a product to cart
2. Click shopping cart link in header
3. Observe cart page


### TC-CART-002 Update product quantity in cart
#### Module Cart Type: Positive Priority: P2
#### Preconditions Cart has at least one product.
#### Test Steps
1. Navigate to shopping cart
2. Change quantity of a product from 1 to 3
3. Click 'Update shopping cart'


### TC-CART-003 Remove product from cart
#### Module Cart Type: Positive Priority: P1
#### Preconditions Cart has at least one product.
#### Test Steps
1. Navigate to shopping cart
2. Click the remove checkbox/button next to a product
3. Click 'Update shopping cart'


### TC-CART-004 Apply invalid coupon code
#### Module Cart Type: Negative Priority: P2
#### Preconditions Cart has at least one product.
#### Test Steps
1. Navigate to shopping cart
2. Locate coupon code field
3. Enter 'INVALIDCOUPON123'
4. Click 'Apply coupon'


### TC-CART-005 Proceed to checkout without accepting terms
#### Module Cart Type: Negative Priority: P1
#### Preconditions Cart has at least one product. User on cart page.
#### Test Steps
1. Navigate to shopping cart
2. Do NOT check 'I agree with the terms of service' checkbox
3. Click 'Checkout'


### TC-CART-006 Empty cart — checkout button behavior
#### Module Cart Type: Exploratory Priority: P2
#### Preconditions Cart is empty.
#### Test Steps
1. Navigate to shopping cart page when no items added
2. Observe page state
3. Try clicking Checkout if visible


### TC-CART-007 Cart persists across page navigation
Module Cart Type: Exploratory Priority: P2
Preconditions User adds items to cart.
Test Steps
1. Add product to cart
2. Navigate to other pages (Home, Category, Product)
3. Return to cart



## Module: Checkout
### TC-CHK-001 Guest checkout — full end-to-end flow
#### Module Checkout Type: Positive Priority: P1
#### Preconditions Cart has at least one item. User is NOT logged in.
#### Test Steps
1. Navigate to cart page
2. Accept terms of service checkbox
3. Click Checkout
4. Select 'Checkout as Guest'
5. Enter billing: First Name, Last Name, Email, Country, City, Address 1, Zip, Phone
6. Click Continue
7. Select or confirm shipping address
8. Click Continue
9. Select shipping method (e.g., Ground)
10. Click Continue
11. Select payment method (e.g., Cash On Delivery)
12. Click Continue
13. Review order summary
14. Click 'Confirm'
[6/29/2026 5:19 PM] Soumitra Dhar: ### TC-CHK-002 Registered user checkout — credit card payment
#### Module Checkout Type: Positive Priority: P1
#### Preconditions User logged in. Cart has items.
#### Test Steps
1. Navigate to cart
2. Accept terms of service
3. Click Checkout
4. Fill or use saved billing address
5. Select shipping method
6. Select payment: Credit Card
7. Enter Visa: 4485564059489345, Exp: 04/2027, CVV: 123
8. Click Continue
9. Confirm order


### TC-CHK-003 Checkout — billing address with missing required field
#### Module Checkout Type: Negative Priority: P1
#### Preconditions In checkout billing address step.
#### Test Steps
1. Reach billing address step
2. Leave 'City' field empty
3. Fill all other required fields
4. Click Continue


### TC-CHK-004 Checkout — invalid zip code format
#### Module Checkout Type: Negative Priority: P2
#### Preconditions In checkout billing address step.
#### Test Steps
1. Enter billing address
2. Enter zip code: 'ABCDE' (non-numeric)
3. Click Continue


### TC-CHK-005 Shipping method — Next Day Air selection
#### Module Checkout Type: Positive Priority: P2
#### Preconditions In shipping method step of checkout.
#### Test Steps
1. Reach shipping method step
2. Select 'Next Day Air' shipping option
3. Click Continue


### TC-CHK-006 Payment method — Purchase Order
#### Module Checkout Type: Positive Priority: P2
#### Preconditions In payment step. Purchase Order method available.
#### Test Steps
1. Reach payment method step
2. Select 'Purchase Order'
3. Enter PO number: 'PO-2024-001'
4. Click Continue
5. Confirm order


### TC-CHK-007 Checkout — browser back button integrity
#### Module Checkout Type: Exploratory Priority: P3
#### Preconditions User is in middle of checkout (at payment step).
#### Test Steps
1. Proceed through checkout to payment step
2. Use browser back button
3. Observe page and cart state


### TC-CHK-008 Order confirmation — unique order number generated
#### Module Checkout Type: Positive Priority: P1
#### Preconditions Order placed successfully.
#### Test Steps
1. Complete the full checkout process
2. Observe the confirmation page



## Module: Account
### TC-ACC-001 My account — order history displays past orders
#### Module Account Type: Positive Priority: P2
#### Preconditions User logged in. At least one order placed.
#### Test Steps
1. Log in with account that has orders
2. Click on username/My Account in header
3. Navigate to 'Orders' section


### TC-ACC-002 Change account password — valid new password
#### Module Account Type: Positive Priority: P2
#### Preconditions User is logged in.
#### Test Steps
1. Navigate to My Account > Change Password
2. Enter current password
3. Enter new password: NewPass@5678
4. Enter confirm new password: NewPass@5678
5. Click 'Change Password'


### TC-ACC-003 Change password — incorrect current password
#### Module Account Type: Negative Priority: P2
#### Preconditions User is logged in.
#### Test Steps
1. Navigate to Change Password
2. Enter an incorrect current password
3. Enter new password and confirmation
4. Click 'Change Password'


### TC-ACC-004 Edit account info — update name
#### Module Account Type: Positive Priority: P2
#### Preconditions User is logged in.
#### Test Steps
1. Navigate to My Account > Account Info
2. Update First Name to 'UpdatedName'
3. Click 'Save'


### TC-ACC-005 Downloadable products — access after purchase
#### Module Account Type: Exploratory Priority: P3
#### Preconditions User purchased a digital download product.
#### Test Steps
1. Navigate to My Account
2. Click 'Downloadable products'
3. Attempt to download purchased product



## Module: Wishlist
### TC-WSH-001 Add product to wishlist and view wishlist page
#### Module Wishlist Type: Positive Priority: P2
#### Preconditions User is logged in.
#### Test Steps
1. Navigate to any product detail page
2. Click 'Add to wishlist'
3. Click 'Wishlist' link in header
4. Observe wishlist page
[6/29/2026 5:19 PM] Soumitra Dhar: ### TC-WSH-002 Move product from wishlist to cart
#### Module Wishlist Type: Positive Priority: P2
#### Preconditions User logged in. Wishlist has at least one item.
#### Test Steps
1. Navigate to Wishlist
2. Select the product (checkbox or Add to cart button)
3. Click 'Add to cart'


### TC-WSH-003 Remove product from wishlist
#### Module Wishlist Type: Positive Priority: P2
#### Preconditions User logged in. Wishlist has at least one item.
#### Test Steps
1. Navigate to Wishlist
2. Click remove button next to a product
3. Confirm if prompted


### TC-WSH-004 Share wishlist via public URL
#### Module Wishlist Type: Exploratory Priority: P3
#### Preconditions User logged in with items in wishlist.
#### Test Steps
1. Navigate to Wishlist page
2. Locate 'Wishlist URL for sharing' field
3. Copy the URL
4. Open the URL in a new incognito browser session



## Module: Navigation
### TC-NAV-001 Homepage loads with all 7 product categories
#### Module Navigation Type: Positive Priority: P1
#### Preconditions Browser open, no prior session needed.
#### Test Steps
1. Navigate to demowebshop.tricentis.com
2. Observe left sidebar categories


### TC-NAV-002 Computers subcategories — Desktops and Notebooks
#### Module Navigation Type: Positive Priority: P2
#### Preconditions User on homepage.
#### Test Steps
1. Click 'Computers' in category nav
2. Observe subcategories or hover to expand
3. Click 'Desktops'
4. Verify products shown
5. Navigate back, click 'Notebooks'
6. Verify products shown

Final Test Case:-
AI+Manual 




