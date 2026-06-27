QA Manual Test Cases
Project: DemoBlaze Testing Application: https://www.demoblaze.com/  
Tester: Kiran Sharma

Human Thinking Test Cases—--------------------------------------

TC 001: TestCase_015:- Verify that the user is able to create an account on successful signup.
Go to https://www.demoblaze.com/ 
Click on the “Signup” option in the top menu section.
Enter required input in the username and password fields.
Click on the Signup page.
On successful signup, a message will be displayed as “Sign up successful” to the users.

TC 002:  Verify the error message on invalid/ blank input  through signup option.
Go to https://www.demoblaze.com/ 
Click on the “Signup” option in the top menu section.
Click on the Signup button without entering any input for either or both of the input fields.
The user should be displayed an error message.

TC 003: Verify the error message for an already existing account.
Go to https://www.demoblaze.com/ 
Click on the “Signup” option in the top menu section.
Click on the Signup button after entering credentials for a previously existing account.
The user should be displayed a message “This user already exists.”.

TC 004:  Verify that popups can be closed through “X” button
Go to https://www.demoblaze.com/ 
Click on the “Contact” option in the top menu section.
Click on the “x” button displayed on the top right edge of the popup.
The current popup window displaying should be closed for the user.
Repeat the same actions for “About Us”, “Login” and “Signup” options.

TC 005: Verify the error message on unsuccessful login for an already existing account
Go to https://www.demoblaze.com/ 
Click on the “Login” option in the top menu section.
Enter credentials in the username and password fields for an account which is not created.
An error message should be displayed stating “User does not exist” .

TC 006: Verify the status message on successful login
Go to https://www.demoblaze.com/ 
Click on the “Login” option in the top menu section.
Enter valid credentials in the username and password fields and click on the “Log in” button.
The user will be redirected to the homepage again but this time the login option will update to logout and signup button to “Welcome XYZ”.

TC 007: Verify that slideshow is scrollable on clicking the given scroll bars
Go to https://www.demoblaze.com/ .
On the landing page, the slideshow gets displayed at the top of the page.
Click on the right scroll bar.

TC 008: Verify that the slide moves towards its right content.
Go to https://www.demoblaze.com/ .
On the landing page, the slideshow gets displayed at the top of the page.
Click on the right scroll bar.

TC 009: Similarly, click on the left scroll bar. Verify that the slide moves towards its left content.
Go to https://www.demoblaze.com/ .
On the landing page, the slideshow gets displayed at the top of the page.
Click on the Left scroll bar.

TC 010: Verify that all top menu options are responsive
Go to https://www.demoblaze.com/ 
Hover over the top menu options displayed on the top right corner of the landing page.
The font color of the options should be changing
Clicking on any of the top menu options.
The user should be redirected to the required page or popup.

TC 011: Verify that the required popup is displayed on clicking the “Contact” option.
Go to https://www.demoblaze.com/ 
Click on the “Contact” option in the top menu section.
A pop should get displayed with a header “New Message” and input fields “Contact Email”, “Contact Name” and “Message”.

TC 012: Verify that a notification gets displayed when user tries to sent message without any input
Go to https://www.demoblaze.com/ 
Click on the “Contact” option in the top menu section.
Click on “sent message” with or without entering any input.
A notification “Thanks for the message!!”  should be displayed to users.

TC 013: Verify that the required popup is displayed on clicking the “About Us” option.
Go to https://www.demoblaze.com/ 
Click on the “About Us” option in the top menu section.
A popup should be displayed with a redirection to a video displayed in it.

TC 014: Verify that a required page is displayed on clicking the “Cart” option.
Go to https://www.demoblaze.com/ 
Click on the “Cart” option in the top menu section.
Users should be redirected to the cart page with the list of products added (if any).

TC 015: Verify that a required popup is displayed on clicking the “Login” option.
Go to https://www.demoblaze.com/ 
Click on the “Login” option in the top menu section.
A popup should be displayed with username and password input fields.

TC 016: Verify that a required popup is displayed on clicking the “Signup” option.
Go to https://www.demoblaze.com/ 
Click on the “Signup” option in the top menu section.
A popup should be displayed with username and password input fields.

TC 017:  Verify that user is able to successfully add a product to the cart
Go to https://www.demoblaze.com/ 
Click on any of the products display d on the product listing section.
Click on the “Add to cart” button displayed in the product details page.
A success message gets displayed to the user as “Product added”.
Now go to the cart page through the cart option in the top menu section.
The added product should be displayed to the user.

TC 018: Verify the details displayed in the cart page
Go to https://www.demoblaze.com/ 
Click on any of the products displayed on the product listing section.
Click on the “Add to cart” button displayed in the product details page.
A success message gets displayed to the user as “Product added”.
Repeat the above steps multiple times to add the same or different product.
Now go to the cart page through the cart option in the top menu section.
The user should be able to see all the added products, their individual price and the total price of the products in the cart.

TC 019:  Verify the delete option in the cart
Go to https://www.demoblaze.com/ 
Click on any of the products displayed on the product listing section.
Add the products in the cart from the product details page.
Repeat the above steps 2-3 times for different products.
Now go to the cart through the “Cart” icon in the top menu section.
Check whether the user is able to see a delete option for every product added in the cart.
A “delete” option will be displayed to the user for each product.

TC 020: Verify the successful order completion flow
Go to https://www.demoblaze.com/ 
Add a single or multiple products into the cart by selecting the products from their individual product details page.
Now go to the cart through the “Cart” icon in the top menu section.
Click on the “Place Order “ button.
Fill at least the details for mandatory fields of name and credit card number in the popup displayed
Click on the “Purchase” button.
A thank you notification will appear to the user confirming the order purchase with the following details : id, amount,card number, name,date.

TC 021:  Verify the mandatory fields in the payment popup
Go to https://www.demoblaze.com/ 
Add a single or multiple products into the cart by selecting the products from their individual product details page.
Now go to the cart through the “Cart” icon in the top menu section.
Click on the “Place Order “ button.
A popup will appear to fill up details for name, country, city, credit card, month and year.
Click on the purchase button without entering the mandatory fields of name and credit card number.
An error notification will be displayed to the user to fill the mandatory fields.

TC 022: Verify the mandatory fields in the payment popup
Go to https://www.demoblaze.com/ 
Add a single or multiple products into the cart by selecting the products from their individual product details page.
Now go to the cart through the “Cart” ic

TC 022: Verify that all details displayed in the footer are correct including copyright details. 
Go to https://www.demoblaze.com/ 
Go to the footer section and check. 


Role- Act as a Senior QA Engineer with expertise in Manual Testing, Functional Testing, Regression Testing, and Web Application Testing.

Task-Generate comprehensive manual test cases for the AutomationExercise web application. Cover all major functionalities including Home Page, Products Listing, Product Search, Product Filtering, Cart Management, Checkout Flow, User Registration, Login, Logout, Account Management, and Contact Us Form.

Context- The application under test is: https://www.demoblaze.com/AutomationExercise is a full-fledged e-commerce practice website where users can: Register a new account with full address details, Login with registered credentials, Browse and explore the home page, View all products and product details, Search and filter products by category and brand, Add products to a shopping cart, Manage cart items (increase quantity, remove items), Proceed through the checkout flow with order placement, Process an order and download the invoice, Logout from the application, Delete a registered account, Submit the Contact Us form, Subscribe to the newsletter via the footer.
The objective is to validate the complete end-to-end user journey and identify possible functional, validation, and security-related issues across the sections: Home, Products, Cart, About Us, Signup/Login, and Contact Us.

Constraints-
Include both Positive and Negative test scenarios.
Include Validation and Error Handling scenarios.
Include Session Management and Security-related scenarios.
Consider real-world user behavior and edge cases.
Avoid duplicate test cases.
Write test cases in a clear step-by-step format.
Ensure test cases are suitable for future automation.
Cover mandatory field validations wherever applicable.
Include business-critical scenarios such as cart persistence and unauthorized access checks.
Do NOT include test cases for the Test Cases or API Testing sections.

Output Format-
Generate test cases using the following format:
TestCase_ID: TC_XXX - Test Scenario
Test Steps:
Step 1
Step 2
Step 3


Final Test Cases (AI + Manual Combined)
Website: https://www.demoblaze.com/  
Sections Covered: Home | Products | About Us | Cart | Signup/Login | Contact Us

Home Page
TestCase_ID: TC_001 - Verify Home Page Loads Successfully
Test Steps:
Step 1: Open the browser and navigate website URL https://www.demoblaze.com/ .
Step 2: Wait until the page is fully loaded.
Step 3: Verify that the Home page is displayed with logo, navigation menu, product sections, category section, brand section, and footer.
Expected Result: Home page should load successfully without broken layout, blank screen, or console-visible functional error.

TestCase_ID: TC_002 - Verify Header Navigation Links
Test Steps:
Step 1: Open the Home page.
Step 2: Click Home, Products, Cart, Signup/Login, Contact Us one by one.
Step 3: Verify that each menu redirects to the correct page.
Expected Result: Each navigation link should open the correct section/page.

TestCase_ID: TC_003 - Verify Home Page Product Visibility
Test Steps:
Step 1: Open the Home page.
Step 2: Scroll to the Featured Items section.
Step 3: Verify product image, product name, price, Add to Cart button, and View Product link.
Expected Result: Product cards should display correct product information and actionable buttons.

TestCase_ID: TC_004 - Verify Product Added to Cart from Home Page
Test Steps:
Step 1: Open the Home page.
Step 2: Click Add to Cart for any product.
Step 3: Verify the confirmation popup.
Step 4: Click View Cart.
Expected Result: Selected product should be added to cart and displayed correctly on the cart page.

TestCase_ID: TC_005 - Verify Continue Shopping from Add to Cart Popup
Test Steps:
Step 1: Open the Home page.
Step 2: Click Add to Cart for any product.
Step 3: Click Continue Shopping on the popup.
Step 4: Verify user remains on the shopping page.
Expected Result: Popup should close and user should be able to continue browsing products.

TestCase_ID: TC_006 - Verify Footer Newsletter Subscription with Valid Email
Test Steps:
Step 1: Open the Home page.
Step 2: Scroll to the footer subscription section.
Step 3: Enter a valid email address.
Step 4: Click the Subscribe button.
Expected Result: System should display a successful subscription message.

TestCase_ID: TC_007 - Verify Newsletter Subscription with Blank Email
Test Steps:
Step 1: Open the Home page.
Step 2: Scroll to the footer subscription section.
Step 3: Leave the email field blank.
Step 4: Click the Subscribe button.
Expected Result: System should not submit blank email and should show proper validation message.

TestCase_ID: TC_008 - Verify Newsletter Subscription with Invalid Email Format
Test Steps:
Step 1: Open the Home page.
Step 2: Enter invalid email format such as testmail.com.
Step 3: Click the Subscribe button.
Expected Result: System should display validation error for invalid email format.
Products Listing and Product Details

TestCase_ID: TC_009 - Verify Products Page Loads Successfully
Test Steps:
Step 1: Open the Home page.
Step 2: Click Products from the header menu.
Step 3: Verify product listing page is displayed.
Expected Result: Products page should display product list with product name, price, image, Add to Cart, and View Product options.

TestCase_ID: TC_010 - Verify Product Detail Page
Test Steps:
Step 1: Open the Products page.
Step 2: Click View Product for any product.
Step 3: Verify product detail page content.
Expected Result: Product detail page should display product name, category, price, availability, condition, brand, quantity field, and Add to Cart button.

TestCase_ID: TC_011 - Verify Add Product to Cart from Product Detail Page
Test Steps:
Step 1: Open any product detail page.
Step 2: Enter quantity as 1.
Step 3: Click Add to Cart.
Step 4: Click View Cart.
Expected Result: Product should be added to cart with correct name, price, quantity, and total.

TestCase_ID: TC_012 - Verify Product Quantity Update Before Adding to Cart
Test Steps:
Step 1: Open any product detail page.
Step 2: Enter quantity as 3.
Step 3: Click Add to Cart.
Step 4: Open the cart page.
Expected Result: Cart should display the product quantity as 3 and total price should be calculated correctly.

TestCase_ID: TC_013 - Verify Product Quantity Cannot Be Zero
Test Steps:
Step 1: Open any product detail page.
Step 2: Enter quantity as 0.
Step 3: Click Add to Cart.
Expected Result: System should not allow zero quantity or should show validation message.

TestCase_ID: TC_014 - Verify Product Quantity Cannot Be Negative
Test Steps:
Step 1: Open any product detail page.
Step 2: Enter quantity as -1.
Step 3: Click Add to Cart.
Expected Result: System should not allow negative quantity and should show validation message.

TestCase_ID: TC_015 - Verify Product Quantity Cannot Accept Alphabetic Value
Test Steps:
Step 1: Open any product detail page.
Step 2: Enter quantity as abc.
Step 3: Click Add to Cart.
Expected Result: Quantity field should not accept alphabetic value or should show proper validation message.

Product Search and Filtering
TestCase_ID: TC_016 - Verify Search Product with Valid Product Name
Test Steps:
Step 1: Open the Products page.
Step 2: Enter a valid product name in the search field.
Step 3: Click the Search button.
Expected Result: Matching product should be displayed in the search result.

TestCase_ID: TC_017 - Verify Search Product with Partial Product Name
Test Steps:
Step 1: Open the Products page.
Step 2: Enter partial product keyword.
Step 3: Click the Search button.
Expected Result: Products matching the keyword should be displayed.

TestCase_ID: TC_018 - Verify Search Product with Invalid Product Name
Test Steps:
Step 1: Open the Products page.
Step 2: Enter a non-existing product name.
Step 3: Click the Search button.
Expected Result: No matching product should be displayed or proper no-result behavior should be shown.

TestCase_ID: TC_019 - Verify Search with Blank Input
Test Steps:
Step 1: Open the Products page.
Step 2: Leave the search field blank.
Step 3: Click the Search button.
Expected Result: System should either display validation message or keep the product listing unchanged.

TestCase_ID: TC_020 - Verify Search Field Against Script Injection
Test Steps:
Step 1: Open the Products page.
Step 2: Enter <script>alert(1)</script> in the search field.
Step 3: Click the Search button.
Expected Result: Script should not execute. Input should be treated as plain text or rejected safely.

TestCase_ID: TC_021 - Verify Product Filter by Category
Test Steps:
Step 1: Open the Home page or Products page.
Step 2: Select any category such as Women, Men, or Kids.
Step 3: Select a sub-category.
Expected Result: Products related to the selected category should be displayed.

TestCase_ID: TC_022 - Verify Product Filter by Brand
Test Steps:
Step 1: Open the Home page or Products page.
Step 2: Select any brand from the Brands section.
Step 3: Verify filtered product list.
Expected Result: Products related to the selected brand should be displayed.

TestCase_ID: TC_023 - Verify Category and Brand Filter Result Consistency
Test Steps:
Step 1: Open the Products page.
Step 2: Apply a category filter.
Step 3: Apply a brand filter.
Step 4: Verify displayed products.
Expected Result: Displayed products should match selected filter criteria and should not show unrelated products.

User Registration

TestCase_ID: TC_024 - Verify New User Registration with Valid Details
Test Steps:
Step 1: Click Signup/Login from the header menu.
Step 2: Enter valid name and unique email in New User Signup section.
Step 3: Click Signup.
Step 4: Fill all mandatory account information and address details.
Step 5: Click Create Account.
Expected Result: Account should be created successfully and success message should be displayed.

TestCase_ID: TC_025 - Verify Registration with Existing Email
Test Steps:
Step 1: Open Signup/Login page.
Step 2: Enter name and already registered email address.
Step 3: Click Signup.
Expected Result: System should display error message that email already exists.

TestCase_ID: TC_026 - Verify Registration with Blank Name
Test Steps:
Step 1: Open Signup/Login page.
Step 2: Leave name field blank.
Step 3: Enter valid email.
Step 4: Click Signup.
Expected Result: System should not allow registration and should show name field validation.

TestCase_ID: TC_027 - Verify Registration with Blank Email
Test Steps:
Step 1: Open Signup/Login page.
Step 2: Enter valid name.
Step 3: Leave email field blank.
Step 4: Click Signup.
Expected Result: System should not allow registration and should show email field validation.

TestCase_ID: TC_028 - Verify Registration with Invalid Email Format
Test Steps:
Step 1: Open Signup/Login page.
Step 2: Enter valid name.
Step 3: Enter invalid email format.
Step 4: Click Signup.
Expected Result: System should display invalid email validation message.

TestCase_ID: TC_029 - Verify Mandatory Fields on Account Information Page
Test Steps:
Step 1: Start signup with valid name and email.
Step 2: On account information page, leave mandatory fields blank.
Step 3: Click Create Account.
Expected Result: System should highlight all mandatory fields and should not create account.

TestCase_ID: TC_030 - Verify Password Field Validation During Registration
Test Steps:
Step 1: Start signup with valid name and email.
Step 2: Enter weak password or leave password blank.
Step 3: Fill remaining mandatory fields.
Step 4: Click Create Account.
Expected Result: System should validate password field and should not allow blank password.

TestCase_ID: TC_031 - Verify Address Details Are Saved Correctly During Registration
Test Steps:
Step 1: Register a new user with full address details.
Step 2: Login with the same user.
Step 3: Add product to cart and proceed to checkout.
Step 4: Verify delivery and billing address.
Expected Result: Address details should match the details entered during registration.

Login and Logout

TestCase_ID: TC_032 - Verify Login with Valid Credentials
Test Steps:
Step 1: Open Signup/Login page.
Step 2: Enter registered email and valid password.
Step 3: Click Login.
Expected Result: User should be logged in successfully and username should be displayed.

TestCase_ID: TC_033 - Verify Login with Invalid Password
Test Steps:
Step 1: Open Signup/Login page.
Step 2: Enter registered email and wrong password.
Step 3: Click Login.
Expected Result: System should display invalid login error and user should not be logged in.

TestCase_ID: TC_034 - Verify Login with Unregistered Email
Test Steps:
Step 1: Open Signup/Login page.
Step 2: Enter unregistered email and any password.
Step 3: Click Login.
Expected Result: System should display error message and should not allow login.

TestCase_ID: TC_035 - Verify Login with Blank Email and Password
Test Steps:
Step 1: Open Signup/Login page.
Step 2: Leave email and password fields blank.
Step 3: Click Login.
Expected Result: System should display mandatory field validation.

TestCase_ID: TC_036 - Verify Login with Invalid Email Format
Test Steps:
Step 1: Open Signup/Login page.
Step 2: Enter invalid email format.
Step 3: Enter password.
Step 4: Click Login.
Expected Result: System should display email format validation.

TestCase_ID: TC_037 - Verify Login Fields Against SQL Injection
Test Steps:
Step 1: Open Signup/Login page.
Step 2: Enter ' OR '1'='1 in email or password field.
Step 3: Click Login.
Expected Result: Login should fail and system should not expose database or technical error.

TestCase_ID: TC_038 - Verify Logout Functionality
Test Steps:
Step 1: Login with valid credentials.
Step 2: Click Logout.
Step 3: Verify user is redirected to Signup/Login page.
Expected Result: User should be logged out successfully and protected user session should end.

TestCase_ID: TC_039 - Verify Browser Back Button After Logout
Test Steps:
Step 1: Login with valid credentials.
Step 2: Click Logout.
Step 3: Click browser Back button.
Expected Result: User should not access logged-in session page after logout.

Cart Management

TestCase_ID: TC_040 - Verify Add Single Product to Cart
Test Steps:
Step 1: Open Products page.
Step 2: Click Add to Cart for one product.
Step 3: Click View Cart.
Expected Result: Selected product should be displayed in cart with correct product name, price, quantity, and total.

TestCase_ID: TC_041 - Verify Add Multiple Products to Cart
Test Steps:
Step 1: Open Products page.
Step 2: Add two or more different products to cart.
Step 3: Open the cart page.
Expected Result: All selected products should be displayed separately in cart.

TestCase_ID: TC_042 - Verify Cart Total Calculation
Test Steps:
Step 1: Add multiple products to cart.
Step 2: Open cart page.
Step 3: Verify price, quantity, and total amount for each product.
Expected Result: Product total should be calculated correctly based on price and quantity.

TestCase_ID: TC_043 - Verify Remove Product from Cart
Test Steps:
Step 1: Add any product to cart.
Step 2: Open cart page.
Step 3: Click remove/delete icon for the product.
Expected Result: Product should be removed from the cart successfully.

TestCase_ID: TC_044 - Verify Empty Cart Behavior
Test Steps:
Step 1: Open cart page without adding any product.
Step 2: Verify cart content.
Expected Result: Cart should show empty state or no product should be listed.

TestCase_ID: TC_045 - Verify Cart Persistence Before Login
Test Steps:
Step 1: Add product to cart as guest user.
Step 2: Open cart page and verify product.
Step 3: Navigate to another page and come back to cart.
Expected Result: Cart item should remain available during the same browser session.

TestCase_ID: TC_046 - Verify Cart Persistence After Login
Test Steps:
Step 1: Add product to cart as guest user.
Step 2: Login with valid credentials.
Step 3: Open cart page.
Expected Result: Product added before login should remain available in cart.

TestCase_ID: TC_047 - Verify Duplicate Product Add Behavior
Test Steps:
Step 1: Add the same product to cart twice.
Step 2: Open cart page.
Expected Result: System should either increase quantity or show the product correctly without duplicate calculation issue.

Checkout Flow and Order Placement

TestCase_ID: TC_048 - Verify Checkout Redirect for Guest User
Test Steps:
Step 1: Add product to cart as guest user.
Step 2: Open cart page.
Step 3: Click Proceed To Checkout.
Expected Result: System should ask user to register/login before checkout.

TestCase_ID: TC_049 - Verify Checkout for Logged-in User
Test Steps:
Step 1: Login with valid credentials.
Step 2: Add product to cart.
Step 3: Open cart page.
Step 4: Click Proceed To Checkout.
Expected Result: Checkout page should open with address details and order review section.

TestCase_ID: TC_050 - Verify Delivery and Billing Address on Checkout Page
Test Steps:
Step 1: Login with registered user.
Step 2: Add product to cart.
Step 3: Proceed to checkout.
Step 4: Verify delivery and billing address.
Expected Result: Delivery and billing address should match user registration details.

TestCase_ID: TC_051 - Verify Order Review Details on Checkout Page
Test Steps:
Step 1: Login with valid user.
Step 2: Add one or more products to cart.
Step 3: Proceed to checkout.
Step 4: Verify product name, quantity, price, and total.
Expected Result: Order review should display correct cart details.

TestCase_ID: TC_052 - Verify Place Order with Comment
Test Steps:
Step 1: Proceed to checkout as logged-in user.
Step 2: Enter order comment in comment text area.
Step 3: Click Place Order.
Expected Result: User should be redirected to payment page.

TestCase_ID: TC_053 - Verify Place Order Without Comment
Test Steps:
Step 1: Proceed to checkout as logged-in user.
Step 2: Leave comment field blank.
Step 3: Click Place Order.
Expected Result: System should allow order placement if comment is optional.

TestCase_ID: TC_054 - Verify Payment with Valid Card Details
Test Steps:
Step 1: Proceed to payment page.
Step 2: Enter valid name on card, card number, CVC, expiry month, and expiry year.
Step 3: Click Pay and Confirm Order.
Expected Result: Order should be placed successfully and success message should be displayed.

TestCase_ID: TC_055 - Verify Payment with Blank Mandatory Fields
Test Steps:
Step 1: Proceed to payment page.
Step 2: Leave all payment fields blank.
Step 3: Click Pay and Confirm Order.
Expected Result: System should not process payment and should show mandatory field validation.

TestCase_ID: TC_056 - Verify Payment with Invalid Card Number
Test Steps:
Step 1: Proceed to payment page.
Step 2: Enter invalid card number.
Step 3: Fill other fields with valid data.
Step 4: Click Pay and Confirm Order.
Expected Result: System should reject invalid card number or show validation error.

TestCase_ID: TC_057 - Verify Payment with Invalid CVC
Test Steps:
Step 1: Proceed to payment page.
Step 2: Enter alphabetic or invalid CVC.
Step 3: Fill remaining payment fields.
Step 4: Click Pay and Confirm Order.
Expected Result: System should validate CVC and should not accept invalid value.

TestCase_ID: TC_058 - Verify Payment with Expired Card Date
Test Steps:
Step 1: Proceed to payment page.
Step 2: Enter expired month and year.
Step 3: Fill remaining payment fields.
Step 4: Click Pay and Confirm Order.
Expected Result: System should reject expired card details.

TestCase_ID: TC_059 - Verify Invoice Download After Successful Order
Test Steps:
Step 1: Complete order successfully.
Step 2: Click Download Invoice.
Step 3: Verify downloaded invoice file.
Expected Result: Invoice should download successfully and should contain correct order details.

TestCase_ID: TC_060 - Verify Continue Button After Order Success
Test Steps:
Step 1: Complete order successfully.
Step 2: Click Continue button.
Expected Result: User should be redirected to expected page without error.

Account Management

TestCase_ID: TC_061 - Verify Delete Account Functionality
Test Steps:
Step 1: Login with valid credentials.
Step 2: Click Delete Account.
Step 3: Confirm account deletion if confirmation appears.
Expected Result: Account should be deleted successfully and confirmation message should be displayed.

TestCase_ID: TC_062 - Verify Login After Account Deletion
Test Steps:
Step 1: Delete an existing account.
Step 2: Go to Signup/Login page.
Step 3: Try to login with deleted account credentials.
Expected Result: Login should fail because account no longer exists.

TestCase_ID: TC_063 - Verify Re-registration with Deleted Account Email
Test Steps:
Step 1: Delete an existing account.
Step 2: Start new registration using the same email.
Step 3: Complete registration.
Expected Result: System should allow re-registration if deleted email is released, or display proper business validation message.

Contact Us Form

TestCase_ID: TC_064 - Verify Contact Us Form with Valid Details
Test Steps:
Step 1: Click Contact Us from the header menu.
Step 2: Enter valid name, email, subject, and message.
Step 3: Upload a valid file if required.
Step 4: Click Submit.
Expected Result: Contact form should be submitted successfully and success message should be displayed.

TestCase_ID: TC_065 - Verify Contact Us Form with Blank Mandatory Fields
Test Steps:
Step 1: Open Contact Us page.
Step 2: Leave name, email, subject, and message fields blank.
Step 3: Click Submit.
Expected Result: System should show mandatory field validation and should not submit the form.

TestCase_ID: TC_066 - Verify Contact Us Form with Invalid Email Format
Test Steps:
Step 1: Open Contact Us page.
Step 2: Enter valid name, subject, and message.
Step 3: Enter invalid email format.
Step 4: Click Submit.
Expected Result: System should display email validation error.

TestCase_ID: TC_067 - Verify Contact Us Form File Upload
Test Steps:
Step 1: Open Contact Us page.
Step 2: Fill valid form details.
Step 3: Upload a valid file.
Step 4: Click Submit.
Expected Result: Form should submit successfully with uploaded file.

TestCase_ID: TC_068 - Verify Contact Us Form with Unsupported File Type
Test Steps:
Step 1: Open Contact Us page.
Step 2: Fill valid contact form details.
Step 3: Upload unsupported file type such as .exe.
Step 4: Click Submit.
Expected Result: System should reject unsupported file type or show validation message.

TestCase_ID: TC_069 - Verify Contact Us Form Against Script Injection
Test Steps:
Step 1: Open Contact Us page.
Step 2: Enter <script>alert(1)</script> in subject or message field.
Step 3: Submit the form.
Expected Result: Script should not execute and input should be handled safely.

Session Management

TestCase_ID: TC_070 - Verify User Session Remains Active During Navigation
Test Steps:
Step 1: Login with valid credentials.
Step 2: Navigate to Home, Products, Cart, and Contact Us pages.
Step 3: Verify logged-in username remains visible.
Expected Result: User session should remain active during normal navigation.

TestCase_ID: TC_071 - Verify Session After Browser Refresh
Test Steps:
Step 1: Login with valid credentials.
Step 2: Refresh the browser page.
Step 3: Verify login status.
Expected Result: User should remain logged in if session persistence is supported.

TestCase_ID: TC_072 - Verify Session After Closing and Reopening Browser
Test Steps:
Step 1: Login with valid credentials.
Step 2: Close the browser.
Step 3: Reopen browser and open the application.
Expected Result: System should behave according to session policy. User should not be logged in if persistent session is not supported.

TestCase_ID: TC_073 - Verify Direct Access to Checkout Without Login
Test Steps:
Step 1: Logout from the application.
Step 2: Directly open checkout page URL.
Expected Result: System should not allow unauthorized checkout access and should redirect user to login/register flow.

TestCase_ID: TC_074 - Verify Cart Access Without Login
Test Steps:
Step 1: Logout from the application.
Step 2: Open cart page directly.
Expected Result: Cart page may open for guest user, but checkout should remain restricted until login/register.

TestCase_ID: TC_075 - Verify Multiple Tabs Session Behavior
Test Steps:
Step 1: Login in one browser tab.
Step 2: Open application in another tab.
Step 3: Logout from first tab.
Step 4: Refresh second tab.
Expected Result: User should be logged out from all tabs after logout.

Security Validation

TestCase_ID: TC_076 - Verify Unauthorized Access to Logged-in User Features
Test Steps:
Step 1: Logout from the application.
Step 2: Try to access account-specific features directly through URL.
Expected Result: System should block unauthorized access and redirect user to login/register page.

TestCase_ID: TC_077 - Verify Sensitive Data Is Not Displayed in URL
Test Steps:
Step 1: Login with valid credentials.
Step 2: Complete checkout and payment flow.
Step 3: Observe browser URL during login and payment steps.
Expected Result: Password, card number, CVC, and other sensitive data should not appear in URL.

TestCase_ID: TC_078 - Verify Password Masking on Login and Registration Forms
Test Steps:
Step 1: Open Signup/Login page.
Step 2: Enter password in password field.
Step 3: Observe the entered value.
Expected Result: Password should be masked and should not be visible as plain text.

TestCase_ID: TC_079 - Verify Login Form Against XSS Input
Test Steps:
Step 1: Open Login page.
Step 2: Enter <script>alert(1)</script> in email or password field.
Step 3: Click Login.
Expected Result: Script should not execute and system should display safe validation/error message.

TestCase_ID: TC_080 - Verify Registration Form Against XSS Input
Test Steps:
Step 1: Open Signup page.
Step 2: Enter script tags in name or address fields.
Step 3: Submit the registration form.
Expected Result: Script should not execute and malicious input should be sanitized or rejected.

TestCase_ID: TC_081 - Verify Application Uses Secure HTTPS Connection
Test Steps:
Step 1: Open the application URL.
Step 2: Check browser address bar.
Step 3: Verify connection security details.
Expected Result: Application should load over HTTPS and browser should not show insecure warning.

TestCase_ID: TC_082 - Verify Error Messages Do Not Expose Technical Details
Test Steps:
Step 1: Perform invalid login.
Step 2: Submit invalid search input.
Step 3: Submit invalid contact form data.
Expected Result: Error messages should be user-friendly and should not expose stack trace, database error, or server details.

TestCase_ID: TC_083 - Verify Payment Page Does Not Store Sensitive Card Data After Refresh
Test Steps:
Step 1: Proceed to payment page.
Step 2: Enter card number and CVC.
Step 3: Refresh the page.
Expected Result: Sensitive payment fields should not retain card number or CVC after refresh.

TestCase_ID: TC_084 - Verify Logout Clears Authenticated Session
Test Steps:
Step 1: Login with valid credentials.
Step 2: Click Logout.
Step 3: Try to access checkout or account page directly.
Expected Result: User should not access authenticated pages after logout.

End-to-End Business Flow

TestCase_ID: TC_085 - Verify Complete E-commerce Journey with New User
Test Steps:
Step 1: Open the application.
Step 2: Register a new user with valid details.
Step 3: Browse Products page.
Step 4: Search for a product.
Step 5: Open product detail page.
Step 6: Add product to cart.
Step 7: Proceed to checkout.
Step 8: Verify address and order details.
Step 9: Place order.
Step 10: Enter valid payment details.
Step 11: Confirm order.
Step 12: Download invoice.
Step 13: Logout.
Expected Result: Complete user journey should work successfully without data mismatch or functional error.

TestCase_ID: TC_086 - Verify Complete E-commerce Journey with Existing User
Test Steps:
Step 1: Open the application.
Step 2: Login with existing registered user.
Step 3: Add multiple products to cart.
Step 4: Proceed to checkout.
Step 5: Place order using valid payment details.
Step 6: Download invoice.
Expected Result: Existing user should be able to complete order successfully.

TestCase_ID: TC_087 - Verify User Cannot Checkout with Empty Cart
Test Steps:
Step 1: Login with valid credentials.
Step 2: Open cart page without adding products.
Step 3: Try to proceed to checkout.
Expected Result: System should not allow checkout with empty cart.

TestCase_ID: TC_088 - Verify Price Consistency Across Product, Cart, Checkout, and Invoice
Test Steps:
Step 1: Open product detail page and note product price.
Step 2: Add product to cart.
Step 3: Verify price in cart.
Step 4: Proceed to checkout and verify price.
Step 5: Complete order and download invoice.
Expected Result: Product price should remain consistent across product detail, cart, checkout, and invoice.

TestCase_ID: TC_089 - Verify User Can Delete Account After Order Completion
Test Steps:
Step 1: Login with valid user.
Step 2: Complete an order successfully.
Step 3: Click Delete Account.
Step 4: Verify account deletion message.
Expected Result: User account should be deleted successfully after order completion.

TestCase_ID: TC_090 - Verify Application Handles Page Refresh During Checkout
Test Steps:
Step 1: Login with valid credentials.
Step 2: Add product to cart.
Step 3: Proceed to checkout.
Step 4: Refresh the checkout page.
Expected Result: Checkout page should reload without losing cart and address details.


Test Case Generator Skill

---
name: demoblaze-test-case-generator skill
description: >
 Generate comprehensive, structured, traceable, and automation-ready manual test cases
 for the DemoBlaze web application (https://www.demoblaze.com/). Use this skill when
 given requirements, user stories, acceptance criteria, feature specifications, or a
 website URL scope. Covers functional, negative, validation, boundary, edge,
 session-management, and security-related scenarios following industry-standard QA
 best practices. Always produce output in the canonical table format with all
 mandatory fields populated and automation metadata included.
---


# DemoBlaze Test Case Generator — SKILL


---


## 1. Purpose


Produce **automation-ready** manual test cases for DemoBlaze that are:


- **Traceable** — every test case has a unique, stable ID
- **Atomic** — one behavior verified per test case
- **Deterministic** — steps and expected results are unambiguous
- **Tool-agnostic** — steps can be scripted in Selenium, Playwright, Cypress, or any WebDriver framework without reinterpretation


---


## 2. Application Module Map


| Module Code | Module Name   | Scope / Entry Point                                  |
|-------------|---------------|------------------------------------------------------|
| HOME        | Home Page     | `https://www.demoblaze.com/`                         |
| NAV         | Navigation    | Top navbar links (Home, Contact, About Us, Cart, Login, Sign Up) |
| PROD        | Products      | Product listing, category filter, product detail page |
| CART        | Cart          | Cart page (`/cart.html`), add/remove/total           |
| CHECKOUT    | Checkout      | Place Order modal, purchase confirmation             |
| AUTH        | Authentication| Sign Up modal, Login modal, Logout                   |
| CONTACT     | Contact Form  | Contact modal                                        |
| SESSION     | Session       | Persistence across navigation, logout behaviour      |
| SECURITY    | Security      | XSS, sensitive data exposure, input sanitisation     |
| E2E         | End-to-End    | Full user journey spanning multiple modules          |


---


## 3. Test Case ID Convention


```
TC_<MODULE>_<NNN>
```


- `MODULE` — uppercase module code from §2
- `NNN`    — zero-padded 3-digit sequence, unique within module (001, 002 …)


**Examples:** `TC_HOME_001`, `TC_AUTH_003`, `TC_E2E_001`


---


## 4. Mandatory Fields — Every Test Case


| Field              | Description                                                                                     |
|--------------------|-------------------------------------------------------------------------------------------------|
| **Test Case ID**   | Unique identifier per §3                                                                        |
| **Title**          | Concise action + subject (≤ 80 chars). Start with a verb: *Verify*, *Validate*, *Confirm*, etc. |
| **Priority**       | `High` / `Medium` / `Low`                                                                       |
| **Preconditions**  | System/data state required **before** Step 1 executes                                           |
| **Test Steps**     | Numbered, imperative, single-action per step. Include exact UI labels, URLs, field names        |
| **Test Data**      | Exact values or tokens (e.g., `username: testUser01`, `password: Pass@1234`)                   |
| **Expected Result**| Observable, measurable outcome. No vague terms like "works" or "correct"                        |
| **Test Type**      | One of: `Functional` / `Negative` / `Boundary` / `Edge` / `Security` / `End-to-End`            |
| **Automation Tag** | Comma-separated tags for test-runner grouping (see §5)                                          |
| **Locator Hints**  | CSS selectors, IDs, or XPath hints for the key elements under test                             |


---


## 5. Automation Tags Reference


| Tag               | When to Apply                                              |
|-------------------|------------------------------------------------------------|
| `@smoke`          | Critical path; run on every build                          |
| `@regression`     | Full regression suite                                      |
| `@functional`     | Positive functional flow                                   |
| `@negative`       | Invalid input / error handling                             |
| `@boundary`       | Min/max/limit values                                       |
| `@edge`           | Unusual but valid states                                   |
| `@security`       | XSS, data exposure, auth bypass                            |
| `@e2e`            | Multi-module journeys                                      |
| `@session`        | Login persistence, logout                                  |
| `@cart`           | Cart CRUD operations                                       |
| `@auth`           | Sign Up / Login / Logout                                   |
| `@checkout`       | Order placement flow                                       |
| `@ui`             | Layout / visibility checks                                 |


---


## 6. Canonical Output Format


Use this exact Markdown table structure for every test case:


```markdown
| Field            | Value                        |
|------------------|------------------------------|
| Test Case ID     | TC_<MODULE>_<NNN>            |
| Title            | Verify <action> <subject>    |
| Priority         | High / Medium / Low          |
| Preconditions    | <system/data state>          |
| Test Steps       | 1. <step> <br> 2. <step> … |
| Test Data        | <key: value pairs or N/A>    |
| Expected Result  | <observable, measurable outcome> |
| Test Type        | Functional / Negative / …    |
| Automation Tag   | @smoke, @regression, …       |
| Locator Hints    | `#signInModal`, `.card-title`, … |
```


Group test cases under H3 module headers:
```
### HOME Module
### NAV Module
### PROD Module
…
```


---


## 7. Module-Level Test Coverage Requirements


### 7.1 HOME
- Page load and full element visibility (logo, navbar, carousel, product grid, footer)
- Product card completeness (image, name, price, clickable link)
- Pagination / "Next" / "Previous" navigation
- Page load performance (observable indicator only)


### 7.2 NAV
- Each navbar link routes to the correct destination or opens the correct modal
- Active link / modal title verification
- Back-navigation does not break state


### 7.3 PROD
- Product detail page loads (name, image, price, description, Add to Cart button)
- Category filter (Phones / Laptops / Monitors) shows only relevant products
- Clicking product from filtered view loads correct detail page
- Boundary: category with 0 visible products (edge case)


### 7.4 CART
- Add single product → appears in cart with correct name and price
- Add duplicate product → behaviour documented (no dedup warning on DemoBlaze)
- Remove product → disappears from cart; total recalculates
- Total = Σ(product prices) with multiple items
- Empty cart state (no items, total = 0)
- Cart persistence across page refreshes (session storage behaviour)


### 7.5 CHECKOUT
- Valid order submission → confirmation modal with order ID, amount, card info
- Blank required fields → system alert or no submission (known DemoBlaze behaviour: JS alert fires)
- Partial fields (some filled, some blank)
- Invalid card format (letters in card number field)
- Boundary: maximum field lengths


### 7.6 AUTH
- Sign Up with unique credentials → success alert "Sign up successful"
- Sign Up with existing username → alert "This user already exist."
- Sign Up with blank username → alert fires
- Sign Up with blank password → alert fires
- Login with valid credentials → username appears in navbar
- Login with invalid password → alert "Wrong password."
- Login with non-existent user → alert "User does not exist."
- Login with blank fields → alert fires
- Logout → navbar reverts to Login / Sign Up links


### 7.7 CONTACT
- Valid submission (email, name, message) → alert "Thanks for the message!!"
- Blank submission → no alert or validation behaviour documented
- Special characters / long strings in message field (boundary/edge)


### 7.8 SESSION
- Login persists across page navigations (Home → Cart → Product → Home)
- Logout terminates session; protected actions unavailable
- Session after browser back-button post-logout


### 7.9 SECURITY
- XSS in Sign Up username field: `<script>alert(1)</script>`
- XSS in Contact message field
- XSS in Checkout name/city/card fields
- Sensitive data (password, card number) not visible in page source or URL
- Direct URL access to `/cart.html` without login


### 7.10 E2E
- Full happy path: Sign Up → Login → Browse category → Add product → Cart verification → Place Order → Confirmation
- Guest (unauthenticated) add-to-cart and checkout flow
- Multi-product purchase flow


---


## 8. Test Data Reference


### Valid Users
| Token         | Value         |
|---------------|---------------|
| `{{username}}`| `testUser_<timestamp>` (unique per run) |
| `{{password}}`| `Pass@1234`   |


### Checkout Form
| Field   | Valid Value          | Invalid Value     |
|---------|----------------------|-------------------|
| Name    | `John Doe`           | *(blank)*         |
| Country | `India`              | *(blank)*         |
| City    | `Kolkata`            | *(blank)*         |
| Credit Card | `4111111111111111` | `ABCD`         |
| Month   | `12`                 | *(blank)*         |
| Year    | `2025`               | *(blank)*         |


### XSS Payloads
```
<script>alert(1)</script>
"><img src=x onerror=alert(1)>
javascript:alert(1)
```


---


## 9. Key Locator Reference (DemoBlaze)


| Element                  | Locator                              |
|--------------------------|--------------------------------------|
| Sign Up button (navbar)  | `#signin2`                           |
| Login button (navbar)    | `#login2`                            |
| Sign Up modal            | `#signInModal`                       |
| Login modal              | `#logInModal`                        |
| Sign Up — username field | `#sign-username`                     |
| Sign Up — password field | `#sign-password`                     |
| Login — username field   | `#loginusername`                     |
| Login — password field   | `#loginpassword`                     |
| Navbar logged-in name    | `#nameofuser`                        |
| Logout link              | `#logout2`                           |
| Cart link (navbar)       | `#cartur`                            |
| Add to Cart button       | `a.btn-success` (product detail)     |
| Place Order button       | `.btn-success[data-target="#orderModal"]` |
| Order modal — Name       | `#name`                              |
| Order modal — Country    | `#country`                           |
| Order modal — City       | `#city`                              |
| Order modal — Card       | `#card`                              |
| Order modal — Month      | `#month`                             |
| Order modal — Year       | `#year`                              |
| Purchase button          | `button.btn-primary` (in order modal)|
| Cart total               | `#totalp`                            |
| Cart delete link         | `a:contains("Delete")` (per row)     |
| Product cards            | `.card`                              |
| Product card title       | `.card-title`                        |
| Product card price       | `.card-block h5`                     |
| Category — Phones        | `a[onclick*="phone"]`                |
| Category — Laptops       | `a[onclick*="notebook"]`             |
| Category — Monitors      | `a[onclick*="monitor"]`              |
| Contact modal trigger    | `a[data-target="#exampleModal"]`     |
| Contact email field      | `#recipient-email`                   |
| Contact name field       | `#recipient-name`                    |
| Contact message field    | `#message-text`                      |
| Send message button      | `button[onclick="send()"]`           |


---


## 10. Workflow — How to Generate Test Cases


```
INPUT
 └── Requirements / User story / Feature description / URL scope
       │
       ▼
STEP 1 — Identify module(s) from §2
       │
       ▼
STEP 2 — Enumerate scenarios:
         • 1 Happy-path functional case minimum
         • 1 Negative / invalid-input case per input field
         • Boundary cases for any numeric / length constraint
         • Edge cases (empty state, duplicates, concurrent actions)
         • Session cases if auth context is relevant
         • Security case if user input is accepted
       │
       ▼
STEP 3 — Assign Test Case ID per §3
       │
       ▼
STEP 4 — Populate all 10 mandatory fields from §4
         (Locator Hints from §9; Test Data from §8)
       │
       ▼
STEP 5 — Apply Automation Tags from §5
       │
       ▼
STEP 6 — Render in canonical format from §6,
         grouped under module headers
       │
       ▼
OUTPUT — Markdown test case table(s), ready for
        manual execution or framework scripting
```


---


## 11. Quality Checklist (Validate Each Test Case Before Output)


- [ ] ID is unique and follows `TC_<MODULE>_<NNN>` convention
- [ ] Title starts with a verb and identifies one specific behaviour
- [ ] Preconditions are sufficient to reach Step 1 without ambiguity
- [ ] Each step is a single action; no compound "do X and Y" in one step
- [ ] Test Data uses concrete values, not placeholders like "some input"
- [ ] Expected Result is observable and measurable — no "page works correctly"
- [ ] Automation Tag set is non-empty and accurate
- [ ] Locator Hints reference real DemoBlaze DOM identifiers (§9)
- [ ] Negative tests assert the *specific* error message or behaviour, not just "fails"
- [ ] Security tests specify the exact payload used


---


## 12. Complete Reference Test Cases


The following serve as canonical examples and output anchors.


### HOME Module


| Field           | Value |
|-----------------|-------|
| Test Case ID    | TC_HOME_001 |
| Title           | Verify Home page loads with all structural elements visible |
| Priority        | High |
| Preconditions   | Browser open, no active session required |
| Test Steps      | 1. Navigate to `https://www.demoblaze.com/` <br> 2. Wait for `DOMContentLoaded` <br> 3. Observe presence of: logo, navbar, category sidebar, product grid, footer |
| Test Data       | URL: `https://www.demoblaze.com/` |
| Expected Result | Page title is "STORE", logo is visible, navbar shows Home / Contact / About Us / Cart / Login / Sign Up, product grid contains ≥ 1 card, footer is visible |
| Test Type       | Functional |
| Automation Tag  | @smoke, @regression, @functional, @ui |
| Locator Hints   | `title`, `#nava`, `.navbar`, `.card`, `footer` |


| Field           | Value |
|-----------------|-------|
| Test Case ID    | TC_HOME_002 |
| Title           | Verify each product card displays image, name, and price |
| Priority        | Medium |
| Preconditions   | Home page fully loaded |
| Test Steps      | 1. Locate all elements matching `.card` <br> 2. For each card, assert `.card-img-top` src is not empty <br> 3. Assert `.card-title` text is not empty <br> 4. Assert `.card-block h5` text matches currency pattern (e.g., `$NNN`) |
| Test Data       | N/A |
| Expected Result | Every product card has a non-empty image src, non-empty title, and price formatted as `$[0-9]+` |
| Test Type       | Functional |
| Automation Tag  | @regression, @functional, @ui |
| Locator Hints   | `.card`, `.card-img-top`, `.card-title`, `.card-block h5` |


---


### AUTH Module


| Field           | Value |
|-----------------|-------|
| Test Case ID    | TC_AUTH_001 |
| Title           | Verify Sign Up succeeds with unique username and valid password |
| Priority        | High |
| Preconditions   | Home page loaded; Sign Up modal closed |
| Test Steps      | 1. Click `#signin2` <br> 2. Wait for `#signInModal` to be visible <br> 3. Enter `testUser_<timestamp>` in `#sign-username` <br> 4. Enter `Pass@1234` in `#sign-password` <br> 5. Click `button[onclick="register()"]` <br> 6. Accept browser alert |
| Test Data       | username: `testUser_20240101120000`, password: `Pass@1234` |
| Expected Result | Browser alert text equals "Sign up successful." |
| Test Type       | Functional |
| Automation Tag  | @smoke, @regression, @functional, @auth |
| Locator Hints   | `#signin2`, `#signInModal`, `#sign-username`, `#sign-password`, `button[onclick="register()"]` |


| Field           | Value |
|-----------------|-------|
| Test Case ID    | TC_AUTH_002 |
| Title           | Verify Sign Up fails when username already exists |
| Priority        | High |
| Preconditions   | User `existingUser01` already registered in the system |
| Test Steps      | 1. Click `#signin2` <br> 2. Wait for `#signInModal` <br> 3. Enter `existingUser01` in `#sign-username` <br> 4. Enter `Pass@1234` in `#sign-password` <br> 5. Click Sign Up button <br> 6. Observe alert |
| Test Data       | username: `existingUser01`, password: `Pass@1234` |
| Expected Result | Browser alert text equals "This user already exist." |
| Test Type       | Negative |
| Automation Tag  | @regression, @negative, @auth |
| Locator Hints   | `#sign-username`, `#sign-password`, `button[onclick="register()"]` |


| Field           | Value |
|-----------------|-------|
| Test Case ID    | TC_AUTH_003 |
| Title           | Verify Login succeeds with valid registered credentials |
| Priority        | High |
| Preconditions   | User `testUser01` registered with password `Pass@1234` |
| Test Steps      | 1. Click `#login2` <br> 2. Wait for `#logInModal` <br> 3. Enter `testUser01` in `#loginusername` <br> 4. Enter `Pass@1234` in `#loginpassword` <br> 5. Click `button[onclick="logIn()"]` <br> 6. Wait for modal to close |
| Test Data       | username: `testUser01`, password: `Pass@1234` |
| Expected Result | `#nameofuser` text equals `"Welcome testUser01"` and navbar shows Logout link (`#logout2`) |
| Test Type       | Functional |
| Automation Tag  | @smoke, @regression, @functional, @auth |
| Locator Hints   | `#login2`, `#logInModal`, `#loginusername`, `#loginpassword`, `#nameofuser`, `#logout2` |


| Field           | Value |
|-----------------|-------|
| Test Case ID    | TC_AUTH_004 |
| Title           | Verify Login fails with correct username and wrong password |
| Priority        | High |
| Preconditions   | Login modal open; user `testUser01` exists |
| Test Steps      | 1. Click `#login2` <br> 2. Enter `testUser01` in `#loginusername` <br> 3. Enter `wrongPass` in `#loginpassword` <br> 4. Click Login button <br> 5. Observe alert |
| Test Data       | username: `testUser01`, password: `wrongPass` |
| Expected Result | Browser alert text equals "Wrong password." |
| Test Type       | Negative |
| Automation Tag  | @regression, @negative, @auth |
| Locator Hints   | `#loginusername`, `#loginpassword`, `button[onclick="logIn()"]` |


| Field           | Value |
|-----------------|-------|
| Test Case ID    | TC_AUTH_005 |
| Title           | Verify Login fails with non-existent username |
| Priority        | High |
| Preconditions   | Login modal open |
| Test Steps      | 1. Click `#login2` <br> 2. Enter `ghost_user_xyz` in `#loginusername` <br> 3. Enter `Pass@1234` in `#loginpassword` <br> 4. Click Login button <br> 5. Observe alert |
| Test Data       | username: `ghost_user_xyz`, password: `Pass@1234` |
| Expected Result | Browser alert text equals "User does not exist." |
| Test Type       | Negative |
| Automation Tag  | @regression, @negative, @auth |
| Locator Hints   | `#loginusername`, `#loginpassword` |


---


### CART Module


| Field           | Value |
|-----------------|-------|
| Test Case ID    | TC_CART_001 |
| Title           | Verify single product is added to cart with correct details |
| Priority        | High |
| Preconditions   | Home page loaded; cart is empty |
| Test Steps      | 1. Click product "Samsung galaxy s6" <br> 2. Wait for product detail page <br> 3. Note displayed price <br> 4. Click `a.btn-success` ("Add to cart") <br> 5. Accept alert "Product added." <br> 6. Click `#cartur` (Cart) <br> 7. Locate product row in cart table |
| Test Data       | Product: Samsung galaxy s6 |
| Expected Result | Cart table contains one row with title "Samsung galaxy s6" and price matching product detail page value |
| Test Type       | Functional |
| Automation Tag  | @smoke, @regression, @functional, @cart |
| Locator Hints   | `a.btn-success`, `#cartur`, `#tbodyid tr td:nth-child(2)`, `#tbodyid tr td:nth-child(3)` |


| Field           | Value |
|-----------------|-------|
| Test Case ID    | TC_CART_002 |
| Title           | Verify cart total equals sum of all added product prices |
| Priority        | High |
| Preconditions   | At least 2 different products added to cart |
| Test Steps      | 1. Add Product A to cart; note price P1 <br> 2. Add Product B to cart; note price P2 <br> 3. Navigate to Cart (`#cartur`) <br> 4. Read value of `#totalp` |
| Test Data       | Product A price: P1, Product B price: P2 |
| Expected Result | `#totalp` text equals `P1 + P2` (integer sum, no decimals) |
| Test Type       | Functional |
| Automation Tag  | @regression, @functional, @cart |
| Locator Hints   | `#totalp`, `#tbodyid tr td:nth-child(3)` |


| Field           | Value |
|-----------------|-------|
| Test Case ID    | TC_CART_003 |
| Title           | Verify product is removed from cart on clicking Delete |
| Priority        | High |
| Preconditions   | Cart contains at least one product |
| Test Steps      | 1. Navigate to Cart page <br> 2. Note product name in first row <br> 3. Click "Delete" link in that row <br> 4. Wait 1–2 seconds for DOM update <br> 5. Assert product row no longer present |
| Test Data       | Any product already in cart |
| Expected Result | Cart table no longer contains the deleted product row; `#totalp` decreases by the deleted item's price |
| Test Type       | Functional |
| Automation Tag  | @regression, @functional, @cart |
| Locator Hints   | `#tbodyid tr`, `a:contains("Delete")`, `#totalp` |


---


### CHECKOUT Module


| Field           | Value |
|-----------------|-------|
| Test Case ID    | TC_CHECKOUT_001 |
| Title           | Verify successful order placement with all valid fields |
| Priority        | High |
| Preconditions   | Cart contains at least one product |
| Test Steps      | 1. Navigate to Cart <br> 2. Click Place Order button <br> 3. Enter `John Doe` in `#name` <br> 4. Enter `India` in `#country` <br> 5. Enter `Kolkata` in `#city` <br> 6. Enter `4111111111111111` in `#card` <br> 7. Enter `12` in `#month` <br> 8. Enter `2025` in `#year` <br> 9. Click Purchase button |
| Test Data       | Name: John Doe, Country: India, City: Kolkata, Card: 4111111111111111, Month: 12, Year: 2025 |
| Expected Result | Confirmation modal appears with text containing "Thank you for your purchase!" and an Order ID |
| Test Type       | Functional |
| Automation Tag  | @smoke, @regression, @functional, @checkout |
| Locator Hints   | `.btn-success[data-target="#orderModal"]`, `#name`, `#country`, `#city`, `#card`, `#month`, `#year`, `button.btn-primary` (purchase), `.sweet-alert h2` |


| Field           | Value |
|-----------------|-------|
| Test Case ID    | TC_CHECKOUT_002 |
| Title           | Verify order submission blocked when all required fields are blank |
| Priority        | High |
| Preconditions   | Cart contains at least one product; Place Order modal open |
| Test Steps      | 1. Navigate to Cart <br> 2. Click Place Order button <br> 3. Leave all fields empty <br> 4. Click Purchase button <br> 5. Observe system response |
| Test Data       | All fields: *(blank)* |
| Expected Result | Browser alert fires with text "Please fill out Name and Creditcard." — confirmation modal does NOT appear |
| Test Type       | Negative |
| Automation Tag  | @regression, @negative, @checkout |
| Locator Hints   | `button.btn-primary` (in `#orderModal`), `.sweet-alert` |


| Field           | Value |
|-----------------|-------|
| Test Case ID    | TC_CHECKOUT_003 |
| Title           | Verify order blocked when Name is blank but other fields are populated |
| Priority        | Medium |
| Preconditions   | Place Order modal open; cart has product |
| Test Steps      | 1. Leave `#name` empty <br> 2. Fill Country, City, Card, Month, Year with valid values <br> 3. Click Purchase |
| Test Data       | Name: *(blank)*, Card: `4111111111111111`, others: valid |
| Expected Result | Alert "Please fill out Name and Creditcard." fires; order not placed |
| Test Type       | Negative |
| Automation Tag  | @regression, @negative, @checkout |
| Locator Hints   | `#name`, `button.btn-primary` |


---


### SECURITY Module


| Field           | Value |
|-----------------|-------|
| Test Case ID    | TC_SECURITY_001 |
| Title           | Verify XSS payload in Sign Up username field is not executed |
| Priority        | High |
| Preconditions   | Sign Up modal open |
| Test Steps      | 1. Open Sign Up modal <br> 2. Enter `<script>alert('XSS')</script>` in `#sign-username` <br> 3. Enter `Pass@1234` in `#sign-password` <br> 4. Click Sign Up <br> 5. Observe page and alerts |
| Test Data       | username: `<script>alert('XSS')</script>`, password: `Pass@1234` |
| Expected Result | No JavaScript alert from injected script executes; input is either rejected or stored as literal text |
| Test Type       | Security |
| Automation Tag  | @regression, @security |
| Locator Hints   | `#sign-username`, `#sign-password` |


| Field           | Value |
|-----------------|-------|
| Test Case ID    | TC_SECURITY_002 |
| Title           | Verify password is not visible in page source or URL after login |
| Priority        | High |
| Preconditions   | Valid user registered |
| Test Steps      | 1. Login with valid credentials <br> 2. After login, inspect current URL <br> 3. View page source (Ctrl+U) <br> 4. Search page source for password value |
| Test Data       | username: `testUser01`, password: `Pass@1234` |
| Expected Result | URL does not contain `Pass@1234`; page source does not contain `Pass@1234` in plain text |
| Test Type       | Security |
| Automation Tag  | @regression, @security |
| Locator Hints   | Browser URL bar, page source |


---


### SESSION Module


| Field           | Value |
|-----------------|-------|
| Test Case ID    | TC_SESSION_001 |
| Title           | Verify login session persists after navigating between pages |
| Priority        | Medium |
| Preconditions   | User logged in successfully |
| Test Steps      | 1. Confirm `#nameofuser` shows logged-in name on Home <br> 2. Navigate to Cart (`/cart.html`) <br> 3. Assert `#nameofuser` still visible and non-empty <br> 4. Click a product to open detail page <br> 5. Assert `#nameofuser` still visible |
| Test Data       | username: `testUser01` |
| Expected Result | `#nameofuser` displays `"Welcome testUser01"` on all navigated pages |
| Test Type       | Functional |
| Automation Tag  | @regression, @session, @functional |
| Locator Hints   | `#nameofuser`, `#logout2` |


| Field           | Value |
|-----------------|-------|
| Test Case ID    | TC_SESSION_002 |
| Title           | Verify logout clears session and reverts navbar to guest state |
| Priority        | High |
| Preconditions   | User logged in |
| Test Steps      | 1. Click `#logout2` <br> 2. Wait for page to update <br> 3. Observe navbar |
| Test Data       | N/A |
| Expected Result | `#nameofuser` is empty or hidden; `#login2` and `#signin2` are visible; `#logout2` is hidden |
| Test Type       | Functional |
| Automation Tag  | @smoke, @regression, @session, @auth |
| Locator Hints   | `#logout2`, `#nameofuser`, `#login2`, `#signin2` |


---


### E2E Module


| Field           | Value |
|-----------------|-------|
| Test Case ID    | TC_E2E_001 |
| Title           | Verify complete user journey: Sign Up → Login → Add to Cart → Place Order → Confirm |
| Priority        | High |
| Preconditions   | Fresh browser session; no existing user with the test username |
| Test Steps      | 1. Navigate to `https://www.demoblaze.com/` <br> 2. Click Sign Up; register `e2eUser_<ts>` / `Pass@1234`; accept alert <br> 3. Click Login; enter same credentials; accept <br> 4. Confirm `#nameofuser` shows username <br> 5. Click category "Phones" <br> 6. Click first product in list <br> 7. Note product price <br> 8. Click Add to Cart; accept alert <br> 9. Click Cart link <br> 10. Verify product row exists and `#totalp` = noted price <br> 11. Click Place Order <br> 12. Fill all fields with valid test data <br> 13. Click Purchase <br> 14. Assert confirmation modal text contains "Thank you for your purchase!" |
| Test Data       | username: `e2eUser_<timestamp>`, password: `Pass@1234`, Name: John Doe, Country: India, City: Kolkata, Card: 4111111111111111, Month: 12, Year: 2025 |
| Expected Result | At each checkpoint: (a) username displayed post-login, (b) product in cart with correct price, (c) order confirmation modal visible with "Thank you for your purchase!" and an Order ID |
| Test Type       | End-to-End |
| Automation Tag  | @smoke, @e2e, @regression |
| Locator Hints   | `#signin2`, `#sign-username`, `#sign-password`, `#login2`, `#loginusername`, `#loginpassword`, `#nameofuser`, `a[onclick*="phone"]`, `.card`, `a.btn-success`, `#cartur`, `#totalp`, `.btn-success[data-target="#orderModal"]`, `#name`, `#card`, `button.btn-primary`, `.sweet-alert h2` |




