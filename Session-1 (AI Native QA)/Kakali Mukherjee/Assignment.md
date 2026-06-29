# Test Cases Report — DemoWebShop (demowebshop.tricentis.com)
# Member:- Kakali Mukherjee
---

## Manual Test Cases (Original)

### MT-001 — Website Access
1. Open any browser and navigate to https://demowebshop.tricentis.com/

**Expected Result:** Website should open successfully.

---

### MT-002 — User Registration
1. Click on 'Register' link at the top of the page
2. Fill in personal details: Gender, First Name, Last Name, Email, Password
3. Enter a valid alpha-numeric, case-sensitive password meeting length requirements
4. Enter the same value in 'Confirm Password'
5. Click 'Register' button

**Expected Result:** Registration should be completed successfully.

---

### MT-003 — User Login
1. Open the site and click on the 'Login' button at the top
2. Enter the registered email and password
3. Click 'Login' button

**Expected Result:** User should be logged into the system.

---

### MT-004 — Forgot Password / Account Recovery
1. Click on 'Forgot Password' link on the login page
2. Enter the new password in the 'Password' field
3. Enter the same value in 'Confirm Password'
4. Click 'Recover' button

**Expected Result:** User should successfully recover their account.

---

### MT-005 — Category Navigation
1. Click on any category from the left panel: Books / Computers / Electronics / Apparel & Shoes / Digital Downloads / Jewelry / Gift Cards
2. Check if any sub-categories exist under the selected category

**Expected Result:** The desired category page should open correctly.

---

### MT-006 — Product Filtering and Selection
1. Click on a product category (e.g., Books)
2. Click on a specific book by name (variable: ${bookName})
3. Use 'Filter by price' and select "Under 25.00"
4. Choose any Category / Sub-Category / Filter Options / Sorting Options

**Expected Result:** The selected/filtered products should be displayed correctly.

---

### MT-007 — Add Book to Cart and Email a Friend
1. Add a product (e.g., Book) to the cart
2. Select "Computing and Internet" category
3. Choose the desired quantity (note: negative values are accepted — no validation present)
4. Press 'Add to cart'
5. Press 'Email a friend'
6. Enter Friend's email address
7. Enter your own email address
8. Add a personal message
9. Click 'Send email'
10. Select 'Add to cart' again if needed
11. Click on 'Shopping Cart' and then 'Go to Cart'
12. Click 'Apply Coupon' if a coupon is available
13. Click 'Add gift card' if a gift card is available

**Expected Result:** The product (Book) should be added to the cart successfully.

---
---

## AI-Generated Test Cases (Original)

### Module: Registration

#### TC-REG-001 — Successful user registration with valid data
**Type:** Positive | **Priority:** P1
**Preconditions:** User is not registered. Browser open at homepage.
1. Navigate to demowebshop.tricentis.com
2. Click 'Register' link in header
3. Select gender (Male/Female)
4. Enter first name: John
5. Enter last name: Smith
6. Enter email: john.smith.test@qa.com
7. Enter password: Test@1234
8. Enter confirm password: Test@1234
9. Click 'Register' button

**Expected Result:** Registration completes successfully; user is redirected or shown a success message.

---

#### TC-REG-002 — Registration with already existing email
**Type:** Negative | **Priority:** P1
**Preconditions:** User 'john.smith.test@qa.com' already registered.
1. Navigate to Register page
2. Fill all fields using the same email as an existing account
3. Click 'Register' button

**Expected Result:** Error message displayed indicating the email is already in use.

---

#### TC-REG-003 — Registration with blank mandatory fields
**Type:** Negative | **Priority:** P1
**Preconditions:** User is on the registration page.
1. Navigate to Register page
2. Leave all fields blank
3. Click 'Register' button

**Expected Result:** Validation errors displayed for all mandatory fields.

---

#### TC-REG-004 — Registration with invalid email format
**Type:** Negative | **Priority:** P2
**Preconditions:** User is on the registration page.
1. Navigate to Register page
2. Enter first name and last name
3. Enter invalid email: 'notanemail'
4. Enter valid password and confirm password
5. Click 'Register'

**Expected Result:** Validation error indicating invalid email format.

---

#### TC-REG-005 — Registration with mismatched passwords
**Type:** Negative | **Priority:** P1
**Preconditions:** User is on the registration page.
1. Navigate to Register page
2. Fill all fields with valid data
3. Enter password: Test@1234
4. Enter confirm password: Different123
5. Click 'Register'

**Expected Result:** Error message stating passwords do not match.

---

#### TC-REG-006 — Registration with password at minimum boundary (6 chars)
**Type:** BVA | **Priority:** P2
**Preconditions:** User is on the registration page.
1. Navigate to Register page
2. Fill name and email fields
3. Enter password: 'Ab1234' (exactly 6 characters)
4. Enter confirm password: 'Ab1234'
5. Click 'Register'

**Expected Result:** Registration succeeds as 6 characters meets the minimum requirement.

---

#### TC-REG-007 — Registration with password below minimum (5 chars)
**Type:** BVA | **Priority:** P2
**Preconditions:** User is on the registration page.
1. Navigate to Register page
2. Fill name and email fields
3. Enter password: 'Ab123' (5 characters)
4. Enter confirm password: 'Ab123'
5. Click 'Register'

**Expected Result:** Validation error indicating password is too short.

---

#### TC-REG-008 — Registration with special characters in name fields
**Type:** Exploratory | **Priority:** P3
**Preconditions:** User is on the registration page.
1. Navigate to Register page
2. Enter first name: "O'Brien"
3. Enter last name: 'St. Claire-Jones'
4. Enter valid email and password
5. Click 'Register'

**Expected Result:** Registration succeeds; special characters in names are accepted.

---

### Module: Login

#### TC-LOG-001 — Successful login with valid credentials
**Type:** Positive | **Priority:** P1
**Preconditions:** Registered user account exists.
1. Navigate to demowebshop.tricentis.com
2. Click 'Log in' in header
3. Enter valid email address
4. Enter valid password
5. Click 'Log in' button

**Expected Result:** User is logged in and redirected to homepage with name visible in header.

---

#### TC-LOG-002 — Login with invalid password
**Type:** Negative | **Priority:** P1
**Preconditions:** Registered user account exists.
1. Navigate to Login page
2. Enter valid email
3. Enter wrong password: 'WrongPass999'
4. Click 'Log in'

**Expected Result:** Error message displayed; login is rejected.

---

#### TC-LOG-003 — Login with unregistered email
**Type:** Negative | **Priority:** P1
**Preconditions:** No account exists for notexist@test.com.
1. Navigate to Login page
2. Enter email: notexist@test.com
3. Enter any password
4. Click 'Log in'

**Expected Result:** Error message stating no account found for the given email.

---

#### TC-LOG-004 — Login with blank email and password
**Type:** Negative | **Priority:** P2
**Preconditions:** User is on login page.
1. Navigate to Login page
2. Leave email field empty
3. Leave password field empty
4. Click 'Log in'

**Expected Result:** Validation errors displayed for both empty fields.

---

#### TC-LOG-005 — 'Remember me' checkbox retains session
**Type:** Exploratory | **Priority:** P3
**Preconditions:** Registered user account exists.
1. Navigate to Login page
2. Enter valid credentials
3. Check 'Remember me' checkbox
4. Click 'Log in'
5. Close and reopen the browser
6. Navigate to the site

**Expected Result:** User session is retained; user remains logged in after browser restart.

---

#### TC-LOG-006 — Forgot password — email sent for registered email
**Type:** Positive | **Priority:** P2
**Preconditions:** Registered user account exists.
1. Navigate to Login page
2. Click 'Forgot password?' link
3. Enter registered email address
4. Click 'Recover'

**Expected Result:** A password recovery email is sent; success message is displayed.

---

#### TC-LOG-007 — Forgot password — unregistered email
**Type:** Negative | **Priority:** P2
**Preconditions:** Email notexist@test.com is not registered.
1. Navigate to Forgot Password page
2. Enter unregistered email
3. Click 'Recover'

**Expected Result:** Appropriate message shown (error or generic message for security).

---

#### TC-LOG-008 — Logout clears session
**Type:** Positive | **Priority:** P1
**Preconditions:** User is logged in.
1. Verify user is logged in (name visible in header)
2. Click 'Log out' link
3. Observe page redirect
4. Attempt to access account page directly via URL

**Expected Result:** Session is cleared; user is redirected and cannot access account pages without logging in again.

---

### Module: Search

#### TC-SRC-001 — Search with valid existing product keyword
**Type:** Positive | **Priority:** P1
**Preconditions:** User on homepage (logged in or guest).
1. Locate search bar in header
2. Type 'computer' in search field
3. Click search button or press Enter

**Expected Result:** Relevant product results are displayed.

---

#### TC-SRC-002 — Search with keyword returning no results
**Type:** Negative | **Priority:** P2
**Preconditions:** User on homepage.
1. Type 'xyznotexistproduct12345' in search bar
2. Press Enter or click Search

**Expected Result:** "No results found" message is displayed.

---

#### TC-SRC-003 — Search with empty string
**Type:** Negative | **Priority:** P2
**Preconditions:** User on homepage.
1. Click on search field without typing anything
2. Click search button

**Expected Result:** Validation message prompting the user to enter a search term.

---

#### TC-SRC-004 — Search with XSS injection payload
**Type:** Negative | **Priority:** P3
**Preconditions:** User on homepage.
1. Type `<script>alert(1)</script>` in search bar
2. Click Search

**Expected Result:** Input is sanitized; no script executes; safe response shown.

---

#### TC-SRC-005 — Search results — sort by price ascending
**Type:** Positive | **Priority:** P2
**Preconditions:** Search results showing multiple products.
1. Perform a search for 'book'
2. Locate 'Sort by' dropdown
3. Select 'Price: Low to High'

**Expected Result:** Products are reordered from lowest to highest price.

---

#### TC-SRC-006 — Search results — change display per page to 12
**Type:** Positive | **Priority:** P3
**Preconditions:** Search results page with more than 4 results.
1. Perform a search returning many products
2. Locate 'Display per page' dropdown
3. Select '12'

**Expected Result:** Up to 12 products are displayed per page.

---

#### TC-SRC-007 — Category navigation — Books
**Type:** Positive | **Priority:** P2
**Preconditions:** User on homepage.
1. Click 'Books' in left navigation categories
2. Verify category page loads
3. Observe products displayed

**Expected Result:** Books category page loads with relevant products listed.

---

### Module: Product

#### TC-PRD-001 — Product detail page loads with all required elements
**Type:** Positive | **Priority:** P1
**Preconditions:** User on homepage or search results.
1. Search for 'simple computer'
2. Click on the product name or image
3. Observe product detail page

**Expected Result:** Product detail page displays name, price, description, quantity field, and Add to Cart button.

---

#### TC-PRD-002 — Add to cart from product detail page
**Type:** Positive | **Priority:** P1
**Preconditions:** User on product detail page (logged in or guest).
1. Navigate to any product detail page
2. Set quantity to 1
3. Click 'Add to cart' button
4. Observe notification

**Expected Result:** Product is added to cart; success notification is displayed.

---

#### TC-PRD-003 — Add to cart with quantity set to 0
**Type:** BVA | **Priority:** P2
**Preconditions:** User on product detail page.
1. Navigate to product detail page
2. Clear quantity field and enter '0'
3. Click 'Add to cart'

**Expected Result:** Validation error displayed; product not added to cart.

---

#### TC-PRD-004 — Add to cart with negative quantity
**Type:** Negative | **Priority:** P2
**Preconditions:** User on product detail page.
1. Navigate to product detail page
2. Enter '-1' in quantity field
3. Click 'Add to cart'

**Expected Result:** Validation error displayed; negative quantity should not be accepted. (Known issue: system may accept negative values — bug to be logged.)

---

#### TC-PRD-005 — Add to cart with very large quantity (999999)
**Type:** BVA | **Priority:** P3
**Preconditions:** User on product detail page.
1. Navigate to product detail page
2. Enter '999999' in quantity field
3. Click 'Add to cart'

**Expected Result:** System either accepts (within stock limits) or displays an appropriate error.

---

#### TC-PRD-006 — Add product to wishlist (logged in)
**Type:** Positive | **Priority:** P2
**Preconditions:** User is logged in. On product detail page.
1. Navigate to product detail page
2. Click 'Add to wishlist' button
3. Observe notification

**Expected Result:** Product is added to wishlist; confirmation notification is displayed.

---

#### TC-PRD-007 — Add to wishlist as guest (not logged in)
**Type:** Negative | **Priority:** P2
**Preconditions:** User is NOT logged in.
1. Navigate to product detail page as guest
2. Click 'Add to wishlist'

**Expected Result:** User is redirected to login page or shown a message to log in first.

---

#### TC-PRD-008 — Product page breadcrumb navigation
**Type:** Positive | **Priority:** P3
**Preconditions:** User navigated to a product via category.
1. Click a category (e.g., Computers > Desktops)
2. Click on a product
3. Verify breadcrumb trail
4. Click each breadcrumb link

**Expected Result:** Breadcrumbs reflect correct navigation path; each link navigates correctly.

---

### Module: Cart

#### TC-CART-001 — View shopping cart with items
**Type:** Positive | **Priority:** P1
**Preconditions:** At least one product added to cart.
1. Add a product to cart
2. Click shopping cart link in header
3. Observe cart page

**Expected Result:** Cart page displays all added products with names, quantities, and prices.

---

#### TC-CART-002 — Update product quantity in cart
**Type:** Positive | **Priority:** P2
**Preconditions:** Cart has at least one product.
1. Navigate to shopping cart
2. Change quantity of a product from 1 to 3
3. Click 'Update shopping cart'

**Expected Result:** Quantity is updated; total price is recalculated accordingly.

---

#### TC-CART-003 — Remove product from cart
**Type:** Positive | **Priority:** P1
**Preconditions:** Cart has at least one product.
1. Navigate to shopping cart
2. Click the remove checkbox/button next to a product
3. Click 'Update shopping cart'

**Expected Result:** Product is removed from cart; cart total is updated.

---

#### TC-CART-004 — Apply invalid coupon code
**Type:** Negative | **Priority:** P2
**Preconditions:** Cart has at least one product.
1. Navigate to shopping cart
2. Locate coupon code field
3. Enter 'INVALIDCOUPON123'
4. Click 'Apply coupon'

**Expected Result:** Error message displayed indicating the coupon code is invalid.

---

#### TC-CART-005 — Proceed to checkout without accepting terms
**Type:** Negative | **Priority:** P1
**Preconditions:** Cart has at least one product. User on cart page.
1. Navigate to shopping cart
2. Do NOT check 'I agree with the terms of service' checkbox
3. Click 'Checkout'

**Expected Result:** Validation error displayed; user cannot proceed without accepting terms.

---

#### TC-CART-006 — Empty cart — checkout button behavior
**Type:** Exploratory | **Priority:** P2
**Preconditions:** Cart is empty.
1. Navigate to shopping cart page when no items have been added
2. Observe page state
3. Try clicking Checkout if visible

**Expected Result:** Appropriate message shown (e.g., "Your cart is empty"); Checkout is not accessible.

---

#### TC-CART-007 — Cart persists across page navigation
**Type:** Exploratory | **Priority:** P2
**Preconditions:** User adds items to cart.
1. Add product to cart
2. Navigate to other pages (Home, Category, Product)
3. Return to cart

**Expected Result:** Cart retains all previously added items after navigation.

---

### Module: Checkout

#### TC-CHK-001 — Guest checkout — full end-to-end flow
**Type:** Positive | **Priority:** P1
**Preconditions:** Cart has at least one item. User is NOT logged in.
1. Navigate to cart page
2. Accept terms of service checkbox
3. Click Checkout
4. Select 'Checkout as Guest'
5. Enter billing details: First Name, Last Name, Email, Country, City, Address 1, Zip, Phone
6. Click Continue
7. Select or confirm shipping address
8. Click Continue
9. Select shipping method (e.g., Ground)
10. Click Continue
11. Select payment method (e.g., Cash On Delivery)
12. Click Continue
13. Review order summary
14. Click 'Confirm'

**Expected Result:** Order is placed successfully; confirmation page with order number is displayed.

---

#### TC-CHK-002 — Registered user checkout — credit card payment
**Type:** Positive | **Priority:** P1
**Preconditions:** User logged in. Cart has items.
1. Navigate to cart
2. Accept terms of service
3. Click Checkout
4. Fill or use saved billing address
5. Select shipping method
6. Select payment: Credit Card
7. Enter card details: 4485564059489345, Exp: 04/2027, CVV: 123
8. Click Continue
9. Confirm order

**Expected Result:** Order is placed successfully with credit card payment.

---

#### TC-CHK-003 — Checkout — billing address with missing required field
**Type:** Negative | **Priority:** P1
**Preconditions:** In checkout billing address step.
1. Reach billing address step
2. Leave 'City' field empty
3. Fill all other required fields
4. Click Continue

**Expected Result:** Validation error for the missing City field; cannot proceed.

---

#### TC-CHK-004 — Checkout — invalid zip code format
**Type:** Negative | **Priority:** P2
**Preconditions:** In checkout billing address step.
1. Enter billing address details
2. Enter zip code: 'ABCDE' (non-numeric)
3. Click Continue

**Expected Result:** Validation error indicating invalid zip code format.

---

#### TC-CHK-005 — Shipping method — Next Day Air selection
**Type:** Positive | **Priority:** P2
**Preconditions:** In shipping method step of checkout.
1. Reach shipping method step
2. Select 'Next Day Air' shipping option
3. Click Continue

**Expected Result:** Next Day Air is selected; cost is reflected in the order summary.

---

#### TC-CHK-006 — Payment method — Purchase Order
**Type:** Positive | **Priority:** P2
**Preconditions:** In payment step. Purchase Order method available.
1. Reach payment method step
2. Select 'Purchase Order'
3. Enter PO number: 'PO-2024-001'
4. Click Continue
5. Confirm order

**Expected Result:** Order is placed using Purchase Order payment method.

---

#### TC-CHK-007 — Checkout — browser back button integrity
**Type:** Exploratory | **Priority:** P3
**Preconditions:** User is at payment step in checkout.
1. Proceed through checkout to payment step
2. Use browser back button
3. Observe page and cart state

**Expected Result:** Cart data remains intact; no duplicate orders or broken states occur.

---

#### TC-CHK-008 — Order confirmation — unique order number generated
**Type:** Positive | **Priority:** P1
**Preconditions:** Order placed successfully.
1. Complete the full checkout process
2. Observe the confirmation page

**Expected Result:** Unique order number is generated and displayed on the confirmation page.

---

### Module: Account

#### TC-ACC-001 — My account — order history displays past orders
**Type:** Positive | **Priority:** P2
**Preconditions:** User logged in. At least one order placed.
1. Log in with an account that has existing orders
2. Click on username/My Account in header
3. Navigate to 'Orders' section

**Expected Result:** Order history lists all past orders with relevant details.

---

#### TC-ACC-002 — Change account password — valid new password
**Type:** Positive | **Priority:** P2
**Preconditions:** User is logged in.
1. Navigate to My Account > Change Password
2. Enter current password
3. Enter new password: NewPass@5678
4. Enter confirm new password: NewPass@5678
5. Click 'Change Password'

**Expected Result:** Password is updated successfully; confirmation message is shown.

---

#### TC-ACC-003 — Change password — incorrect current password
**Type:** Negative | **Priority:** P2
**Preconditions:** User is logged in.
1. Navigate to Change Password
2. Enter an incorrect current password
3. Enter new password and confirmation
4. Click 'Change Password'

**Expected Result:** Error message displayed; password is not changed.

---

#### TC-ACC-004 — Edit account info — update name
**Type:** Positive | **Priority:** P2
**Preconditions:** User is logged in.
1. Navigate to My Account > Account Info
2. Update First Name to 'UpdatedName'
3. Click 'Save'

**Expected Result:** Account info is updated; name change is reflected in the header.

---

#### TC-ACC-005 — Downloadable products — access after purchase
**Type:** Exploratory | **Priority:** P3
**Preconditions:** User purchased a digital download product.
1. Navigate to My Account
2. Click 'Downloadable products'
3. Attempt to download purchased product

**Expected Result:** Download link is accessible and product downloads successfully.

---

### Module: Wishlist

#### TC-WSH-001 — Add product to wishlist and view wishlist page
**Type:** Positive | **Priority:** P2
**Preconditions:** User is logged in.
1. Navigate to any product detail page
2. Click 'Add to wishlist'
3. Click 'Wishlist' link in header
4. Observe wishlist page

**Expected Result:** Wishlist page displays the added product correctly.

---

#### TC-WSH-002 — Move product from wishlist to cart
**Type:** Positive | **Priority:** P2
**Preconditions:** User logged in. Wishlist has at least one item.
1. Navigate to Wishlist
2. Select the product checkbox or click 'Add to cart'
3. Click 'Add to cart'

**Expected Result:** Product is moved/added to cart; cart count is updated.

---

#### TC-WSH-003 — Remove product from wishlist
**Type:** Positive | **Priority:** P2
**Preconditions:** User logged in. Wishlist has at least one item.
1. Navigate to Wishlist
2. Click remove button next to a product
3. Confirm if prompted

**Expected Result:** Product is removed from wishlist; wishlist is updated.

---

#### TC-WSH-004 — Share wishlist via public URL
**Type:** Exploratory | **Priority:** P3
**Preconditions:** User logged in with items in wishlist.
1. Navigate to Wishlist page
2. Locate 'Wishlist URL for sharing' field
3. Copy the URL
4. Open the URL in a new incognito browser session

**Expected Result:** Wishlist is accessible to others via the shared URL without login.

---

### Module: Navigation

#### TC-NAV-001 — Homepage loads with all 7 product categories
**Type:** Positive | **Priority:** P1
**Preconditions:** Browser open, no prior session needed.
1. Navigate to demowebshop.tricentis.com
2. Observe left sidebar categories

**Expected Result:** All 7 categories are visible: Books, Computers, Electronics, Apparel & Shoes, Digital Downloads, Jewelry, Gift Cards.

---

#### TC-NAV-002 — Computers subcategories — Desktops and Notebooks
**Type:** Positive | **Priority:** P2
**Preconditions:** User on homepage.
1. Click 'Computers' in category nav
2. Observe subcategories or hover to expand
3. Click 'Desktops'
4. Verify products are shown
5. Navigate back and click 'Notebooks'
6. Verify products are shown

**Expected Result:** Both Desktops and Notebooks subcategory pages load with relevant products.

---
---

# Final Test Cases: AI + Human Thinking

> These test cases are derived by merging manual test case insights (real-world observations, known bugs, workflow nuances) with AI-generated structured coverage (BVA, negative, exploratory). Duplicates are consolidated and gaps are filled.

---

## Module: Registration

### TC_Final_001 — Successful Registration with Valid Data
1. Navigate to https://demowebshop.tricentis.com/
2. Click the 'Register' link in the page header
3. Select gender (Male or Female)
4. Enter First Name: John
5. Enter Last Name: Smith
6. Enter Email: john.smith.test@qa.com
7. Enter Password: Test@1234 (alpha-numeric, case-sensitive, meets minimum length)
8. Enter Confirm Password: Test@1234
9. Click 'Register' button

**Expected Result:** Registration completes successfully. User is redirected or shown a confirmation message. Account is created.

---

### TC_Final_002 — Registration with Duplicate Email
1. Navigate to the Register page
2. Fill in all fields using an email already registered in the system (e.g., john.smith.test@qa.com)
3. Click 'Register'

**Expected Result:** An error message is displayed indicating the email address is already registered. Registration is blocked.

---

### TC_Final_003 — Registration with All Fields Left Blank
1. Navigate to the Register page
2. Leave all fields empty (Gender unselected, no name, no email, no password)
3. Click 'Register'

**Expected Result:** Validation errors are displayed for all mandatory fields. Registration is not submitted.

---

### TC_Final_004 — Registration with Invalid Email Format
1. Navigate to the Register page
2. Enter First Name and Last Name
3. Enter an invalid email: notanemail
4. Enter a valid password and confirm password
5. Click 'Register'

**Expected Result:** Validation error displayed indicating the email format is invalid.

---

### TC_Final_005 — Registration with Mismatched Passwords
1. Navigate to the Register page
2. Fill in all other fields with valid data
3. Enter Password: Test@1234
4. Enter Confirm Password: Different123
5. Click 'Register'

**Expected Result:** Error message displayed stating passwords do not match. Account is not created.

---

### TC_Final_006 — Registration with Password at Minimum Boundary (6 Characters)
1. Navigate to the Register page
2. Fill in name and email fields
3. Enter Password: Ab1234 (exactly 6 characters)
4. Enter Confirm Password: Ab1234
5. Click 'Register'

**Expected Result:** Registration succeeds as 6 characters is the minimum accepted length.

---

### TC_Final_007 — Registration with Password Below Minimum (5 Characters)
1. Navigate to the Register page
2. Fill in name and email fields
3. Enter Password: Ab123 (5 characters)
4. Enter Confirm Password: Ab123
5. Click 'Register'

**Expected Result:** Validation error displayed indicating password does not meet minimum length requirement.

---

### TC_Final_008 — Registration with Special Characters in Name Fields
1. Navigate to the Register page
2. Enter First Name: O'Brien
3. Enter Last Name: St. Claire-Jones
4. Enter a valid email and password
5. Click 'Register'

**Expected Result:** Registration succeeds. Special characters in name fields are accepted and stored correctly.

---

## Module: Login

### TC_Final_009 — Successful Login with Valid Credentials
1. Navigate to https://demowebshop.tricentis.com/
2. Click 'Log in' in the header
3. Enter the registered email address
4. Enter the correct password
5. Click 'Log in'

**Expected Result:** User is logged in successfully. User's name/account is visible in the page header.

---

### TC_Final_010 — Login with Incorrect Password
1. Navigate to the Login page
2. Enter a valid registered email
3. Enter an incorrect password: WrongPass999
4. Click 'Log in'

**Expected Result:** Error message is displayed. Login is rejected. User remains on the login page.

---

### TC_Final_011 — Login with Unregistered Email
1. Navigate to the Login page
2. Enter email: notexist@test.com
3. Enter any password
4. Click 'Log in'

**Expected Result:** Error message displayed indicating no account exists for the provided email.

---

### TC_Final_012 — Login with Empty Fields
1. Navigate to the Login page
2. Leave both email and password fields empty
3. Click 'Log in'

**Expected Result:** Validation errors displayed for both fields. Login is not attempted.

---

### TC_Final_013 — Forgot Password Flow for Registered Email
1. Navigate to the Login page
2. Click 'Forgot password?' link
3. Enter the registered email address
4. Click 'Recover'

**Expected Result:** Password recovery email is sent. Success confirmation is displayed on screen.

---

### TC_Final_014 — Forgot Password Flow for Unregistered Email
1. Navigate to the Forgot Password page
2. Enter an unregistered email: notexist@test.com
3. Click 'Recover'

**Expected Result:** Appropriate message is shown (error or generic security message). No recovery email is sent.

---

### TC_Final_015 — Logout Clears Session and Blocks Protected Pages
1. Verify user is logged in (name visible in header)
2. Click 'Log out'
3. Observe the page redirect
4. Attempt to access the account page directly via URL

**Expected Result:** Session is cleared. User is redirected to the homepage or login page. Direct URL access to account page is blocked.

---

### TC_Final_016 — Remember Me Persists Session After Browser Close
1. Navigate to the Login page
2. Enter valid credentials
3. Check the 'Remember me' checkbox
4. Click 'Log in'
5. Close the browser completely
6. Reopen the browser and navigate to the site

**Expected Result:** User remains logged in after browser restart without needing to re-enter credentials.

---

## Module: Search & Navigation

### TC_Final_017 — Search with Valid Product Keyword
1. Locate the search bar in the header
2. Type 'computer' in the search field
3. Click the search button or press Enter

**Expected Result:** Search results page loads displaying relevant products matching the keyword.

---

### TC_Final_018 — Search with No Matching Results
1. Type 'xyznotexistproduct12345' in the search bar
2. Press Enter or click Search

**Expected Result:** A "No products were found" or similar no-results message is displayed.

---

### TC_Final_019 — Search with Empty Input
1. Click the search field without entering any text
2. Click the search button

**Expected Result:** Validation message prompts the user to enter a search term. No search is performed.

---

### TC_Final_020 — Search with XSS Injection Payload (Security)
1. Type `<script>alert(1)</script>` in the search bar
2. Click Search

**Expected Result:** Input is safely sanitized. No script alert executes. A safe results page or no-results page is displayed.

---

### TC_Final_021 — Sort Search Results by Price Low to High
1. Search for 'book'
2. On the results page, locate the 'Sort by' dropdown
3. Select 'Price: Low to High'

**Expected Result:** Products are re-ordered from lowest to highest price.

---

### TC_Final_022 — Filter Products by Price (Under $25.00)
1. Navigate to the Books category
2. Locate the 'Filter by price' panel
3. Select "Under 25.00"

**Expected Result:** Only products priced under $25.00 are displayed in the results.

---

### TC_Final_023 — Category Navigation — All 7 Categories Accessible
1. Navigate to the homepage
2. Observe the left sidebar
3. Click each of the 7 categories one by one: Books, Computers, Electronics, Apparel & Shoes, Digital Downloads, Jewelry, Gift Cards

**Expected Result:** All 7 category links are visible and each navigates to the correct category page with products listed.

---

### TC_Final_024 — Sub-Category Navigation — Computers > Desktops and Notebooks
1. Click 'Computers' in the left navigation
2. Click 'Desktops' from the sub-categories
3. Verify products are displayed
4. Navigate back and click 'Notebooks'
5. Verify products are displayed

**Expected Result:** Both Desktops and Notebooks sub-category pages load with correct product listings.

---

## Module: Product

### TC_Final_025 — Product Detail Page Displays All Key Elements
1. Search for 'simple computer'
2. Click on the product name or image
3. Inspect the product detail page

**Expected Result:** Page displays product name, price, description, images, quantity field, 'Add to cart' button, and breadcrumb navigation.

---

### TC_Final_026 — Add Product to Cart with Valid Quantity
1. Navigate to any product detail page
2. Set quantity to 1
3. Click 'Add to cart'

**Expected Result:** Product is added to cart. Success notification is shown. Cart count in header is updated.

---

### TC_Final_027 — Add Product to Cart with Quantity = 0 (Boundary)
1. Navigate to a product detail page
2. Clear the quantity field and enter 0
3. Click 'Add to cart'

**Expected Result:** Validation error is displayed. Product is not added to cart.

---

### TC_Final_028 — Add Product to Cart with Negative Quantity (Known Bug)
1. Navigate to a product detail page
2. Enter -1 in the quantity field
3. Click 'Add to cart'

**Expected Result:** Validation error should be displayed preventing negative quantity. **Note:** Known issue — system currently accepts negative values without validation. This is a bug to be logged and tracked.

---

### TC_Final_029 — Add Product to Cart with Very Large Quantity (999999)
1. Navigate to a product detail page
2. Enter 999999 in the quantity field
3. Click 'Add to cart'

**Expected Result:** System either accepts within stock limits or displays an appropriate stock/limit error message.

---

### TC_Final_030 — Email a Friend from Product Page
1. Navigate to a product detail page
2. Click 'Email a friend'
3. Enter a friend's email address
4. Enter your own email address
5. Enter a personal message
6. Click 'Send email'

**Expected Result:** Email is sent successfully. Confirmation message is displayed.

---

### TC_Final_031 — Add Product to Wishlist (Logged In)
1. Log in to the application
2. Navigate to any product detail page
3. Click 'Add to wishlist'

**Expected Result:** Product is added to wishlist. Success notification is displayed.

---

### TC_Final_032 — Add to Wishlist as Guest (Not Logged In)
1. As a guest (not logged in), navigate to a product detail page
2. Click 'Add to wishlist'

**Expected Result:** User is redirected to the login page or shown a message to log in to use the wishlist.

---

### TC_Final_033 — Breadcrumb Navigation from Product Page
1. Click a category (e.g., Computers > Desktops)
2. Click on a product
3. Verify the breadcrumb trail reflects the navigation path
4. Click each breadcrumb link

**Expected Result:** Breadcrumbs are correct and each link navigates back to the appropriate page.

---

## Module: Cart

### TC_Final_034 — View Cart with Added Items
1. Add at least one product to the cart
2. Click the shopping cart link in the header

**Expected Result:** Cart page displays all added products with correct names, quantities, unit prices, and total.

---

### TC_Final_035 — Update Product Quantity in Cart
1. Navigate to the shopping cart
2. Change the quantity of a product from 1 to 3
3. Click 'Update shopping cart'

**Expected Result:** Quantity is updated. Order total is recalculated and displayed correctly.

---

### TC_Final_036 — Remove Product from Cart
1. Navigate to the shopping cart
2. Check the remove checkbox or click the remove button next to a product
3. Click 'Update shopping cart'

**Expected Result:** Product is removed. Cart total is recalculated. Empty cart message shown if no items remain.

---

### TC_Final_037 — Apply Invalid Coupon Code
1. Navigate to shopping cart (with at least one item)
2. Enter 'INVALIDCOUPON123' in the coupon code field
3. Click 'Apply coupon'

**Expected Result:** Error message is displayed indicating the coupon code is invalid or expired.

---

### TC_Final_038 — Apply Valid Gift Card
1. Navigate to shopping cart
2. Enter a valid gift card code in the gift card field
3. Click 'Add gift card'

**Expected Result:** Gift card is applied. Discount amount is reflected in the cart total.

---

### TC_Final_039 — Proceed to Checkout Without Accepting Terms of Service
1. Navigate to the shopping cart with at least one item
2. Do NOT check the 'I agree with the terms of service' checkbox
3. Click 'Checkout'

**Expected Result:** Validation error displayed requiring the user to accept terms before proceeding.

---

### TC_Final_040 — Cart is Empty — Checkout Not Available
1. Navigate to the shopping cart when no items have been added

**Expected Result:** A message such as "Your shopping cart is empty" is shown. Checkout option is not available or leads to an appropriate warning.

---

### TC_Final_041 — Cart Persists Across Page Navigation
1. Add a product to the cart
2. Navigate to the homepage, then a category page, then a product detail page
3. Return to the cart

**Expected Result:** Cart retains all previously added items with correct quantities and prices.

---

## Module: Checkout

### TC_Final_042 — Guest Checkout — Full End-to-End Flow
1. Add at least one item to the cart (as a guest)
2. Navigate to the cart page
3. Accept the terms of service checkbox
4. Click 'Checkout'
5. Select 'Checkout as Guest'
6. Enter billing details: First Name, Last Name, Email, Country, City, Address 1, Zip Code, Phone
7. Click Continue
8. Confirm or select shipping address
9. Click Continue
10. Select a shipping method (e.g., Ground)
11. Click Continue
12. Select payment method (e.g., Cash On Delivery)
13. Click Continue
14. Review the order summary
15. Click 'Confirm'

**Expected Result:** Order is placed successfully. Confirmation page with a unique order number is displayed.

---

### TC_Final_043 — Registered User Checkout with Credit Card
1. Log in to the application
2. Add items to cart
3. Navigate to cart, accept terms of service, click Checkout
4. Use saved or enter new billing address
5. Select shipping method
6. Select payment method: Credit Card
7. Enter: Card No. 4485564059489345, Expiry: 04/2027, CVV: 123
8. Click Continue
9. Confirm the order

**Expected Result:** Order is placed successfully using credit card. Unique order number is shown on confirmation page.

---

### TC_Final_044 — Checkout with Missing Required Billing Field
1. Proceed to the billing address step in checkout
2. Fill all fields except leave 'City' blank
3. Click Continue

**Expected Result:** Validation error for the missing City field is displayed. User cannot proceed to next step.

---

### TC_Final_045 — Checkout with Invalid Zip Code Format
1. Proceed to the billing address step
2. Enter zip code: ABCDE (non-numeric)
3. Fill all other required fields
4. Click Continue

**Expected Result:** Validation error displayed indicating zip code format is invalid.

---

### TC_Final_046 — Select Next Day Air Shipping Method
1. Proceed to the shipping method step in checkout
2. Select 'Next Day Air'
3. Click Continue

**Expected Result:** Next Day Air is selected. Updated shipping cost is reflected in the order summary.

---

### TC_Final_047 — Checkout with Purchase Order Payment
1. Proceed to the payment step
2. Select 'Purchase Order'
3. Enter PO number: PO-2024-001
4. Click Continue
5. Confirm the order

**Expected Result:** Order is placed using Purchase Order. Confirmation page with unique order number displayed.

---

### TC_Final_048 — Browser Back Button During Checkout
1. Proceed through checkout to the payment step
2. Click the browser's back button
3. Observe the page state and cart

**Expected Result:** Cart data is preserved. No duplicate orders are created. Application does not enter a broken state.

---

### TC_Final_049 — Unique Order Number on Confirmation Page
1. Complete the full checkout process (any payment method)
2. Observe the confirmation page

**Expected Result:** A unique order number is generated and prominently displayed on the confirmation page.

---

## Module: Account Management

### TC_Final_050 — View Order History
1. Log in with an account that has past orders
2. Click on the account name or 'My Account' in the header
3. Navigate to the 'Orders' section

**Expected Result:** All past orders are displayed with order numbers, dates, status, and totals.

---

### TC_Final_051 — Change Password with Valid Credentials
1. Log in and navigate to My Account > Change Password
2. Enter current password
3. Enter new password: NewPass@5678
4. Enter confirm new password: NewPass@5678
5. Click 'Change Password'

**Expected Result:** Password is updated successfully. Confirmation message shown. New password works on next login.

---

### TC_Final_052 — Change Password with Incorrect Current Password
1. Log in and navigate to Change Password
2. Enter an incorrect current password
3. Enter a new password and confirmation
4. Click 'Change Password'

**Expected Result:** Error message displayed. Password is not changed.

---

### TC_Final_053 — Edit Account Info — Update Name
1. Log in and navigate to My Account > Account Info
2. Update First Name to 'UpdatedName'
3. Click 'Save'

**Expected Result:** Account info is saved. Updated name is reflected in the header and account info page.

---

### TC_Final_054 — Access Downloadable Products After Purchase
1. Log in with an account that has purchased a digital download
2. Navigate to My Account > Downloadable Products
3. Click the download link for the purchased product

**Expected Result:** Product download initiates successfully.

---

## Module: Wishlist

### TC_Final_055 — Add Product to Wishlist and Verify Wishlist Page
1. Log in to the application
2. Navigate to any product detail page
3. Click 'Add to wishlist'
4. Click 'Wishlist' link in the header
5. Observe the wishlist page

**Expected Result:** Wishlist page displays the added product with correct name, price, and options.

---

### TC_Final_056 — Move Product from Wishlist to Cart
1. Log in and navigate to the Wishlist page
2. Select the product or click 'Add to cart' next to it
3. Confirm action

**Expected Result:** Product is added to cart. Cart count in header is updated.

---

### TC_Final_057 — Remove Product from Wishlist
1. Log in and navigate to the Wishlist page
2. Click the remove button next to a product
3. Confirm if prompted

**Expected Result:** Product is removed from wishlist. Wishlist is updated accordingly.

---

### TC_Final_058 — Share Wishlist via Public URL (Incognito Verification)
1. Log in with items in wishlist
2. Navigate to the Wishlist page
3. Locate the 'Wishlist URL for sharing' field
4. Copy the shared URL
5. Open the URL in a new incognito/private browser session

**Expected Result:** Wishlist is viewable publicly via the shared URL without requiring login.

---

*End of Report*
*Total Final Test Cases: 58*
*Modules Covered: Registration, Login, Search & Navigation, Product, Cart, Checkout, Account Management, Wishlist*
