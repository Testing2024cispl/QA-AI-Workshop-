# Session-1
# QA Manual Test Cases
**Member Name: Soumitra Dhar**

**URL:https://demowebshop.tricentis.com/**

## Human Thinking Test Cases

### TC-001 (Verify user can register successfully)
#### Preconditions: User is on the homepage
#### Test Steps	
Click Register → Enter valid details → Submit

### TC-002 (Verify mandatory fields validation in registration)
#### Preconditions: User is on the registration page
#### Test Steps	
Click Register without data

### TC-003 (Verify valid login functionality)
#### Preconditions: User must be registered
#### Test Steps	 
Enter valid credentials → Login

### TC-004 (Verify invalid login error message)
#### Preconditions: User is on the login page
#### Test Steps	
Enter invalid credentials → Login

### TC-005 (Verify search with valid product name)
#### Preconditions: User is on the homepage
#### Test Steps	
Enter product name → Search

### TC-006 (Verify search with invalid product name)
#### Preconditions: User is on the homepage
#### Test Steps	
Enter random text → Search

### TC-007 (Verify add product to cart)
#### Preconditions: User is logged in
#### Test Steps	
Open product → Click Add to Cart

### TC-008 (Verify cart quantity update)
#### Preconditions: Product in cart
#### Test Steps	
Update quantity in cart

### TC-009 (Verify checkout process)
#### Preconditions: Items in cart
#### Test Steps	 
Go to checkout → Enter details → Confirm

### TC-010 (Verify checkout without login)
#### Preconditions: User not logged in
#### Test Steps	
Try to check out

### TC-011 (Verify homepage layout alignment)
#### Preconditions: Open homepage
#### Test Steps	
Check UI alignment

### TC-012 (Verify responsiveness)
#### Preconditions: Open the site in mobile view
#### Test Steps	
Resize the browser

### TC-013 (Verify logout functionality)
#### Preconditions: User is logged in
#### Test Steps	
Click Logout

### TC-014 (Verify registration with empty fields)
#### Preconditions: User is on the registration page
#### Test Steps	
Click Register without data

### TC-015 (Verify invalid email format)
#### Preconditions: User is on the registration page
#### Test Steps	
Enter an invalid email

### TC-016 (Verify registration with existing email)\
#### Preconditions: Email already exists
#### Test Steps	
Register with existing email

### TC-017 (Verify password mismatch)
#### Preconditions: User is on the registration page
#### Test Steps	
Enter a different password and confirm password

### TC-018 (Verify login with invalid credentials)
#### Preconditions: User is on the login page
#### Test Steps	 
Enter wrong credentials

### TC-019 (Verify login with empty fields)
#### Preconditions: User is on the login page
#### Test Steps	 
Click login without data

### TC-020 (Verify login with unregistered email)
#### Preconditions: User is on the login page
#### Test Steps	
Enter a random email

### TC-021 (Verify search with special characters)
#### Preconditions: User is on homepage
#### Test Steps	
Enter @@###

### TC-022 (Verify search with long input)
#### Preconditions: User is on homepage
#### Test Steps	
Enter very long string

### TC-023 (Verify adding out-of-stock product)
#### Preconditions: Product unavailable
#### Test Steps	
Try to add a product

### TC-024 (Verify invalid cart quantity)
#### Preconditions: Product in cart
#### Test Steps	
Enter -1 or alphabets

### TC-025 (Verify checkout with empty cart)
#### Preconditions: Cart is empty
#### Test Steps	
Go to checkout

### TC-026 (Verify incomplete address)
#### Preconditions: In checkout
#### Test Steps	
Leave mandatory fields empty

### TC-027 (Verify payment failure)
#### Preconditions: Items in cart
#### Test Steps	
Enter invalid payment details

### TC-028 (Verify UI on very small screen)
#### Preconditions: Open the site in mobile view
#### Test Steps	
Resize to 320px

# AI Manual Test Cases:-
**Member Name: Soumitra Dhar**
## System Under Test: Tricentis Demo Web Shop
## URL: https://demowebshop.tricentis.com/
## Prepared By:  QA Engineer	Testing Types: Functional, BVA, Negative, Exploratory
## Document Version: 1.0	Total Test Cases: 57
## Modules Covered: Registration, Login, Search, Product, Cart, Checkout, Account, Wishlist, Navigation

## Test Summary

1.Module	
2.Registration	
3.Login	
4.Search	
5.Product	
6.Cart	
7.Checkout	
8.Account
9.Wishlist	
10.Navigation	


# AI-Generated Test Cases 

## Module: Registration
### TC-REG-001  Successful user registration with valid data
#### Module	Registration     Type: Positive     Priority: P1
#### Preconditions	User is not registered. Browser open at homepage.
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


### TC-REG-002  Registration with already existing email
#### Module	Registration     Type: Negative     Priority: P1
#### Preconditions	User 'john.smith.test@qa.com' already registered.
#### Test Steps
1. Navigate to Register page
2. Fill all fields with same email as existing account
3. Click 'Register' button


### TC-REG-003  Registration with blank mandatory fields
#### Module	Registration     Type: Negative     Priority: P1
#### Preconditions	User is on the registration page.
#### Test Steps
1. Navigate to Register page
2. Leave all fields blank
3. Click 'Register' button


### TC-REG-004  Registration with invalid email format
#### Module	Registration     Type: Negative     Priority: P2
#### Preconditions	User is on the registration page.
#### Test Steps	
1. Navigate to Register page
2. Enter first name, last name
3. Enter invalid email: 'notanemail'
4. Enter valid password and confirm
5. Click 'Register'


### TC-REG-005  Registration with mismatched passwords
#### Module	Registration     Type: Negative     Priority: P1
#### Preconditions	User is on the registration page.
#### Test Steps	
1. Navigate to Register page
2. Fill all fields with valid data
3. Enter password: Test@1234
4. Enter confirm password: Different123
5. Click 'Register'


### TC-REG-006  Registration with password at minimum boundary (6 chars)
#### Module	Registration     Type: BVA     Priority: P2
#### Preconditions	User is on the registration page.
#### Test Steps	
1. Navigate to Register page
2. Fill name and email fields
3. Enter password: 'Ab1234' (exactly 6 chars)
4. Enter confirm password: 'Ab1234'
5. Click 'Register'


### TC-REG-007  Registration with password below minimum (5 chars)
#### Module	Registration     Type: BVA     Priority: P2
#### Preconditions	User is on the registration page.
#### Test Steps	
1. Navigate to Register page
2. Fill name and email fields
3. Enter password: 'Ab123' (5 chars)
4. Enter confirm password: 'Ab123'
5. Click 'Register'


### TC-REG-008  Registration with special characters in name fields
#### Module	Registration     Type: Exploratory     Priority: P3
#### Preconditions	User is on the registration page.
#### Test Steps	
1. Navigate to Register page
2. Enter first name: "O'Brien"
3. Enter last name: 'St. Claire-Jones'
4. Enter valid email and password
5. Click 'Register'



## Module: Login
### TC-LOG-001  Successful login with valid credentials
#### Module	Login     Type: Positive     Priority: P1
#### Preconditions	Registered user account exists.
#### Test Steps
1. Navigate to demowebshop.tricentis.com
2. Click 'Log in' in header
3. Enter valid email address
4. Enter valid password
5. Click 'Log in' button


### TC-LOG-002  Login with invalid password
#### Module	Login     Type: Negative     Priority: P1
#### Preconditions	Registered user account exists.
#### Test Steps
1. Navigate to Login page
2. Enter valid email
3. Enter wrong password: 'WrongPass999'
4. Click 'Log in'


### TC-LOG-003  Login with unregistered email
#### Module	Login     Type: Negative     Priority: P1
#### Preconditions	No account exists for notexist@test.com.
#### Test Steps	
1. Navigate to Login page
2. Enter email: notexist@test.com
3. Enter any password
4. Click 'Log in'


### TC-LOG-004  Login with blank email and password
#### Module	Login     Type: Negative     Priority: P2
#### Preconditions	User is on login page.
#### Test Steps
1. Navigate to Login page
2. Leave email field empty
3. Leave password field empty
4. Click 'Log in'


### TC-LOG-005  'Remember me' checkbox retains session
#### Module	Login     Type: Exploratory     Priority: P3
#### Preconditions	Registered user account exists.
#### Test Steps	
1. Navigate to Login page
2. Enter valid credentials
3. Check 'Remember me' checkbox
4. Click 'Log in'
5. Close and reopen browser
6. Navigate to site


### TC-LOG-006  Forgot password — email sent for registered email
#### Module	Login     Type: Positive     Priority: P2
#### Preconditions	Registered user account exists.
#### Test Steps
1. Navigate to Login page
2. Click 'Forgot password?' link
3. Enter registered email address
4. Click 'Recover'


### TC-LOG-007  Forgot password — unregistered email
#### Module	Login     Type: Negative     Priority: P2
#### Preconditions	Email notexist@test.com is not registered.
#### Test Steps
1. Navigate to Forgot Password page
2. Enter unregistered email
3. Click 'Recover'


### TC-LOG-008  Logout clears session
#### Module	Login     Type: Positive     Priority: P1
#### Preconditions	User is logged in.
#### Test Steps
1. Verify user is logged in (name in header)
2. Click 'Log out' link
3. Observe page redirect
4. Try to access account page directly via URL



## Module: Search
### TC-SRC-001  Search with valid existing product keyword
#### Module	Search     Type: Positive     Priority: P1
#### Preconditions	User on homepage (logged in or guest).
#### Test Steps	
1. Locate search bar in header
2. Type 'computer' in search field
3. Click search button or press Enter


### TC-SRC-002  Search with keyword returning no results
#### Module	Search     Type: Negative     Priority: P2
#### Preconditions	User on homepage.
#### Test Steps
1. Type 'xyznotexistproduct12345' in search bar
2. Press Enter or click Search


### TC-SRC-003  Search with empty string
#### Module	Search     Type: Negative     Priority: P2
#### Preconditions	User on homepage.
#### Test Steps	
1. Click on search field without typing anything
2. Click search button


### TC-SRC-004  Search with XSS injection payload
#### Module	Search     Type: Negative     Priority: P3
#### Preconditions	User on homepage.
#### Test Steps	
1. Type '<script>alert(1)</script>' in search bar
2. Click Search


### TC-SRC-005  Search results — sort by price ascending
#### Module	Search     Type: Positive     Priority: P2
#### Preconditions	Search results showing multiple products.
#### Test Steps
1. Perform a search for 'book'
2. Locate 'Sort by' dropdown
3. Select 'Price: Low to High'


### TC-SRC-006  Search results — change display per page to 12
#### Module	Search     Type: Positive     Priority: P3
#### Preconditions	Search results page with more than 4 results.
#### Test Steps
1. Perform search returning many products
2. Locate 'Display per page' dropdown
3. Select '12'


### TC-SRC-007  Category navigation — Books
#### Module	Search     Type: Positive     Priority: P2
#### Preconditions	User on homepage.
#### Test Steps	
1. Click 'Books' in left navigation categories
2. Verify category page loads
3. Observe products displayed



## Module: Product
### TC-PRD-001  Product detail page loads with all required elements
#### Module	Product     Type: Positive     Priority: P1
#### Preconditions	User on homepage or search results.
#### Test Steps	
1. Search for 'simple computer'
2. Click on the product name/image
3. Observe product detail page


### TC-PRD-002  Add to cart from product detail page
#### Module	Product     Type: Positive     Priority: P1
#### Preconditions	User on product detail page (logged in or guest).
#### Test Steps
1. Navigate to any product detail page
2. Set quantity to 1
3. Click 'Add to cart' button
4. Observe notification


### TC-PRD-003  Add to cart with quantity set to 0
#### Module	Product     Type: BVA     Priority: P2
#### Preconditions	User on product detail page.
#### Test Steps
1. Navigate to product detail page
2. Clear quantity field and enter '0'
3. Click 'Add to cart'


### TC-PRD-004  Add to cart with negative quantity
#### Module	Product     Type: Negative     Priority: P2
#### Preconditions	User on product detail page.
#### Test Steps	
1. Navigate to product detail page
2. Enter '-1' in quantity field
3. Click 'Add to cart'


### TC-PRD-005  Add to cart with very large quantity (999999)
#### Module	Product     Type: BVA     Priority: P3
#### Preconditions	User on product detail page.
#### Test Steps	
1. Navigate to product detail page
2. Enter '999999' in quantity field
3. Click 'Add to cart'


### TC-PRD-006  Add product to wishlist (logged in)
#### Module	Product     Type: Positive     Priority: P2
#### Preconditions	User is logged in. On product detail page.
#### Test Steps	
1. Navigate to product detail page
2. Click 'Add to wishlist' button
3. Observe notification


### TC-PRD-007  Add to wishlist as guest (not logged in)
#### Module	Product     Type: Negative     Priority: P2
#### Preconditions	User is NOT logged in.
#### Test Steps	
1. Navigate to product detail page as guest
2. Click 'Add to wishlist'


### TC-PRD-008  Product page breadcrumb navigation
#### Module	Product     Type: Positive     Priority: P3
#### Preconditions	User navigated to a product via category.
#### Test Steps
1. Click a category (e.g., Computers > Desktops)
2. Click on a product
3. Verify breadcrumb trail
4. Click each breadcrumb link



## Module: Cart
### TC-CART-001  View shopping cart with items
#### Module	Cart     Type: Positive     Priority: P1
#### Preconditions	At least one product added to cart.
#### Test Steps	
1. Add a product to cart
2. Click shopping cart link in header
3. Observe cart page


### TC-CART-002  Update product quantity in cart
#### Module	Cart     Type: Positive     Priority: P2
#### Preconditions	Cart has at least one product.
#### Test Steps	
1. Navigate to shopping cart
2. Change quantity of a product from 1 to 3
3. Click 'Update shopping cart'


### TC-CART-003  Remove product from cart
#### Module	Cart     Type: Positive     Priority: P1
#### Preconditions	Cart has at least one product.
#### Test Steps	
1. Navigate to shopping cart
2. Click the remove checkbox/button next to a product
3. Click 'Update shopping cart'


### TC-CART-004  Apply invalid coupon code
#### Module	Cart     Type: Negative     Priority: P2
#### Preconditions	Cart has at least one product.
#### Test Steps
1. Navigate to shopping cart
2. Locate coupon code field
3. Enter 'INVALIDCOUPON123'
4. Click 'Apply coupon'


### TC-CART-005  Proceed to checkout without accepting terms
#### Module	Cart     Type: Negative     Priority: P1
#### Preconditions	Cart has at least one product. User on cart page.
#### Test Steps
1. Navigate to shopping cart
2. Do NOT check 'I agree with the terms of service' checkbox
3. Click 'Checkout'


### TC-CART-006  Empty cart — checkout button behavior
#### Module	Cart     Type: Exploratory     Priority: P2
#### Preconditions	Cart is empty.
#### Test Steps
1. Navigate to shopping cart page when no items added
2. Observe page state
3. Try clicking Checkout if visible


### TC-CART-007  Cart persists across page navigation
Module	Cart     Type: Exploratory     Priority: P2
Preconditions	User adds items to cart.
Test Steps
1. Add product to cart
2. Navigate to other pages (Home, Category, Product)
3. Return to cart



## Module: Checkout
### TC-CHK-001  Guest checkout — full end-to-end flow
#### Module	Checkout     Type: Positive     Priority: P1
#### Preconditions	Cart has at least one item. User is NOT logged in.
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


### TC-CHK-002  Registered user checkout — credit card payment
#### Module	Checkout     Type: Positive     Priority: P1
#### Preconditions	User logged in. Cart has items.
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


### TC-CHK-003  Checkout — billing address with missing required field
#### Module	Checkout     Type: Negative     Priority: P1
#### Preconditions	In checkout billing address step.
#### Test Steps
1. Reach billing address step
2. Leave 'City' field empty
3. Fill all other required fields
4. Click Continue


### TC-CHK-004  Checkout — invalid zip code format
#### Module	Checkout     Type: Negative     Priority: P2
#### Preconditions	In checkout billing address step.
#### Test Steps
1. Enter billing address
2. Enter zip code: 'ABCDE' (non-numeric)
3. Click Continue


### TC-CHK-005  Shipping method — Next Day Air selection
#### Module	Checkout     Type: Positive     Priority: P2
#### Preconditions	In shipping method step of checkout.
#### Test Steps
1. Reach shipping method step
2. Select 'Next Day Air' shipping option
3. Click Continue


### TC-CHK-006  Payment method — Purchase Order
#### Module	Checkout     Type: Positive     Priority: P2
#### Preconditions	In payment step. Purchase Order method available.
#### Test Steps	
1. Reach payment method step
2. Select 'Purchase Order'
3. Enter PO number: 'PO-2024-001'
4. Click Continue
5. Confirm order


### TC-CHK-007  Checkout — browser back button integrity
#### Module	Checkout     Type: Exploratory     Priority: P3
#### Preconditions	User is in middle of checkout (at payment step).
#### Test Steps
1. Proceed through checkout to payment step
2. Use browser back button
3. Observe page and cart state


### TC-CHK-008  Order confirmation — unique order number generated
#### Module	Checkout     Type: Positive     Priority: P1
#### Preconditions	Order placed successfully.
#### Test Steps
1. Complete the full checkout process
2. Observe the confirmation page



## Module: Account
### TC-ACC-001  My account — order history displays past orders
#### Module	Account     Type: Positive     Priority: P2
#### Preconditions	User logged in. At least one order placed.
#### Test Steps
1. Log in with account that has orders
2. Click on username/My Account in header
3. Navigate to 'Orders' section


### TC-ACC-002  Change account password — valid new password
#### Module	Account     Type: Positive     Priority: P2
#### Preconditions	User is logged in.
#### Test Steps
1. Navigate to My Account > Change Password
2. Enter current password
3. Enter new password: NewPass@5678
4. Enter confirm new password: NewPass@5678
5. Click 'Change Password'


### TC-ACC-003  Change password — incorrect current password
#### Module	Account     Type: Negative     Priority: P2
#### Preconditions	User is logged in.
#### Test Steps
1. Navigate to Change Password
2. Enter an incorrect current password
3. Enter new password and confirmation
4. Click 'Change Password'


### TC-ACC-004  Edit account info — update name
#### Module	Account     Type: Positive     Priority: P2
#### Preconditions	User is logged in.
#### Test Steps
1. Navigate to My Account > Account Info
2. Update First Name to 'UpdatedName'
3. Click 'Save'


### TC-ACC-005  Downloadable products — access after purchase
#### Module	Account     Type: Exploratory     Priority: P3
#### Preconditions	User purchased a digital download product.
#### Test Steps
1. Navigate to My Account
2. Click 'Downloadable products'
3. Attempt to download purchased product



## Module: Wishlist
### TC-WSH-001  Add product to wishlist and view wishlist page
#### Module	Wishlist     Type: Positive     Priority: P2
#### Preconditions	User is logged in.
#### Test Steps
1. Navigate to any product detail page
2. Click 'Add to wishlist'
3. Click 'Wishlist' link in header
4. Observe wishlist page


### TC-WSH-002  Move product from wishlist to cart
#### Module	Wishlist     Type: Positive     Priority: P2
#### Preconditions	User logged in. Wishlist has at least one item.
#### Test Steps
1. Navigate to Wishlist
2. Select the product (checkbox or Add to cart button)
3. Click 'Add to cart'


### TC-WSH-003  Remove product from wishlist
#### Module	Wishlist     Type: Positive     Priority: P2
#### Preconditions	User logged in. Wishlist has at least one item.
#### Test Steps
1. Navigate to Wishlist
2. Click remove button next to a product
3. Confirm if prompted


### TC-WSH-004  Share wishlist via public URL
#### Module	Wishlist     Type: Exploratory     Priority: P3
#### Preconditions	User logged in with items in wishlist.
#### Test Steps	
1. Navigate to Wishlist page
2. Locate 'Wishlist URL for sharing' field
3. Copy the URL
4. Open the URL in a new incognito browser session



## Module: Navigation
### TC-NAV-001  Homepage loads with all 7 product categories
#### Module	Navigation     Type: Positive     Priority: P1
#### Preconditions	Browser open, no prior session needed.
#### Test Steps
1. Navigate to demowebshop.tricentis.com
2. Observe left sidebar categories


### TC-NAV-002  Computers subcategories — Desktops and Notebooks
#### Module	Navigation     Type: Positive     Priority: P2
#### Preconditions	User on homepage.
#### Test Steps
1. Click 'Computers' in category nav
2. Observe subcategories or hover to expand
3. Click 'Desktops'
4. Verify products shown
5. Navigate back, click 'Notebooks'
6. Verify products shown

======================================
# Final QA Test Cases - Manual + AI



### TC-REG-001 Module: Registration Scenario: Register user with valid
details Type: Positive Priority: P1 Precondition: User is not registered
Steps: Open Register → Enter valid details → Submit

### TC-REG-002 Module: Registration Scenario: Validate mandatory fields
during registration Type: Negative Priority: P1 Precondition: User is on
registration page Steps: Leave mandatory fields empty → Submit

### TC-REG-003 Module: Registration Scenario: Register using existing email
Type: Negative Priority: P1 Precondition: Email already registered
Steps: Enter existing email → Submit

### TC-LOG-001 Module: Login Scenario: Login with valid credentials Type:
Positive Priority: P1 Precondition: Registered user exists Steps: Enter
valid email/password → Login

### TC-LOG-002 Module: Login Scenario: Login with invalid password Type:
Negative Priority: P1 Precondition: Registered email exists Steps: Enter
wrong password → Login

### TC-SRC-001 Module: Search Scenario: Search existing product Type:
Positive Priority: P1 Precondition: User on homepage Steps: Enter
product keyword → Search

### TC-PRD-001 Module: Product Scenario: Product detail page validation
Type: Positive Priority: P1 Precondition: Product available Steps: Open
product → Verify details

### TC-PRD-002 Module: Product Scenario: Add product to cart Type: Positive
Priority: P1 Precondition: Product page opened Steps: Click Add to Cart

### TC-CART-001 Module: Cart Scenario: View cart with added product Type:
Positive Priority: P1 Precondition: Product added Steps: Open cart page

TC-CART-002 Module: Cart Scenario: Update product quantity Type:
Positive Priority: P2 Precondition: Cart contains product Steps: Change
quantity → Update cart

### TC-CHK-001 Module: Checkout Scenario: Complete guest checkout flow Type:
Positive Priority: P1 Precondition: Cart contains item Steps: Checkout →
Enter details → Confirm order

### TC-CHK-002 Module: Checkout Scenario: Complete registered user checkout
Type: Positive Priority: P1 Precondition: Logged in user with cart item
Steps: Checkout → Payment → Confirm

### TC-ACC-001 Module: Account Scenario: Verify order history Type: Positive
Priority: P2 Precondition: User has previous order Steps: Open My
Account → Orders

### TC-WSH-001 Module: Wishlist Scenario: Add and view wishlist item Type:
Positive Priority: P2 Precondition: User logged in Steps: Add product →
Open wishlist

### TC-NAV-001 Module: Navigation Scenario: Verify homepage categories
navigation Type: Positive Priority: P1 Precondition: Application opened
Steps: Open homepage → Verify categories


=======================================
# Session-2
# QA Test Case Skill

## Purpose

This skill contains a consolidated QA test case structure for web
application testing. Duplicate test scenarios are removed and only
unique functional, negative, and boundary validation scenarios are
maintained.

## Application Coverage

-   Registration
-   Login
-   Search
-   Product
-   Cart
-   Checkout
-   Account
-   Wishlist
-   Navigation

## Test Case Format

Each test case should contain:

-   Test Case ID
-   Module
-   Test Scenario
-   Test Type
-   Priority
-   Preconditions
-   Test Steps

## QA Test Cases

### TC-REG-001

Module: Registration\
Scenario: Register user with valid details\
Type: Positive\
Priority: P1\
Precondition: User is not registered\
Steps: 1. Open Register page 2. Enter valid user details 3. Submit
registration

### TC-REG-002

Module: Registration\
Scenario: Validate mandatory fields during registration\
Type: Negative\
Priority: P1\
Precondition: User is on registration page\
Steps: 1. Leave required fields empty 2. Click Submit 3. Verify
validation message

### TC-LOG-001

Module: Login\
Scenario: Login with valid credentials\
Type: Positive\
Priority: P1\
Precondition: Registered user exists\
Steps: 1. Enter valid email and password 2. Click Login 3. Verify
successful login

### TC-LOG-002

Module: Login\
Scenario: Login with invalid credentials\
Type: Negative\
Priority: P1\
Precondition: User account exists\
Steps: 1. Enter incorrect password 2. Click Login 3. Verify error
message

### TC-SRC-001

Module: Search\
Scenario: Search existing product\
Type: Positive\
Priority: P1\
Precondition: User is on homepage\
Steps: 1. Enter product keyword 2. Click Search 3. Verify search results

### TC-PRD-001

Module: Product\
Scenario: Validate product detail page\
Type: Positive\
Priority: P1\
Precondition: Product is available\
Steps: 1. Open product page 2. Verify product details

### TC-PRD-002

Module: Product\
Scenario: Add product to cart\
Type: Positive\
Priority: P1\
Precondition: Product page is opened\
Steps: 1. Click Add to Cart 2. Verify product added

### TC-CART-001

Module: Cart\
Scenario: View cart items\
Type: Positive\
Priority: P1\
Precondition: Product added to cart\
Steps: 1. Open cart 2. Verify item details

### TC-CART-002

Module: Cart\
Scenario: Update cart quantity\
Type: Positive\
Priority: P2\
Precondition: Cart contains product\
Steps: 1. Change quantity 2. Update cart 3. Verify updated quantity

### TC-CHK-001

Module: Checkout\
Scenario: Complete checkout flow\
Type: Positive\
Priority: P1\
Precondition: Cart contains item\
Steps: 1. Proceed to checkout 2. Enter required details 3. Confirm order

### TC-ACC-001

Module: Account\
Scenario: Verify order history\
Type: Positive\
Priority: P2\
Precondition: User has previous order\
Steps: 1. Open My Account 2. Navigate to Orders 3. Verify order history

### TC-WSH-001

Module: Wishlist\
Scenario: Add and view wishlist item\
Type: Positive\
Priority: P2\
Precondition: User is logged in\
Steps: 1. Add product to wishlist 2. Open wishlist 3. Verify product

### TC-NAV-001

Module: Navigation\
Scenario: Verify category navigation\
Type: Positive\
Priority: P1\
Precondition: Application homepage loaded\
Steps: 1. Open homepage 2. Navigate categories 3. Verify navigation flow

## QA Guidelines

-   Avoid duplicate test scenarios
-   Maintain positive and negative coverage
-   Include boundary validations where required
-   Keep test cases clear and execution-ready












   





												
													
