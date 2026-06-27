ASSIGNMENT-01 (15/06/26)
----------------------------------

QA Manual Test Cases
------------------------------------
Name: Priyanka Saha
Url: https://automationexercise.com/

TC_AE_001:[Registration]- Verify User Registration with Valid Details

  1. Click Signup/Login.
  2. Enter name and email.
  3. Click Signup.
  4. Fill the registration form.
  5. Submit.
  Expected Result-User account should be created successfully and logged in.

TC_AE_002:[Registration]- Verify User Registration with InValid Email

  1. Click Signup/Login.
  2. Enter a valid name.
  3. Enter invalid email format.
  4. Click Signup.
  Expected Result-Email validation message should appear. 

TC_AE_003: [Registration] - Verify Registration with Existing Email ID

 1. Click Signup/Login.
 2. Enter a valid name.
 3. Enter an already registered email address.  
 4. Click Signup.
 Expected Result-Email validation message should appear. 

TC_AE_004: [Login] -Verify Login with Valid Credentials 

 1. Click Signup/Login.
 2. Enter registered email. .
 3. Enter valid password.   
 4. Click Login.
 Expected Result-Error message should appear.

TC_AE_005: [Login] -Verify Login with Invalid Credentials

 1. Click Signup/Login.
 2. Enter registered email. .
 3. Enter incorrect password.   
 4. Click Login.
 Expected Result-Error message should appear. 

TC_AE_006: [Products] -Verify Product Details Page  

 1. Click on Products
 2. Click View Product. .
 Expected Result-.Product details should be displayed. 

And so on…..

AI Generated Test Cases:
------------------------------------------------------

Name: Priyanka Saha
Url: https://automationexercise.com/

Prompt:
You are a QA Engineer. Write end-to-end functional testcases(Positive and Negative) for given website-https://automationexercise.com/. Output format should be as given below:

TC_AE_001:[Registration]- Verify User Registration with Valid Details

  1. Click Signup/Login.
  2. Enter name and email.
  3. Click Signup.
  4. Fill registration form.
  5. Submit.
Expected Result-User account should be created successfully and logged in.

Output:
---------
Final Test Cases: AI+Manual:
---------------------------------
Registration Module
--------------------------------
TC_AE_001: [Registration] - Verify User Registration with Valid Details
Click Signup/Login.
Enter valid name and email.
Click Signup.
Fill all mandatory registration details.
Click Create Account.
Click Continue.
Expected Result: User account should be created successfully and logged in.

TC_AE_002: [Registration] - Verify Registration with Existing Email
Click Signup/Login.
Enter valid name.
Enter an already registered email address.
Click Signup.
Expected Result: Error message "Email Address already exist!" should be displayed.

TC_AE_003: [Registration] - Verify Registration with Blank Name
Navigate to Signup/Login.
Leave Name field empty.
Enter valid email.
Click Signup.
Expected Result: User should not proceed to account creation page.

TC_AE_004: [Registration] - Verify Registration with Blank Email
Navigate to Signup/Login.
Enter valid name.
Leave Email field empty.
Click Signup.
Expected Result: Validation message should appear for Email field.

TC_AE_005: [Registration] - Verify Registration with Invalid Email Format
Enter valid name.
Enter invalid email (abc@).
Click Signup.
Expected Result: Email validation message should appear.

TC_AE_006: [Registration] - Verify Mandatory Fields During Registration
Start registration process.
Leave mandatory fields blank.
Click Create Account.
Expected Result: Mandatory field validation messages should appear.

TC_AE_007: [Registration] - Verify Password Field Security
Enter password during registration.
Observe password field.
Expected Result: Password characters should be masked.

TC_AE_008: [Registration] - Verify Account Creation with Minimum Required Data
Enter only mandatory details.
Submit registration form.
Expected Result: Account should be created successfully.

Login Module
--------------------------------------------
TC_AE_009: [Login] - Verify Login with Valid Credentials
Click Signup/Login.
Enter registered email.
Enter valid password.
Click Login.
Expected Result: User should be logged in successfully.

TC_AE_010: [Login] - Verify Login with Invalid Password
Enter registered email.
Enter incorrect password.
Click Login.
Expected Result: Error message should appear.

TC_AE_011: [Login] - Verify Login with Unregistered Email
Enter unregistered email.
Enter password.
Click Login.
Expected Result: Login should fail.

TC_AE_012: [Login] - Verify Login with Blank Email
Leave email blank.
Enter password.
Click Login.
Expected Result: Validation message should appear.

TC_AE_013: [Login] - Verify Login with Blank Password
Enter email.
Leave password blank.
Click Login.
Expected Result: Validation message should appear.

TC_AE_014: [Login] - Verify Password Masking
Enter password.
Expected Result: Password should be hidden.

Logout Module
--------------------------------------------
TC_AE_015: [Logout] - Verify User Logout
Login successfully.
Click Logout.
Expected Result: User should be redirected to Login page.

TC_AE_016: [Logout] - Verify Browser Back After Logout
Login and logout.
Click browser Back button.
Expected Result: User should not access secured pages.

Product Module
----------------------------------------------
TC_AE_017: [Products] - Verify Product Page Navigation
Click Products menu.
Expected Result: Products page should open successfully.

TC_AE_018: [Products] - Verify Product Details Page
Open Products page.
Click View Product.
Expected Result: Product details should be displayed.

TC_AE_019: [Products] - Verify Product Search with Valid Keyword
Enter valid product keyword.
Click Search.
Expected Result: Relevant products should appear.

TC_AE_020: [Products] - Verify Search with Invalid Keyword
Enter invalid keyword.
Click Search.
Expected Result: No products found message should appear.

TC_AE_021: [Products] - Verify Search with Empty Keyword
Leave search box blank.
Click Search.
Expected Result: Appropriate validation or all products should display.

TC_AE_022: [Products] - Verify Category Filtering
Select any category.
Expected Result: Products belonging to selected category should appear.

TC_AE_023: [Products] - Verify Brand Filtering
Select product brand.
Expected Result: Brand-specific products should appear.

Cart Module
----------------------------------
TC_AE_024: [Cart] - Verify Add Product to Cart
Open product page.
Click Add to Cart.
Expected Result: Product should be added successfully.

TC_AE_025: [Cart] - Verify Multiple Product Addition
Add multiple products.
Expected Result: All products should appear in cart.

TC_AE_026: [Cart] - Verify Quantity Update
Add product.
Change quantity.
Expected Result: Updated quantity should reflect correctly.

TC_AE_027: [Cart] - Verify Product Removal
Add product.
Remove product.
Expected Result: Product should be removed.

TC_AE_028: [Cart] - Verify Empty Cart
Remove all products.
Expected Result: Cart should display empty message.

TC_AE_029: [Cart] - Verify Cart Persistence After Login
Add products before login.
Login.
Expected Result: Cart items should remain.

Checkout Module
--------------------------------------------
TC_AE_030: [Checkout] - Verify Checkout with Logged-in User
Login.
Add products.
Proceed to checkout.
Expected Result: Checkout page should open.

TC_AE_031: [Checkout] - Verify Checkout Without Login
Add product.
Click Checkout.
Expected Result: User should be asked to login.

TC_AE_032: [Checkout] - Verify Address Details During Checkout
Proceed to checkout.
Expected Result: Registered address should display correctly.

TC_AE_033: [Checkout] - Verify Order Comment Field
Enter comments.
Continue.
Expected Result: Comments should be saved.

Payment Module
-----------------------------------------
TC_AE_034: [Payment] - Verify Successful Payment
Enter valid card details.
Submit payment.
Expected Result: Order should be placed successfully.

TC_AE_035: [Payment] - Verify Payment with Invalid Card Number
Enter invalid card number.
Submit.
Expected Result: Payment should fail.

TC_AE_036: [Payment] - Verify Blank Payment Fields
Leave payment fields empty.
Submit.
Expected Result: Validation messages should appear.

TC_AE_037: [Payment] - Verify Expired Card Details
Enter expired card information.
Submit.
Expected Result: Payment should fail.

Contact Us Module
-----------------------------------
TC_AE_038: [Contact Us] - Verify Contact Form Submission
Open Contact Us.
Enter valid details.
Upload file.
Submit.
Expected Result: Success message should appear.

TC_AE_039: [Contact Us] - Verify Submission with Blank Fields
Leave mandatory fields blank.
Submit.
Expected Result: Validation messages should appear.

TC_AE_040: [Contact Us] - Verify Invalid Email Format
Enter invalid email.
Submit.
Expected Result: Validation error should appear.

Subscription Module
---------------------------------------
TC_AE_041: [Subscription] - Verify Footer Subscription
Scroll to footer.
Enter valid email.
Click Subscribe.
Expected Result: Subscription success message should appear.

TC_AE_042: [Subscription] - Verify Invalid Email Subscription
Enter invalid email.
Subscribe.
Expected Result: Validation message should appear.

UI & Validation
------------------------------------------------------
TC_AE_043: [UI] - Verify Logo Navigation
Click website logo.
Expected Result: User should navigate to Home page.

End-to-End Scenarios
------------------------------------
TC_AE_044: [E2E] - Verify Complete Purchase Flow
Register user.
Login.
Search product.
Add to cart.
Checkout.
Make payment.
Confirm order.
Expected Result: Order should be placed successfully.

TC_AE_045: [E2E] - Verify Guest User to Registered User Checkout
Add products as guest.
Register account.
Complete checkout.
Expected Result: Order should complete successfully.

TC_AE_046: [E2E] - Verify Account Deletion
Login.
Click Delete Account.
Confirm deletion.
Expected Result: Account should be deleted successfully.

TC_AE_047: [E2E] - Verify Re-registration with Deleted Email
Delete account.
Register again using same email.
Expected Result: User should be able to create a new account if allowed by application logic.


OBSERVATIONS (SUITABLE/NOT SUITABLE):
--------------------------------------------
AI Generated responses are more structured, well-defined and cover almost all possible scenarios available for testing within a few seconds. It creates a huge number of test cases which must be sorted out by QA manually as per his/her requirement and also must verify whether the AI generated responses are correct or not.
Overall, AI improves quality testing in less time.

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
ASSIGNMENT -02 (22/06/26)
----------------------------------

Name: Priyanka Saha
Url: https://automationexercise.com/

---------------------------------------------------------------

# E-Commerce Test Case Generator Skill

## Name
E-Commerce Test Case Generator

## Purpose
Generate comprehensive, structured, and reusable test cases for any e-commerce web application covering all critical functional and non-functional areas — from user authentication and product discovery to checkout, order management, and post-purchase flows. This skill is framework-agnostic and can be adapted to any e-commerce platform (e.g., fashion, electronics, grocery, health & wellness).

---

## Instructions

1. Analyze the provided input (user story, feature spec, acceptance criteria, or business rule).
2. Identify the e-commerce module or functional area being tested (e.g., Cart, Checkout, Search).
3. Generate test scenarios covering all of the following case types:
   - **Positive cases** — happy path / expected behavior
   - **Negative cases** — invalid inputs, unauthorized access, broken flows
   - **Boundary value cases** — min/max quantities, price limits, character limits
   - **Edge cases** — empty states, zero results, concurrent actions, network drops
   - **UI/UX cases** — layout, responsiveness, accessibility, error message clarity
   - **Security cases** — authentication bypass, injection attempts, session handling
   - **Performance cases** — load time thresholds, image rendering, API response time
4. Write each test case with precise, unambiguous steps reproducible by any tester.
5. Assign priority (High / Medium / Low) based on business impact.
6. Tag each test with the relevant module and test type.
7. Flag any assumption made due to missing specification details.
8. Avoid generating duplicate or overlapping test cases.

---

## Input

The skill accepts one or more of the following:

- User Story (e.g., "As a guest user, I want to add items to the cart without logging in")
- Acceptance Criteria
- Feature Specification or PRD excerpt
- API Documentation (for backend/integration test cases)
- Business Rules (e.g., "Coupon codes cannot be stacked")
- Module Name only (e.g., "Write test cases for the Wishlist module")
- Bug Report (to derive regression test cases)
- UI Screenshot or Figma description

---

## E-Commerce Module Coverage

When generating test cases, this skill covers the following standard modules:

### 1. Home Page & Navigation
- Hero banners, promotional sliders load correctly
- Category navigation menus (top nav, sidebar, hamburger) work on all breakpoints
- Footer links (About, Contact, T&C, Privacy Policy) are functional
- Breadcrumb trail reflects correct page hierarchy
- Site search bar is accessible from all pages

### 2. User Authentication & Account Management
- New user registration with valid and invalid data
- Login with correct credentials, wrong password, unregistered email
- Password reset via email link (valid/expired token)
- Social login flows (if applicable)
- Session persistence after browser refresh / tab close
- Account logout and session invalidation
- Profile update (name, email, phone, address)
- Account deletion / deactivation

### 3. Product Listing Page (PLP)
- Products display with correct image, name, price, and rating
- Filter options (category, price range, brand, size, rating) work independently and in combination
- Sort options (price low-high, high-low, newest, relevance) produce correct ordering
- Pagination — correct item count per page, navigation between pages
- Infinite scroll (if applicable) — loads next batch without duplicate items
- Out-of-stock badge displays correctly and blocks add-to-cart
- Quick view / hover interactions (if applicable)

### 4. Product Detail Page (PDP)
- Product images, thumbnails, and zoom functionality work correctly
- All variants (size, color, quantity) are selectable and update price/stock dynamically
- Product description, specifications, and reviews render without truncation
- "Add to Cart" and "Buy Now" buttons behave correctly
- Related / recommended products section loads relevant items
- Share product links generate correct URLs
- Breadcrumb reflects correct category path

### 5. Search Functionality
- Keyword search returns relevant results
- Partial keyword, misspelling, and synonym handling
- Empty search bar submission shows validation or all products
- No-results state shows user-friendly message and suggestions
- Search with special characters
- Search filters persist when applied after a new search

### 6. Shopping Cart
- Add single and multiple items to cart
- Update item quantity (increase, decrease, set to zero)
- Remove individual items from cart
- Cart persists across sessions for logged-in users
- Guest cart behavior (persists in session, prompts login at checkout)
- Correct subtotal, item count, and line-item prices shown
- Out-of-stock items flagged if stock changes after cart addition
- Maximum cart item / quantity limits enforced

### 7. Wishlist / Save for Later
- Add item to wishlist from PLP and PDP
- Remove item from wishlist
- Move item from wishlist to cart
- Wishlist persists across sessions (logged-in users)
- Guest user prompted to login/register to save wishlist
- Wishlist item count badge updates in real time

### 8. Coupon Codes & Promotions
- Valid coupon applies correct discount amount
- Invalid, expired, or already-used coupon shows appropriate error
- Stacking multiple coupons (if not allowed, verify block)
- Minimum order value requirement enforced for coupon eligibility
- Discount visible in cart summary and at checkout
- Promotional banners link to correct category / product pages

### 9. Checkout Flow
- Guest checkout without account creation
- Logged-in checkout with pre-filled address
- Add, edit, and delete shipping addresses
- Address form validation (required fields, postcode format, phone format)
- Shipping method selection (standard, express, pickup) and correct fee calculation
- Order summary matches cart contents before payment
- Place order button disabled until all required fields are complete

### 10. Payment Processing
- Successful payment with valid card details
- Declined payment with invalid card number, expired date, wrong CVV
- Payment with saved cards (if applicable)
- Alternative payment methods (UPI, PayPal, Wallet, COD) work end-to-end
- 3DS authentication / OTP verification flow completes correctly
- Payment timeout / network drop handling — no double charge
- Order NOT created if payment fails

### 11. Order Confirmation & Email Notifications
- Order confirmation page displays correct order ID, items, and total
- Confirmation email received with correct order details
- Order appears in "My Orders" immediately after placement
- Invoice / receipt download works (PDF opens correctly)

### 12. Order Management (Post-Purchase)
- Order list displays correct status (Processing, Shipped, Delivered, Cancelled)
- Order detail page shows tracking number and carrier link
- Cancel order within allowed window — refund initiated
- Return / refund request flow (submit reason, upload image if required)
- Reorder from previous order populates cart correctly

### 13. Reviews & Ratings
- Verified-purchase user can submit a rating and text review
- Guest or non-purchaser blocked from submitting review
- Review with prohibited content shows moderation message
- Average rating updates after new review is submitted
- Existing reviews render correctly with date and username

### 14. Responsive Design & Cross-Browser Compatibility
- Layout renders correctly on desktop (1280px+), tablet (768px), and mobile (375px)
- Touch interactions (swipe carousel, tap dropdowns) work on mobile
- All pages tested on Chrome, Firefox, Safari, and Edge
- No horizontal scroll on any breakpoint
- CTA buttons and form inputs are tap-friendly

### 15. Accessibility
- All images have descriptive alt text
- Form fields have associated labels
- Keyboard-only navigation reaches all interactive elements
- Error messages linked to fields

### 16. Performance & Load Behavior
- Home page loads within 3 seconds on a standard connection
- Product images use lazy loading — below-fold images not fetched on page load
- API calls for search/filter return results within 2 seconds
- No broken images or 404 resources on any key page

---

## Output Format

Generate test cases using the following structure:

| Field | Description |
|-------|-------------|
| Test Case ID | Unique identifier — format: `[MODULE]-TC-[NUMBER]` e.g. `CART-TC-001` |
| Title | Short, action-oriented description of what is being tested |
| Module | E-commerce area (Cart, Auth, Search, Checkout, etc.) |
| Priority | High / Medium / Low |
| Test Type | Functional / Negative / Boundary / UI / Security / Performance / Regression |
| Preconditions | System state and data required before execution |
| Test Steps | Numbered, unambiguous steps to execute the test |
| Test Data | Specific input values, credentials, or configurations to use |
| Expected Result | Exact observable outcome that defines pass/fail |
| Actual Result | (Leave blank — filled during execution) |
| Status | Pass / Fail / Blocked / Not Executed (filled during execution) |
| Notes / Assumptions | Any clarification, dependency, or out-of-scope boundary |

---

## Example Test Case

**Test Case ID:** CART-TC-007  
**Title:** Verify cart quantity cannot exceed maximum stock limit  
**Module:** Shopping Cart  
**Priority:** High  
**Test Type:** Boundary  
**Preconditions:** User is logged in; product "Blue Polo Shirt - Size M" has a stock limit of 5 units  
**Test Steps:**
1. Navigate to the product detail page for "Blue Polo Shirt - Size M"
2. Set quantity to 5 and click "Add to Cart"
3. Navigate to the Cart page
4. Attempt to increase the quantity to 6 using the "+" button

**Test Data:** Product with max stock = 5; quantity input = 6  
**Expected Result:** Quantity remains at 5; an inline message displays "Maximum available quantity is 5"  
**Actual Result:** _(to be filled)_  
**Status:** Not Executed  
**Notes:** Behavior may differ if stock is managed server-side vs. client-side validation only

---

## Constraints

- Every test case must have a unique Test Case ID following the `[MODULE]-TC-[NUMBER]` convention.
- Test steps must be written so a junior tester with no product knowledge can execute them without guidance.
- Expected results must describe observable, measurable outcomes — never vague statements like "it should work."
- Do not assume functionality not explicitly stated in the input; flag gaps under Notes / Assumptions.
- Cover at minimum one positive and one negative test per feature described.
- Security and accessibility test cases must be included for any authentication, form, or payment-related feature.
- All test cases must be traceable to the input requirement or user story provided.
- Regression test cases should be flagged explicitly for features that have had past defects.







