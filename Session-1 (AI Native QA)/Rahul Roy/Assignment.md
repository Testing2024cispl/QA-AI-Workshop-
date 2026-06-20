**MEMBER:- RAHUL ROY**

# QA Manual Test Cases

**Website:** https://automationexercise.com/
**Sections Covered:** Home | Products | Cart | Signup/Login | Contact Us

---

## Human Thinking Test Cases

---

### TC_AE_001 – Verify homepage title and main headings are displayed correctly.
1. Open the URL: https://automationexercise.com/
2. Verify the page title.
3. Verify the H1 heading 'AutomationExercise' is displayed.
4. Verify the H2 heading 'Full-Fledged practice website for Automation Engineers' is displayed.

---

### TC_AE_002 – Verify navigation to the 'Products' page.
1. Click on the 'Products' link in the header.

---

### TC_AE_003 – Verify navigation to the 'Cart' page.
1. Click on the 'Cart' link in the header.

---

### TC_AE_004 – Verify navigation to the 'Signup / Login' page.
1. Click on the 'Signup / Login' link in the header.

---

### TC_AE_005 – Verify successful subscription with a valid email address.
1. Scroll down to the subscription form.
2. Enter a valid email address into the 'subscribe_email' field.
3. Click the 'Subscribe' button (or equivalent submit action for the form).

---

### TC_AE_006 – Verify subscription with an invalid email format.
1. Scroll down to the subscription form.
2. Enter an invalid email address into the 'subscribe_email' field.
3. Click the 'Subscribe' button.

---

### TC_AE_007 – Verify subscription with an empty email address.
1. Scroll down to the subscription form.
2. Leave the 'subscribe_email' field empty.
3. Click the 'Subscribe' button.

---

### TC_AE_008 – Add a single 'Rs. 500' product to the cart from the homepage.
1. Locate the product with price 'Rs. 500'.
2. Hover over the product to reveal the 'Add to cart' button.
3. Click the 'Add to cart' button.

---

### TC_AE_009 – Verify 'View Cart' button functionality after adding a product.
1. Add a product to the cart (e.g., 'Rs. 500').
2. In the 'Added!' modal, click the 'View Cart' button.

---

### TC_AE_010 – Verify 'Continue Shopping' button functionality after adding a product.
1. Add a product to the cart (e.g., 'Rs. 500').
2. In the 'Added!' modal, click the 'Continue Shopping' button.

---

### TC_AE_011 – Add multiple different products to the cart and verify cart count.
1. Add product 'Rs. 500' to cart.
2. Click 'Continue Shopping'.
3. Add product 'Rs. 400' to cart.
4. Click 'Continue Shopping'.
5. Verify the cart icon count.

---

### TC_AE_012 – Verify navigation to the 'Test Cases' page.
1. Click on the 'Test Cases' link in the header.

---

### TC_AE_013 – Verify navigation to 'API Testing' page via 'APIs list for practice' link.
1. Click on the 'APIs list for practice' link (either in header or main content).

---

### TC_AE_014 – Verify navigation to 'Contact Us' page.
1. Click on the 'Contact us' link in the header.

---

### TC_AE_015 – Verify navigation to 'Women' category and then 'Dress' sub-category.
1. Click on the 'Women' category link in the sidebar.
2. Click on the 'Dress' sub-category link under 'Women'.

---

### TC_AE_016 – Verify navigation to 'Men' category and then 'Jeans' sub-category.
1. Click on the 'Men' category link in the sidebar.
2. Click on the 'Jeans' sub-category link under 'Men'.

---

### TC_AE_017 – Verify navigation to 'Polo' brand products.
1. Click on the '(6)Polo' brand link in the sidebar.

---

### TC_AE_018 – Verify product price displayed on the homepage matches the expected value.
1. Locate the product with the price 'Rs. 1000'.
2. Verify the displayed price.

---

### TC_AE_019 – Attempt to subscribe with an email containing special characters (edge case).
1. Scroll down to the subscription form.
2. Enter an email address with unusual but potentially valid characters into the 'subscribe_email' field.
3. Click the 'Subscribe' button.

---

### TC_AE_020 – Verify Subscription in Cart Page Footer.
1. Open the automationexercise website.
2. Click on "Cart" in the navigation.
3. Scroll to the bottom of the cart page.
4. Look for the "SUBSCRIPTION" footer section.
5. Enter an email address and click the subscribe button.
6. Verify the success subscription confirmation message appears.

---

### TC_AE_021 – Proceed to Checkout as Logged In User.
1. Open the automationexercise website.
2. Log in with a valid registered account.
3. Add a product to the cart.
4. Go to the Cart page.
5. Click the "Proceed to Checkout" button.
6. Verify the checkout page loads showing address details and the order summary.

---

### TC_AE_022 – Verify Address Details on Checkout Page Match Registration.
1. Open the automationexercise website.
2. Register a new user with complete address details.
3. Add a product to the cart.
4. Proceed to Checkout.
5. On the checkout page, verify that both the delivery address and billing address match the address entered at the time of registration.

---

### TC_AE_023 – Register a New User with Valid Details.
1. Open the automationexercise website.
2. Click on "Signup / Login" in the navigation.
3. Verify the "New User Signup!" section is visible.
4. Enter a name and a fresh email address not previously used.
5. Click the "Signup" button.
6. Fill in the complete account form — Title, Name, Email, Password, Date of Birth.
7. Also fill in First Name, Last Name, Company, Address, Country, State, City, Zip Code, and Mobile Number.
8. Optionally check "Sign up for our newsletter!" and "Receive special offers from our partners!".
9. Click "Create Account".
10. Verify the "ACCOUNT CREATED!" message appears.
11. Click "Continue" and check that "Logged in as [username]" is visible in the header.

---

### TC_AE_024 – Register with an Already Existing Email.
1. Open the automationexercise website.
2. Click on "Signup / Login".
3. Enter a name and an email address that is already registered.
4. Click "Signup".
5. Verify an error message "Email Address already exist!" is displayed.

---

### TC_AE_025 – Login with Correct Credentials.
1. Open the automationexercise website.
2. Click "Signup / Login" in the navigation.
3. Find the "Login to your account" section.
4. Enter a valid registered email address and the corresponding password.
5. Click the "Login" button.
6. Verify that "Logged in as [username]" shows up in the header/navigation area.

---

### TC_AE_026 – Login with Wrong Password.
1. Open the automationexercise website.
2. Click "Signup / Login".
3. Enter a valid email but type in the wrong password.
4. Click "Login".
5. Verify an error message "Your email or password is incorrect!" is displayed.

---

### TC_AE_027 – Login with Unregistered Email.
1. Open the automationexercise website.
2. Click "Signup / Login".
3. Enter an email that has never been registered.
4. Enter any password.
5. Click "Login".
6. Verify that an appropriate error message is shown.

---

### TC_AE_028 – Logout Functionality.
1. Open the automationexercise website.
2. Log in with valid credentials.
3. Verify "Logged in as [username]" is shown.
4. Click the "Logout" button from the navigation bar.
5. Confirm the user is signed out and redirected back to the Login page.

---

### TC_AE_029 – Submit Contact Us Form with Valid Data.
1. Open the automationexercise website.
2. Click "Contact Us" in the navigation bar.
3. Verify the "GET IN TOUCH" heading is visible.
4. Fill in your name, email address, subject, and a message.
5. Upload any file (optional field).
6. Click "Submit".
7. On the browser confirmation dialog/popup, click OK.
8. Verify the success message "Success! Your details have been submitted successfully." is displayed.

---

### TC_AE_030 – Submit Contact Us Form with Empty Fields.
1. Open the automationexercise website.
2. Click on "Contact Us".
3. Leave all the fields (name, email, subject, message) completely empty.
4. Try clicking the Submit button.
5. Verify that validation errors or mandatory field warnings appear for the required fields.



---

# AI Manual Test Cases

---

# Prompt

### Role:
Act as a Senior QA Engineer with expertise in Manual Testing, Functional Testing, Regression Testing, and Web Application Testing.

### Task:
Generate comprehensive manual test cases for the AutomationExercise web application. Cover all major functionalities including Home Page, Products Listing, Product Search, Product Filtering, Cart Management, Checkout Flow, User Registration, Login, Logout, Account Management, and Contact Us Form.

### Context:
The application under test is:
https://automationexercise.com/
AutomationExercise is a full-fledged e-commerce practice website where users can:
Register a new account with full address details,
Login with registered credentials,
Browse and explore the home page,
View all products and product details,
Search and filter products by category and brand,
Add products to a shopping cart,
Manage cart items (increase quantity, remove items),
Proceed through the checkout flow with order placement,
Process an order and download the invoice,
Logout from the application,
Delete a registered account,
Submit the Contact Us form,
Subscribe to the newsletter via the footer.

The objective is to validate the complete end-to-end user journey and identify possible functional, validation, and security-related issues across the sections: Home, Products, Cart, Signup/Login, and Contact Us.

### Constraints:
- Include both Positive and Negative test scenarios.
- Include Validation and Error Handling scenarios.
- Include Session Management and Security-related scenarios.
- Consider real-world user behavior and edge cases.
- Avoid duplicate test cases.
- Write test cases in a clear step-by-step format.
- Ensure test cases are suitable for future automation.
- Cover mandatory field validations wherever applicable.
- Include business-critical scenarios such as cart persistence and unauthorized access checks.
- Do NOT include test cases for the Test Cases or API Testing sections.

### Output Format:
TestCase_ID: TestCase_AI_XXX – Test Scenario
Test Steps:
Step 1
Step 2
Step 3
Step 4

---

### TestCase_AI_001 – Verify Home Page is Accessible
1. Open a browser.
2. Navigate to https://automationexercise.com.
3. Verify home page loads without errors.
4. Verify logo is visible.

---

### TestCase_AI_002 – Verify Navigation Links on Home Page
1. Open the website.
2. Observe the top navigation bar.
3. Verify all nav links: Home, Products, Cart, Signup/Login, Contact Us are visible.

---

### TestCase_AI_003 – Verify Subscription with Valid Email on Home Page
1. Open the home page.
2. Scroll to the footer.
3. Verify "SUBSCRIPTION" text is present.
4. Enter a valid email in the subscription field.
5. Click the submit arrow button.
6. Verify success subscription message.

---

### TestCase_AI_004 – Verify Scroll Up Arrow Button on Home Page
1. Navigate to home page.
2. Scroll down to the bottom.
3. Click the scroll-up arrow at bottom-right.
4. Verify the page scrolls to the top.

---

### TestCase_AI_005 – Verify Scroll Up Without Arrow Button
1. Navigate to home page.
2. Scroll down to the bottom.
3. Manually scroll back up using mouse or keyboard.
4. Verify the hero text is visible at the top.

---

### TestCase_AI_006 – Verify All Products Page
1. Click on "Products" in the navigation.
2. Verify the page heading "ALL PRODUCTS" is displayed.
3. Verify a list of products is visible.

---

### TestCase_AI_007 – Verify Product Detail Page
1. Navigate to Products page.
2. Click "View Product" on any product.
3. Verify product name, category, price, availability, condition, and brand are shown.

---

### TestCase_AI_008 – Search Product with Valid Keyword
1. Navigate to Products page.
2. Enter a valid keyword in the search box.
3. Click Search button.
4. Verify "SEARCHED PRODUCTS" heading is visible.
5. Verify matching products are shown.

---

### TestCase_AI_009 – Search Product with Invalid Keyword
1. Navigate to Products page.
2. Enter a random non-existent keyword.
3. Click Search.
4. Verify no results are returned or an appropriate message is shown.

---

### TestCase_AI_010 – Filter Products by Women Category
1. Navigate to website.
2. On the sidebar, click "Women" category.
3. Click a subcategory (e.g., Dress).
4. Verify the correct products are shown for that category.

---

### TestCase_AI_011 – Filter Products by Men Category
1. Navigate to website.
2. On the sidebar, click "Men" category.
3. Click a subcategory (e.g., Tshirts).
4. Verify correct products are shown.

---

### TestCase_AI_012 – Filter Products by Brand
1. Navigate to Products page.
2. Click any brand name from the Brands sidebar.
3. Verify user is taken to the brand page.
4. Verify brand products are displayed.

---

### TestCase_AI_013 – Switch Between Brands
1. Navigate to Products page.
2. Click one brand from the sidebar.
3. Verify brand products load.
4. Click a different brand.
5. Verify the new brand's products are shown.

---

### TestCase_AI_014 – Add Product to Cart from Products Page
1. Navigate to Products page.
2. Hover over a product.
3. Click "Add to cart".
4. Verify modal/popup confirmation appears.

---

### TestCase_AI_015 – Continue Shopping After Adding to Cart
1. Navigate to Products page.
2. Add a product to cart.
3. On the confirmation popup, click "Continue Shopping".
4. Verify the user remains on the Products page.

---

### TestCase_AI_016 – View Cart After Adding Products
1. Add one or more products to the cart.
2. Click "View Cart".
3. Verify the cart page shows all added products with names, prices, quantity, and total.

---

### TestCase_AI_017 – Remove Product from Cart
1. Add a product to the cart.
2. Go to the cart page.
3. Click the "X" button next to the product.
4. Verify the product is removed.

---

### TestCase_AI_018 – Verify Product Quantity in Cart
1. Go to any product detail page.
2. Set quantity to 4.
3. Add to cart.
4. Go to cart.
5. Verify quantity shows as 4.

---

### TestCase_AI_019 – Verify Subscription in Cart Page Footer
1. Navigate to Cart page.
2. Scroll to footer.
3. Enter valid email in the subscription field.
4. Click subscribe.
5. Verify success message.

---

### TestCase_AI_020 – Proceed to Checkout Without Login
1. Add a product to cart.
2. Go to cart.
3. Click "Proceed To Checkout".
4. Verify the system prompts to Register/Login.

---

### TestCase_AI_021 – Proceed to Checkout as Logged In User
1. Login with valid credentials.
2. Add a product to cart.
3. Click "Proceed To Checkout".
4. Verify address details and order review are displayed.

---

### TestCase_AI_022 – Place Order: Register While Checkout
1. Add products to cart.
2. Go to cart and click Proceed To Checkout.
3. Click Register/Login button.
4. Register a new account.
5. Verify "ACCOUNT CREATED!" message.
6. Go back to cart and proceed to checkout.
7. Verify address details and place order.
8. Enter payment details and confirm.
9. Verify success message "Your order has been placed successfully!".

---

### TestCase_AI_023 – Place Order: Register Before Checkout
1. Register a new account first.
2. Login with that account.
3. Add products to cart.
4. Proceed to checkout.
5. Verify address details.
6. Place order with payment details.
7. Verify order success message.

---

### TestCase_AI_024 – Place Order: Login Before Checkout
1. Login with a pre-existing account.
2. Add products to cart.
3. Proceed to checkout.
4. Fill in order comment and place order.
5. Enter payment details.
6. Verify order success message.

---

### TestCase_AI_025 – Download Invoice After Order
1. Place an order successfully.
2. On the success page, click "Download Invoice".
3. Verify the invoice file is downloaded.

---

### TestCase_AI_026 – Verify Address on Checkout Matches Registration
1. Register a new account with a specific address.
2. Add products to cart and proceed to checkout.
3. Verify that the delivery and billing addresses shown match the registration address.

---

### TestCase_AI_027 – Add Product to Cart from Recommended Items
1. Scroll to the bottom of the home page.
2. Find "RECOMMENDED ITEMS" section.
3. Click "Add to Cart" on a recommended product.
4. Click "View Cart".
5. Verify the product appears in the cart.

---

### TestCase_AI_028 – Search Products and Verify Cart After Login
1. Go to Products page.
2. Search for a product and add to cart.
3. Click Signup/Login and log in.
4. Go back to cart page.
5. Verify the previously added products are still in the cart.

---

### TestCase_AI_029 – Register New User with Valid Data
1. Click "Signup / Login".
2. Enter name and a new email.
3. Click Signup.
4. Fill all account details.
5. Click "Create Account".
6. Verify "ACCOUNT CREATED!" is visible.

---

### TestCase_AI_030 – Register with Existing Email
1. Click "Signup / Login".
2. Enter a name and an already registered email.
3. Click Signup.
4. Verify "Email Address already exist!" error is shown.

---

### TestCase_AI_031 – Login with Correct Credentials
1. Click "Signup / Login".
2. Enter correct email and password.
3. Click Login.
4. Verify "Logged in as [username]" is visible.

---

### TestCase_AI_032 – Login with Incorrect Password
1. Click "Signup / Login".
2. Enter valid email but wrong password.
3. Click Login.
4. Verify "Your email or password is incorrect!" message.

---

### TestCase_AI_033 – Login with Unregistered Email
1. Click "Signup / Login".
2. Enter a non-registered email and any password.
3. Click Login.
4. Verify appropriate error message is displayed.

---

### TestCase_AI_034 – Login with Empty Fields
1. Click "Signup / Login".
2. Leave email and password fields blank.
3. Click Login.
4. Verify validation messages appear.

---

### TestCase_AI_035 – Logout Functionality
1. Login with valid credentials.
2. Click Logout from the navigation.
3. Verify the user is redirected to the Login page.

---

### TestCase_AI_036 – Browser Back Button After Logout
1. Login with valid credentials.
2. Click Logout.
3. Press the browser Back button.
4. Verify protected pages are not accessible without login.

---

### TestCase_AI_037 – Delete Account
1. Register a new account.
2. Log in.
3. Click "Delete Account".
4. Verify "ACCOUNT DELETED!" message.

---

### TestCase_AI_038 – Submit Contact Us Form with Valid Data
1. Click "Contact Us".
2. Verify "GET IN TOUCH" is visible.
3. Fill in name, email, subject, and message.
4. Upload a file.
5. Click Submit and accept the popup.
6. Verify success message.

---

### TestCase_AI_039 – Submit Contact Us Form with Empty Fields
1. Navigate to Contact Us page.
2. Leave all fields blank.
3. Click Submit.
4. Verify validation messages for required fields.

---

### TestCase_AI_040 – Submit Contact Us Form with Invalid Email
1. Navigate to Contact Us page.
2. Enter name, invalid email, subject, and message.
3. Click Submit.
4. Verify email format validation message.

---

### TestCase_AI_041 – Verify Home Navigation from Contact Us Page
1. Submit Contact Us form successfully.
2. Click the "Home" button on the Contact Us page.
3. Verify user is redirected to the Home page.

---

### TestCase_AI_042 – Add Product Review
1. Navigate to Products page.
2. Click "View Product" on any item.
3. Scroll to "Write Your Review" section.
4. Enter name, email, and review text.
5. Click Submit.
6. Verify "Thank you for your review." message.


---

# My Thoughts

## What I felt Suitable:
- AI generated a large number of test cases within seconds, significantly reducing the test design effort.
- AI covered all major modules: Home Page, Products, Cart, Checkout, Registration, Login, Logout, and Contact Us.
- AI included both positive and negative test scenarios across all sections.
- AI helped identify edge cases like cart persistence after login, browser back-button post-logout, and subscription form validation.
- AI-generated test cases followed a clean, structured, step-by-step format suitable for both manual and automation use.
- AI was useful for generating an initial coverage baseline before in-depth exploratory testing began.
- AI surfaced validation-related scenarios (empty fields, invalid email formats) that improve overall test coverage.

## What I felt Not Suitable:
- AI generated generic test cases and lacked awareness of actual UI element positions and real popup behaviors observed only during hands-on exploration.
- Some AI test cases were slightly redundant or overlapping in intent (e.g., multiple subscription tests).
- AI had no knowledge of exact field-level validations enforced by the site (specific password rules, optional vs mandatory fields during registration).
- AI missed granular UI-specific scenarios like verifying exact product prices, cart icon badge count, and label verification on checkout.
- Several AI test cases lacked detailed expected results, making them less immediately ready for automation scripting.
- AI did not prioritize test cases based on business risk or functional criticality.
- Boundary value analysis, price-specific checks, and real exploratory edge cases were absent from AI output.
- Human review was still required to eliminate irrelevant scenarios, add missing steps, and align test cases with what the site actually does.


---

# Final Test Cases (AI + Manual Combined)

**Website:** https://automationexercise.com/

**Sections Covered:** Home | Products | Cart | Signup/Login | Contact Us

---

### TC_Final_001 – Verify Home Page Loads and Key Headings Are Visible

1. Open a browser and navigate to https://automationexercise.com.
2. Wait for the page to fully load.
3. Verify the browser page title is correct.
4. Verify the H1 heading 'AutomationExercise' is displayed.
5. Verify the H2 heading 'Full-Fledged practice website for Automation Engineers' is visible.
6. Verify the site logo appears in the header.

**Expected Result:**
The home page loads without errors. The logo, H1, and H2 headings are correctly displayed.

---

### TC_Final_002 – Verify All Navigation Menu Links Are Present and Functional

1. Open https://automationexercise.com.
2. Observe the top navigation bar.
3. Verify the following links are visible: Home, Products, Cart, Signup/Login, Test Cases, API Testing, Video Tutorials, Contact Us.
4. Click each navigation link one at a time and verify the user is taken to the correct page.
5. Use the browser back button to return after each navigation.

**Expected Result:**
All navigation links are present, correctly labeled, and each navigates to its respective page without errors.

---

### TC_Final_003 – Verify Featured Products Are Displayed on Home Page

1. Open https://automationexercise.com.
2. Scroll through the homepage.
3. Verify that product cards are displayed in the featured section.
4. Confirm each product card shows a product image, name, and price (e.g., 'Rs. 500', 'Rs. 1000').
5. Verify that "Add to cart" and "View Product" options are accessible on hover.

**Expected Result:**
Featured products are visible on the home page with correct names, prices, and action buttons.

---

### TC_Final_004 – Verify Product Price Accuracy on Home Page

1. Open https://automationexercise.com.
2. Locate a product with the price 'Rs. 500' on the home page.
3. Verify the price label displays exactly 'Rs. 500'.
4. Locate a product with the price 'Rs. 1000'.
5. Verify the price label displays exactly 'Rs. 1000'.

**Expected Result:**
Product prices displayed on the home page match the expected values without any rounding or formatting errors.

---

### TC_Final_005 – Verify Subscription with Valid Email in Home Page Footer

1. Open https://automationexercise.com.
2. Scroll down to the footer section.
3. Verify the text "SUBSCRIPTION" is present.
4. Enter a valid email address in the subscription input field.
5. Click the arrow/submit button next to the input.

**Expected Result:**
A success message "You have been successfully subscribed!" is displayed.

---

### TC_Final_006 – Verify Subscription with Invalid Email Format in Home Page Footer

1. Open https://automationexercise.com.
2. Scroll down to the subscription form in the footer.
3. Enter an invalid email address (e.g., "user@" or "notanemail").
4. Click the 'Subscribe' button.

**Expected Result:**
An appropriate validation error is shown and the subscription does not proceed.

---

### TC_Final_007 – Verify Subscription with Empty Email in Home Page Footer

1. Open https://automationexercise.com.
2. Scroll down to the subscription form in the footer.
3. Leave the email field completely empty.
4. Click the 'Subscribe' button.

**Expected Result:**
A mandatory field validation message is displayed and the form is not submitted.

---

### TC_Final_008 – Verify Subscription with Special Character Email (Edge Case)

1. Open https://automationexercise.com.
2. Scroll to the subscription form in the footer.
3. Enter an email address containing special characters (e.g., "user+tag@domain.co").
4. Click the 'Subscribe' button.

**Expected Result:**
If the email is technically valid, the subscription succeeds. If it is invalid, an appropriate error message is shown.

---

### TC_Final_009 – Verify Recommended Items Section on Home Page

1. Open https://automationexercise.com.
2. Scroll towards the bottom of the home page.
3. Locate the "RECOMMENDED ITEMS" section.
4. Verify that a list or carousel of recommended products is displayed.
5. Confirm each item shows a product name, image, and an "Add to Cart" button.

**Expected Result:**
The Recommended Items section is visible with functional product cards containing images, names, and cart options.

---

### TC_Final_010 – Verify Scroll Up Using Arrow Button

1. Open https://automationexercise.com.
2. Scroll to the very bottom of the home page.
3. Verify the "SUBSCRIPTION" section is visible at the footer.
4. Locate and click the upward arrow icon at the bottom-right corner.

**Expected Result:**
The page scrolls smoothly back to the top and the H2 heading "Full-Fledged practice website for Automation Engineers" is visible on screen.

---

### TC_Final_011 – Verify Scroll Up Without Using Arrow Button

1. Open https://automationexercise.com.
2. Scroll to the bottom of the home page.
3. Verify the "SUBSCRIPTION" section is visible.
4. Use the mouse wheel or keyboard to manually scroll back to the top.

**Expected Result:**
The page scrolls to the top and the hero heading text is clearly visible.

---

### TC_Final_012 – Verify All Products Page Loads with Complete Listing

1. Open https://automationexercise.com.
2. Click "Products" in the navigation bar.
3. Wait for the page to load.
4. Verify the heading "ALL PRODUCTS" is displayed.
5. Verify a list of products is visible on the page.

**Expected Result:**
The ALL PRODUCTS page loads successfully and displays a complete product listing.

---

### TC_Final_013 – Verify Product Detail Page Shows All Required Information

1. Navigate to the Products page.
2. Click "View Product" on any product in the list.
3. Verify the product detail page opens.
4. Check that all of the following are displayed: product name, category, price, availability, condition, and brand.

**Expected Result:**
All product detail fields are correctly populated and visible on the product page.

---

### TC_Final_014 – Search Product with Valid Keyword

1. Navigate to the Products page.
2. Locate the search input field.
3. Enter a valid product keyword (e.g., "Top", "Dress", "Jeans").
4. Click the Search button.
5. Verify the heading "SEARCHED PRODUCTS" appears.
6. Verify only products matching the keyword are displayed.

**Expected Result:**
The searched products section appears and all displayed products are relevant to the entered keyword.

---

### TC_Final_015 – Search Product with Invalid / Non-Existent Keyword

1. Navigate to the Products page.
2. Enter a random, non-existent keyword in the search box (e.g., "xyzqwerty123").
3. Click the Search button.

**Expected Result:**
No products are returned, or an appropriate empty-state or "no results found" message is shown.

---

### TC_Final_016 – Filter Products by Women → Dress Sub-Category

1. Open https://automationexercise.com.
2. On the left sidebar, click on the "Women" category.
3. Click on the "Dress" sub-category link under Women.
4. Verify the category page opens.

**Expected Result:**
The correct Women → Dress category page is displayed, showing only products from that sub-category.

---

### TC_Final_017 – Filter Products by Men → Jeans Sub-Category

1. Open https://automationexercise.com.
2. On the left sidebar, click on the "Men" category.
3. Click on the "Jeans" sub-category link.
4. Verify the category page opens.

**Expected Result:**
The correct Men → Jeans category page is displayed with relevant products.

---

### TC_Final_018 – View and Verify Products by Brand (Polo)

1. Navigate to the Products page.
2. On the left sidebar, locate the BRANDS section.
3. Click on the "Polo" brand link.
4. Verify the brand-specific product page opens.
5. Confirm products displayed belong to the Polo brand.

**Expected Result:**
The Polo brand page opens and displays only Polo-branded products.

---

### TC_Final_019 – Switch Between Two Different Brands

1. Navigate to the Products page.
2. Click on any brand from the Brands sidebar.
3. Verify the brand products load correctly.
4. Click on a different brand from the sidebar.

**Expected Result:**
The product listing updates immediately to show only the newly selected brand's products, with no residual items from the previous brand.

---

### TC_Final_020 – Add Product Review on Product Detail Page

1. Navigate to the Products page.
2. Click "View Product" on any product.
3. Scroll down to the "Write Your Review" section on the product detail page.
4. Enter a name, email address, and review text.
5. Click the "Submit" button.

**Expected Result:**
A success message "Thank you for your review." is displayed.

---

### TC_Final_021 – Add a Single Product to Cart from Home Page

1. Open https://automationexercise.com.
2. On the home page, locate the product priced at 'Rs. 500'.
3. Hover over the product to reveal action buttons.
4. Click the "Add to cart" button.
5. Verify the "Added!" confirmation modal/popup appears.

**Expected Result:**
The product is added to the cart and the confirmation modal appears with "View Cart" and "Continue Shopping" options.

---

### TC_Final_022 – Verify 'Continue Shopping' Button Keeps User on Current Page

1. Add a product to the cart from the home page or Products page.
2. When the "Added!" modal appears, click the "Continue Shopping" button.

**Expected Result:**
The modal closes and the user remains on the same page they were on, with no unwanted navigation.

---

### TC_Final_023 – Verify 'View Cart' Button Navigates to Cart Page

1. Add a product to the cart.
2. When the "Added!" modal appears, click the "View Cart" button.

**Expected Result:**
The user is navigated to the Cart page, which displays the recently added product.

---

### TC_Final_024 – Add Multiple Products to Cart and Verify Cart Count

1. Open https://automationexercise.com.
2. Hover over product 'Rs. 500' and click "Add to cart".
3. Click "Continue Shopping" to dismiss the modal.
4. Hover over product 'Rs. 400' and click "Add to cart".
5. Click "Continue Shopping".
6. Check the cart icon in the navigation header.

**Expected Result:**
The cart icon/badge count reflects the correct number of distinct items added (e.g., 2 products).

---

### TC_Final_025 – Verify All Cart Details Are Correct After Adding Products

1. Add two or more products to the cart.
2. Click "View Cart" or navigate to the Cart page.
3. Verify all added products are listed.
4. For each item, confirm the product name, unit price, quantity, and total price are correctly shown.

**Expected Result:**
The cart displays all added items with accurate names, prices, quantities, and a correct grand total.

---

### TC_Final_026 – Verify Product Quantity Update in Cart

1. Navigate to the Products page.
2. Click "View Product" on any product.
3. On the product detail page, change the quantity field to 4.
4. Click "Add to cart".
5. Navigate to the Cart page.

**Expected Result:**
The product appears in the cart with the quantity correctly set to 4, and the total price is calculated accordingly.

---

### TC_Final_027 – Remove a Product from Cart

1. Add at least one product to the cart.
2. Navigate to the Cart page.
3. Click the "X" (delete) button next to the product.

**Expected Result:**
The product is removed from the cart. If no other items remain, an empty cart state is displayed.

---

### TC_Final_028 – Add Product to Cart from Recommended Items Section

1. Open https://automationexercise.com.
2. Scroll to the bottom of the home page.
3. Locate the "RECOMMENDED ITEMS" section.
4. Click "Add to Cart" on any recommended product.
5. Click "View Cart".

**Expected Result:**
The selected recommended product appears correctly in the cart.

---

### TC_Final_029 – Verify Subscription in Cart Page Footer

1. Navigate to the Cart page via the header.
2. Scroll to the footer of the cart page.
3. Verify the "SUBSCRIPTION" section is present.
4. Enter a valid email address and click the subscribe button.

**Expected Result:**
A success message "You have been successfully subscribed!" is displayed.

---

### TC_Final_030 – Proceed to Checkout Without Being Logged In

1. Open https://automationexercise.com.
2. Add a product to the cart without logging in.
3. Navigate to the Cart page.
4. Click "Proceed To Checkout".

**Expected Result:**
The system displays a prompt asking the user to Register or Login before the checkout can proceed.

---

### TC_Final_031 – Proceed to Checkout as a Logged In User

1. Login with a valid registered account.
2. Add a product to the cart.
3. Navigate to the Cart page.
4. Click "Proceed To Checkout".

**Expected Result:**
The checkout page loads and displays the user's saved delivery and billing address details along with a review of the order.

---

### TC_Final_032 – Verify Address on Checkout Page Matches Registration Details

1. Register a new user with a specific, complete address.
2. Add a product to the cart.
3. Proceed to the Checkout page.
4. Compare the delivery address and billing address shown on the checkout page against the address entered during registration.

**Expected Result:**
Both the delivery and billing addresses on the checkout page exactly match the address provided at the time of registration.

---

### TC_Final_033 – Place Order: Register While at Checkout

1. Add products to the cart without logging in.
2. Navigate to the Cart page and click "Proceed To Checkout".
3. Click the "Register / Login" button on the checkout prompt.
4. Complete the registration form with all valid details and click "Create Account".
5. Verify "ACCOUNT CREATED!" is shown and click Continue.
6. Verify "Logged in as [username]" appears in the header.
7. Navigate back to the Cart and click "Proceed To Checkout".
8. Verify address details and the order summary on the checkout page.
9. Enter a comment in the order message box and click "Place Order".
10. Enter payment details: Name on Card, Card Number, CVC, and Expiration Date.
11. Click "Pay and Confirm Order".

**Expected Result:**
The success message "Your order has been placed successfully!" is displayed.

---

### TC_Final_034 – Place Order: Login Before Checkout

1. Login with a valid pre-existing account.
2. Add products to the cart.
3. Navigate to the Cart page.
4. Click "Proceed To Checkout".
5. Verify address details and order review.
6. Enter an order comment and click "Place Order".
7. Enter valid payment details and click "Pay and Confirm Order".

**Expected Result:**
The order is placed and the confirmation message "Your order has been placed successfully!" is displayed.

---

### TC_Final_035 – Download Invoice After Order Placement

1. Complete an order placement flow successfully (login → add to cart → checkout → confirm payment).
2. On the order success confirmation page, click the "Download Invoice" button.

**Expected Result:**
An invoice PDF file is downloaded to the user's device successfully.

---

### TC_Final_036 – Verify Cart Persists After Logging In (Search + Add + Login)

1. Open the Products page without logging in.
2. Search for a product using a keyword.
3. Add one of the search result products to the cart.
4. Navigate to Signup/Login and log in with valid credentials.
5. Navigate to the Cart page.

**Expected Result:**
The product added before login is still present in the cart after the user logs in.

---

### TC_Final_037 – Register New User with Valid and Complete Details

1. Open https://automationexercise.com.
2. Click "Signup / Login" in the navigation.
3. Verify the "New User Signup!" section is visible.
4. Enter a unique name and a brand-new email address not used before.
5. Click "Signup".
6. Verify "ENTER ACCOUNT INFORMATION" is displayed.
7. Fill in: Title, Name, Email, Password, Day/Month/Year of Birth.
8. Check "Sign up for our newsletter!" and "Receive special offers from our partners!".
9. Fill in: First Name, Last Name, Company, Address, Address2, Country, State, City, Zipcode, and Mobile Number.
10. Click "Create Account".
11. Verify "ACCOUNT CREATED!" is shown.
12. Click "Continue".
13. Verify "Logged in as [username]" is visible in the navigation header.

**Expected Result:**
A new account is created successfully and the user is automatically logged in.

---

### TC_Final_038 – Register with an Already Registered Email

1. Open https://automationexercise.com.
2. Click "Signup / Login".
3. Verify "New User Signup!" is visible.
4. Enter a valid name and an email address already associated with an existing account.
5. Click "Signup".

**Expected Result:**
The error message "Email Address already exist!" is displayed and no new account is created.

---

### TC_Final_039 – Login with Correct Email and Password

1. Open https://automationexercise.com.
2. Click "Signup / Login".
3. Locate the "Login to your account" section.
4. Enter a valid registered email address and the correct matching password.
5. Click the "Login" button.

**Expected Result:**
The user is logged in successfully and "Logged in as [username]" is visible in the navigation header.

---

### TC_Final_040 – Login with Incorrect Password

1. Open https://automationexercise.com.
2. Click "Signup / Login".
3. Enter a valid registered email but type an incorrect password.
4. Click "Login".

**Expected Result:**
The error message "Your email or password is incorrect!" is shown and the user is not logged in.

---

### TC_Final_041 – Login with Unregistered / Non-Existent Email

1. Open https://automationexercise.com.
2. Click "Signup / Login".
3. Enter an email address that has never been registered on the site.
4. Enter any password.
5. Click "Login".

**Expected Result:**
An appropriate error message is displayed indicating the credentials are not recognized.

---

### TC_Final_042 – Login with Empty Email and Password Fields

1. Open https://automationexercise.com.
2. Click "Signup / Login".
3. Leave both the email and password fields completely empty.
4. Click the "Login" button.

**Expected Result:**
Mandatory field validation messages appear for both the email and password fields; no login attempt is made.

---

### TC_Final_043 – Logout Functionality

1. Open https://automationexercise.com.
2. Login with valid credentials.
3. Verify "Logged in as [username]" is displayed in the header.
4. Click the "Logout" button in the navigation bar.

**Expected Result:**
The user is logged out and redirected to the Login page.

---

### TC_Final_044 – Browser Back Button Does Not Grant Access After Logout

1. Login with valid credentials.
2. Perform an action that takes you to a protected page (e.g., My Account or Cart).
3. Click "Logout".
4. After being redirected to the Login page, click the browser's Back button.

**Expected Result:**
The user is not able to access the previously visited protected page and remains on or is redirected back to the Login page.

---

### TC_Final_045 – Delete Account After Login

1. Open https://automationexercise.com.
2. Register a new user or log in to an existing account.
3. Verify "Logged in as [username]" in the header.
4. Click "Delete Account" from the navigation.

**Expected Result:**
The message "ACCOUNT DELETED!" is displayed and the account is permanently removed. The user is redirected away from authenticated pages.

---

### TC_Final_046 – Submit Contact Us Form with All Valid Data

1. Open https://automationexercise.com.
2. Click "Contact Us" in the navigation bar.
3. Verify the "GET IN TOUCH" heading is visible on the page.
4. Enter a valid name in the Name field.
5. Enter a valid email address in the Email field.
6. Enter a subject in the Subject field.
7. Enter a message in the Message text area.
8. Upload any file using the file upload input.
9. Click the "Submit" button.
10. On the browser confirmation dialog/popup, click OK.

**Expected Result:**
The success message "Success! Your details have been submitted successfully." is displayed on the page.

---

### TC_Final_047 – Submit Contact Us Form with All Fields Empty

1. Open https://automationexercise.com.
2. Click "Contact Us" in the navigation.
3. Leave all form fields (Name, Email, Subject, Message) completely empty.
4. Click the "Submit" button.

**Expected Result:**
Validation error messages appear for all required fields and the form is not submitted.

---

### TC_Final_048 – Submit Contact Us Form with Invalid Email Format

1. Open https://automationexercise.com.
2. Navigate to the Contact Us page.
3. Enter a valid name in the Name field.
4. Enter an incorrectly formatted email (e.g., "user@" or "user.com") in the Email field.
5. Enter a valid subject and message.
6. Click Submit.

**Expected Result:**
An email format validation error is displayed and the form is not submitted.

---

### TC_Final_049 – Verify 'Home' Button on Contact Us Page Navigates to Home

1. Open https://automationexercise.com.
2. Navigate to the Contact Us page.
3. Fill in all required fields and submit the form successfully.
4. After the success message appears, click the "Home" button visible on the page.

**Expected Result:**
The user is redirected back to the home page successfully.


---

### TC_Final_050 – Complete End-to-End User Journey: Register → Browse → Search → Cart → Order → Delete Account

1. Open https://automationexercise.com.
2. Click "Signup / Login" and register a new user with all valid details (name, email, password, full address).
3. Verify "ACCOUNT CREATED!" is shown and click Continue.
4. Verify "Logged in as [username]" is visible in the header.
5. Click "Products" in the navigation.
6. Verify the "ALL PRODUCTS" page loads.
7. Enter a valid keyword in the search bar (e.g., "Top") and click Search.
8. Verify "SEARCHED PRODUCTS" section appears.
9. Click "View Product" on one of the search results.
10. Verify the product detail page shows name, price, category, availability, condition, and brand.
11. Set quantity to 2 and click "Add to cart".
12. Click "Continue Shopping".
13. Navigate to the Cart page.
14. Verify the product appears with quantity 2 and correct price.
15. Click "Proceed To Checkout".
16. Verify address details on the checkout page match the registration address.
17. Enter a comment and click "Place Order".
18. Enter valid payment details: Name on Card, Card Number, CVC, Expiration Date.
19. Click "Pay and Confirm Order".
20. Verify the success message "Your order has been placed successfully!".
21. Click "Download Invoice" and verify the file is downloaded.
22. Click "Continue".
23. Click "Delete Account" from the navigation.
24. Verify "ACCOUNT DELETED!" is displayed.

**Expected Result:**
The entire user journey — from registration through product discovery, search, cart management, order placement, invoice download, and account deletion — completes successfully without any functional errors or broken flows.


