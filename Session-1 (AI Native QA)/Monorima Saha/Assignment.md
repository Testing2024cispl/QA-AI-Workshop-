QA Manual Test Cases:- 

Member 1:-Monorima Saha
Query/Test cases:- https://automationexercise.com/ 

Human Thinking Test Cases 

Test Cases_001:- (User registration) 

Open the browse
Navigate to url 'http://automationexercise.com' 
Verify that home page is visible successfully
Click on 'Signup / Login' button
Verify 'New User Signup!' is visible
Enter name and email address
Click 'Signup' button
Verify that 'ENTER ACCOUNT INFORMATION' is visible 
Enter name and already registered email address
Click 'Signup' button
Verify error 'Email Address already exist!' is visible
Enter name and unique email address 
Then click on “Signup
Verify that 'ENTER ACCOUNT INFORMATION' is visible” 
Fill the following details: Title, Name, Email, Password, Date of birth
Select checkbox 'Sign up for our newsletter!'
Select checkbox 'Receive special offers from our partners!'
Fill details: First name, Last name, Company, Address, Address2, Country, State, City, Zipcode, Mobile Number
Click 'Create Account button'
Verify that 'ACCOUNT CREATED!' is visible
Click 'Continue' button
Verify that 'Logged in as username' is visible 


Test Cases_002:- (User login with correct email address and password) 


1. Open the browse
2. Navigate to url 'http://automationexercise.com' 
3. Verify that home page is visible successfully
4. Click on 'Signup / Login' button
5. Verify 'Login to your account' is visible
6. Enter correct email address and password
7. Click 'login' button
8. Verify that 'Logged in as username' is visible

Test Cases_003:- (User login with incorrect email address and password) 
1. Open the browse
2. Navigate to url 'http://automationexercise.com' 
3. Verify that home page is visible successfully
4. Click on 'Signup / Login' button
5. Verify 'Login to your account' is visible
6. Enter incorrect email address and password
7. Click 'login' button
8. Verify error 'Your email or password is incorrect!' is visible 
Test Cases_004:- (Place order after registration) 
Open the browser 
Navigate  to [http://automationexercise.com ].
Confirm that the home page loads and is fully visible.
Click on the 'Signup / Login' button.
Fill in all required registration details (Name, Email, Password, Address, Date of Birth,Company, Address, Address 2, Country, State,City, Zipcode,Mobile Number)
Click the 'Create Account' button.
Verify that the 'ACCOUNT CREATED!' message is displayed, then click the 'Continue' button.
Confirm that 'Logged in as [username]' is visibly displayed at the top of the page.
Browse the store and add desired products to the shopping cart.
Click the 'Cart' button in the header.
Confirm that the cart page displays the correct selected items.
IClick the 'Proceed To Checkout' button.
Verify that the delivery/billing Address Details are correct and review the order items.
Enter a description/instruction in the comment text area and click 'Place Order'.
Enter the payment details (Name on Card, Card Number, CVC, and Expiration Date) and click the 'Pay and Confirm Order' button.
Verify the success message 'Your order has been placed successfully!' 
Test Cases_005:- (Place order: Register while Checkout) 

Open the browser 
Navigate to (http://automationexercise.com ).
Confirm that the home page loads successfully.
Select and add the desired products to the shopping cart.
Click the 'Cart' button and verify that the cart page is correctly displayed with the selected items.
Authentication Interception (Sign Up)
Click the 'Proceed To Checkout' button.
From the checkout prompt, click the 'Register / Login' button.
Fill in all required signup information and complete the account creation process.
Verify that 'ACCOUNT CREATED!' is displayed, and click 'Continue'.
Confirm that the header displays 'Logged in as [username]'.
Order Completion & Payment
Click the 'Cart' button to return to the active session's cart.
Click 'Proceed To Checkout' again.
Verify that the registered Address Details match and review the order summary.
Input an optional description in the comment text box and click 'Place Order'.
Enter the payment details (Name on Card, Card Number, CVC, and Expiration Date) and click 'Pay and Confirm Order'. 
Verify the success message 'Your order has been placed successfully!' 
AI Manual Test Cases:- 
User login 

Prompt : Act as an expert Manual QA . I need you to generate a comprehensive suite of test cases for the login functionality of the website "Automation Exercise".



Reference URL: https://automationexercise.com/login  
TC_LOG_001: Successful Login with Valid Credentials (Positive)
Pre-conditions: The user must have a previously registered and active account on the platform.
Test Steps:
Open the browser and navigate to https://automationexercise.com/login.
Locate the "Login to your account" section.
Enter a valid registered email into the Email Address field.
Enter the matching valid password into the Password field.
Click the Login button.
Test Data: * Email: valid_user@example.com
Password: ValidPassword123
Expected Result: The user is redirected to the home page. The header displays "Logged in as [Username]" and a "Logout" button becomes visible.
TC_LOG_002: Login Attempt with Incorrect Password (Negative)
Pre-conditions: The email address used must be a valid, registered account.
Test Steps:
Navigate to https://automationexercise.com/login.
Enter the valid registered email into the Email Address field.
Enter an incorrect/invalid string into the Password field.
Click the Login button.
Test Data: * Email: valid_user@example.com
Password: WrongPassword!!!
Expected Result: Login fails. The user remains on the login page. A visible red error message is displayed: "Your email or password is incorrect!".
TC_LOG_003: Login Attempt with Unregistered Email (Negative)
Pre-conditions: The email address used must not exist in the database.
Test Steps:
Navigate to https://automationexercise.com/login.
Enter an unregistered email address into the Email Address field.
Enter any random characters into the Password field.
Click the Login button.
Test Data: * Email: nonexistent_qa_user_2026@domain.com
Password: RandomPassword
Expected Result: Login fails. The application displays the validation error: "Your email or password is incorrect!".
TC_LOG_004: Validation of Blank Inputs (Negative)
Pre-conditions: User is on the login/signup page.
Test Steps:
Clear any pre-filled data from the Email Address and Password text fields.
Leave both fields completely empty.
Click the Login button.
Test Data: None (Blank fields)
Expected Result: The form is not submitted. Browser/HTML5-native validation triggers, highlighting the empty field with a validation prompt (e.g., "Please fill out this field").
TC_LOG_005: Validation of Empty Password Field (Negative)
Pre-conditions: User is on the login/signup page.
Test Steps:
Enter a valid email format into the Email Address field.
Leave the Password field completely empty.
Click the Login button.
Test Data: * Email: valid_user@example.com
Expected Result: Submission is blocked. The browser focuses on the password field displaying a standard prompt requesting input.
TC_LOG_006: Invalid Email Format Handling (Boundary/Validation)
Pre-conditions: User is on the login page.
Test Steps:
Enter a malformed string missing standard syntax (e.g., no @ symbol or no top-level domain) into the Email Address field.
Enter a value into the Password field.
Click the Login button.
Test Data: * Email: test_user_at_domain.com or test_user@domain
Password: Password123
Expected Result: HTML5 form validation intercepts the submission, displaying a notice indicating that the input format is invalid (e.g., "Please include an '@' in the email address").
TC_LOG_007: Password Field Character Masking (Security)
Pre-conditions: User is on the login page.
Test Steps:
Click inside the Password field under the "Login to your account" section.
Type alphanumeric and special characters.
Observe how characters are displayed on the UI.
Test Data: SecretP@$$w0rd
Expected Result: All characters entered are instantly masked using bullet points (•) or asterisks (*). Plain text must not be exposed. The HTML element must possess the property type="password".
TC_LOG_008: Basic SQL Injection Vulnerability Test (Security)
Pre-conditions: User is on the login page.
Test Steps:
Enter a typical SQL injection payload into both the Email Address and Password fields.
Click the Login button.
Test Data: * Input: ' OR '1'='1
Expected Result: The system securely treats the payload as a generic literal string. System logs no database exceptions to the client UI, authentication fails, and the default message "Your email or password is incorrect!" appears.
TC_LOG_009: Post-Logout Session Restriction (Functional)
Pre-conditions: The user is actively logged into their account.
Test Steps:
Click the Logout button located in the top navigation header bar.
Verify redirection back to https://automationexercise.com/login.
Click the browser's Back arrow button.
Test Data: N/A
Expected Result: Clicking logout tears down the active session. Attempting to click the browser's back button should either keep the user on the login page or redirect them back to the landing page as an unauthenticated guest; they must not access the previously authenticated session views.
TC_LOG_010: UI Verification & Layout Check (UI/UX)
Pre-conditions: Access the site using standard desktop and laptop screen resolutions (e.g., 1920x1080, 1366x768).
Test Steps:
Navigate directly to https://automationexercise.com/login.
Inspect the presentation layout.
Verify the existence of the "Login to your account" block on the left side and "New User Signup!" on the right.
Ensure placeholders ("Email Address", "Password") exist inside the entry inputs.
Expected Result: Text descriptions are spelled cleanly without typos. Structural elements do not overlap, forms are correctly aligned, and fields are fully clickable/accessible. 

User registration 
Prompt: Act as a Senior Manual QA Engineer. I need you to generate a robust suite of test cases for the Signup functionality of the website "Automation Exercise".



Reference URL: https://automationexercise.com/login 

TC_SIGN_001: Initial Signup Step-1 with Unique Credentials (Positive)
Pre-conditions: The user is on the login/signup landing page, and the email address used must not exist in the database.
Test Steps:
Navigate to [https://automationexercise.com/login](https://automationexercise.com/login).
Locate the "New User Signup!" section on the right-hand side.
Enter a valid name in the Name field.
Enter a unique, unregistered email address in the Email Address field.
Click the Signup button.
Test Data:
Name: John Doe
Email: johndoe_qa_2026@example.com
Expected Result: The user is successfully redirected to the detailed registration page ([https://automationexercise.com/signup](https://automationexercise.com/signup)), and the section header "ENTER ACCOUNT INFORMATION" is visible.
TC_SIGN_002: Initial Signup Step-1 with Existing Email (Negative)
Pre-conditions: An account with the chosen email address must already be fully registered and active on the system.
Test Steps:
Navigate to [https://automationexercise.com/login](https://automationexercise.com/login).
Go to the "New User Signup!" section.
Enter any name in the Name field.
Enter an already registered email address in the Email Address field.
Click the Signup button.
Test Data:
Name: John Duplicate
Email: already_registered_user@example.com
Expected Result: Form submission fails. The page does not redirect, and a red error message is clearly displayed below the signup form: "Email Address already exist!".
TC_SIGN_003: Step-2 Complete Account Creation with All Fields (Positive)
Pre-conditions: User has successfully passed Step-1 and is currently viewing the /signup form.
Test Steps:
Select a title radio button (e.g., Mr. or Mrs.).
Verify that Name and Email fields are pre-populated.
Enter a valid string into the Password field.
Select Day, Month, and Year dropdown values under Date of Birth.
Select both checkboxes: "Sign up for our newsletter!" and "Receive special offers from our partners!".
Fill out all address profile information fields: First name, Last name, Company, Address, Address 2, select a Country, State, City, Zipcode, and Mobile Number.
Click the Create Account button.
Test Data: Comprehensive dummy datasets matching standard address structures.
Expected Result: The account is generated cleanly. The application redirects to [https://automationexercise.com/account_created](https://automationexercise.com/account_created), displaying a large green/black confirmation header text: "ACCOUNT CREATED!".
TC_SIGN_004: Step-2 Mandatory Field Validation (Negative)
Pre-conditions: User has successfully completed Step-1 and is on the /signup page.
Test Steps:
Leave the Password field entirely empty.
Leave critical address information fields (First name, Last name, Address, State, City, Zipcode, Mobile Number) blank.
Click the Create Account button.
Expected Result: Page validation halts form submission. The browser intercepts the action using standard HTML5 constraints, flashing a validation tooltip over the first missing mandatory text input field (e.g., "Please fill out this field"). No account is created in the database.
TC_SIGN_005: Step-2 Read-Only Email Integrity Check (UI/UX / Security)
Pre-conditions: User has successfully passed Step-1 and is on the /signup page.
Test Steps:
Locate the Email text box under the "Enter Account Information" block.
Attempt to click into the field, clear the text, or type new characters inside it.
Inspect the underlying DOM element for the field using browser DevTools.
Expected Result: The Email field must be visually grayed out/immutable and completely non-editable by the user. The HTML element must contain either the disabled or readonly attribute, ensuring user data continuity from Step-1.
TC_SIGN_006: Step-2 Checkbox Selection Independency (Functional)
Pre-conditions: User is on the /signup page.
Test Steps:
Click the label or checkbox for "Sign up for our newsletter!" and verify it becomes marked active.
Click it a second time to uncheck it.
Click the checkbox for "Receive special offers from our partners!" while leaving the newsletter checkbox unchecked.
Proceed to fill out mandatory data fields and click Create Account.
Expected Result: Both checkboxes must act independently (not behaving like exclusive radio items). The system successfully records the state where only one selection is saved upon profile confirmation.
TC_SIGN_007: Validation of Invalid Email Formatting in Step-1 (Boundary)
Pre-conditions: User is on the login/signup page.
Test Steps:
In the "New User Signup!" box, enter a valid name.
Input a bad syntax string into the Email Address field (e.g., testuser@, @domain.com, or testuser.domain.com).
Click the Signup button.
Expected Result: Browser-native email type validation blocks form submission, displaying a localized warning indicating that the text is missing an @ symbol or domain configuration. The user is not allowed to reach Step-2. 
Place order after registration

Prompt: Act as a Senior QA Automation Engineer. Generate a comprehensive suite of test cases for the End-to-End (E2E) "Register and Place Order" workflow on Automation Exercise.

Reference URL: https://automationexercise.com/   
TC_M_E2E_01: Register While Checkout (Mid-Stream User Journey)
Pre-conditions: Access to a modern desktop web browser. Use a new, unique email address for this run.
Execution Steps:
Open your browser and navigate to [https://automationexercise.com/]
Verify: The home page loads successfully; banners and the main navigation header are visible.
Scroll down to the products list, hover over the first product, and click "Add to Cart".
When the confirmation modal appears, click the "View Cart" button.
Verify: The page redirects to /view_cart. The correct product, quantity (1), and price are present.
Click the "Proceed To Checkout" button.
On the checkout modal popup, click the "Register / Login" text link.
Under "New User Signup!" on the right, input a name and a unique email address. Click "Signup".
Complete all fields on the /signup detailed registration form (Title, Password, Date of Birth, Full Address, and Mobile Number). Click "Create Account".
Verify: The page updates to /account_created, displaying "ACCOUNT CREATED!". Click "Continue".
Verify: The top navigation bar displays a user icon with the text "Logged in as [Your Name]".
Click the "Cart" button in the header menu, then click "Proceed To Checkout".
Verify: The checkout page displays two panels: "Address Details" and "Review Your Order".
Enter a text comment in the description text area (e.g., "Leave at the front door"), then click "Place Order".
On the payment page, fill in dummy inputs for Name on Card, Card Number, CVC, and Expiration Date. Click "Pay and Confirm Order".
Verify: A confirmation layout appears stating "ORDER PLACED!" with a success message: "Your order has been placed successfully!".
Click "Delete Account" in the top navigation bar.
Verify: The page updates to display "ACCOUNT DELETED!". Click "Continue" to return to the anonymous home screen state.
Expected Result: The user completes the entire flow from guest to paying customer, and the account is cleanly purged at the end without database or session errors.
TC_M_E2E_02: Register Before Checkout (Pre-Authenticated Journey)
Pre-conditions: Ensure you have a new email address ready for registration.
Execution Steps:
Navigate to [https://automationexercise.com/]
Click the "Signup / Login" button in the top navigation header.
Under "New User Signup!", input a name and email, then complete the full account registration form immediately.
Verify: Upon clicking "Continue" on the Account Created screen, you are returned to the home page with the header displaying "Logged in as [Your Name]".
Click the "Products" button in the navigation header.
Search or scroll for any item, click "Add to Cart", and then click "View Cart" on the confirmation popup.
Click the "Proceed To Checkout" button.
Verify: The system bypasses the authentication intercept modal and directs you straight to the /checkout page showing your address details.
Enter an order comment, click "Place Order", fill out the credit card form, and confirm payment.
Verify: The order successfully completes with the confirmation message displayed.
Click "Delete Account" to restore clean test data conditions.
Expected Result: A pre-authenticated user builds a cart and checks out directly without hitting intercept barriers or losing cart items.
TC_M_E2E_03: Checkout Address & Data Integrity Verification
Pre-conditions: User is executing Step 1 of registration.
Execution Steps:
Advance through the initial registration step until you reach the detailed registration form (/signup).
Input highly specific, contrasting strings into the address lines:
First Name / Last Name: Jane / Tester
Address 1: 456 Manual Verification Lane
Address 2: Suite 9B (Upper Level)
State / City / Zip: New York / Brooklyn / 11201
Complete account creation and navigate back to the Cart page with items added.
Click "Proceed To Checkout".
Verify (Address Block Mapping):
Check the "Your Delivery Address" block. Confirm it reads exactly as input in Step 2.
Check the "Your Billing Address" block. Confirm it perfectly mirrors the delivery address text strings.
Look for truncated lines, missing details, or misaligned text spacing.
Expected Result: Custom registration metrics map exactly to the checkout invoice page without any truncated words or format issues.
TC_M_E2E_04: Payment Form Field Validation (Negative Boundary Case)
Pre-conditions: The tester is logged in and has reached the payment processing page (/payment).
Execution Steps:
Leave the Card Number and CVC text input boxes completely empty.
Fill out valid entries for Name on Card and Expiration Date.
Click the "Pay and Confirm Order" button.
Verify: Look for native browser validation alerts or on-page form alerts. The application must prevent navigation to /payment_done.
Fill in an invalid alphabetical string into the CVC text input (e.g., ABC).
Click "Pay and Confirm Order".
Verify: The application prevents payment processing or reports formatting problems.
Expected Result: The order processing step blocks incomplete data entry and prevents submission to protect payment data integrity. 
Place order: Register while Checkout 

Prompt: Act as a Senior Manual QA Engineer. Generate a detailed test suite for the End-to-End (E2E) workflow: "Place Order: Register while Checkout" on Automation Exercise.



Reference URL: https://automationexercise.com/ 

TC_RWC_001: Place Order - Register while Checkout (Happy Path E2E)
Pre-conditions: Access to a modern desktop browser with a cleared cache. Prepare a unique email address prefix (e.g., qa_register_checkout_2026@example.com).
Execution Steps:
Open the browser and navigate to [https://automationexercise.com/]
Verify: The home page loads successfully; product categories and the main navbar are visible.
Hover over the first available product card and click "Add to Cart".
When the confirmation popup appears, click "Continue Shopping".
Hover over a second product card and click "Add to Cart".
When the confirmation popup appears, click the "View Cart" link text.
Verify: The app navigates to /view_cart. Both items are present with a total quantity of 1 each.
Click the "Proceed To Checkout" button on the right side of the cart summary.
On the popup modal overlay, click the "Register / Login" text link.
Under the "New User Signup!" column on the right, input a name and your prepared unique email. Click "Signup".
On the detailed registration form (/signup), fill out all mandatory information: Select Title, enter Password (• masked), Date of Birth, First Name, Last Name, Address, Country, State, City, Zipcode, and Mobile Number.
Click the "Create Account" button.
Verify: The page redirects to /account_created with the header "ACCOUNT CREATED!". Click "Continue".
Verify: The header navigation bar now displays "Logged in as [Your Name]".
Click the "Cart" button in the top menu, then click "Proceed To Checkout".
Verify: The page shifts to /checkout. Both the "Address Details" and "Review Your Order" tables are loaded.
Type a custom message in the comment description text area, then click "Place Order".
On the /payment page, fill in valid dummy credit card details (Name on Card, Card Number, CVC, Expiration Date).
Click the "Pay and Confirm Order" button.
Verify: The application displays "ORDER PLACED!" with a success message stating your order has been placed successfully.
Click "Delete Account" in the top navigation bar.
Verify: The page updates to show "ACCOUNT DELETED!". Click "Continue" to return safely to the anonymous homepage.
Expected Result: The user successfully moves from anonymous cart building to registration, finishes the payment transaction, and cleans up the test data footprints without errors.
TC_RWC_002: Cart State Persistence Across Authentication Boundary
Pre-conditions: The user must be unauthenticated and have items in their cart.
Execution Steps:
Navigate to [https://automationexercise.com/] and select "Products" from the top menu.
Add three distinct products to the cart, then go to the /view_cart page.
Click "Proceed To Checkout" and click "Register / Login" on the intercept modal.
Complete the entire signup process using unique credentials and click "Continue" on the final confirmation screen.
Click back on the "Cart" link in the navigation header.
Verify: Look closely at the cart table grid. It must retain exactly the same three distinct items added when you were an anonymous guest. No items should be dropped, missing, or duplicated into higher quantities.
Expected Result: The application merges or retains anonymous cart items cleanly after a user registers mid-session.
TC_RWC_003: Checkout Address Profile Data Integrity Verification
Pre-conditions: The tester is executing the signup phase of the Register while Checkout journey.
Execution Steps:
Progress through the cart checkout process until you reach the detailed registration layout form (/signup).
Input highly descriptive, distinct alpha-numeric characters inside the address parameters:
First/Last Name: Jordan / Automation
Address 1: 777 Integration Boulevard
Address 2: Apartment Block 4C
State / City / Zip: Texas / Austin / 73301
Complete the account creation screen, return to the Cart page, and click "Proceed To Checkout".
Verify (Delivery Panel Check): Read line-by-line the strings inside the "Your Delivery Address" element container. Ensure name, addresses, and geographic coordinates perfectly match the strings from Step 2.
Verify (Billing Panel Check): Read line-by-line the strings inside the "Your Billing Address" element container. Confirm they match your input and mirror the delivery data exactly.
Expected Result: Profile parameters map directly into the functional invoice panels without truncating text lines or scrambling data fields.
TC_RWC_004: Payment Screen Missing Data Constraints (Negative Case)
Pre-conditions: The user is logged in, has a populated cart, and has advanced past the checkout overview down to the /payment node.
Execution Steps:
Intentionally leave the Name on Card and Card Number text input boxes blank.
Enter values into the CVC, Expiration Month, and Expiration Year inputs.
Click the "Pay and Confirm Order" button.
Verify: Ensure the application intercepts the processing attempt. It must show a missing field warning or an active HTML5 form warning, blocking advancement to /payment_done.
Enter alphabetical characters into the Card Number field (e.g., THISISNOTACARD).
Click "Pay and Confirm Order".
Verify: The application highlights layout errors or rejects the entry formatting.
Expected Result: The order processing step drops or halts invalid financial execution paths to preserve database data integrity.
Your thoughts:- 
● What you felt Suitable:- 
The AI provided clean metadata outlines including explicit Pre-conditions, distinct Test Data, and isolated Expected Results, which keeps a testing repository organized. 

AI Test Cases
Best for:
Structured documentation
Negative testing
Automation preparation
Strong in coverage & structure, weak in practical prioritization.

● What you felt Not suitable:- 
Generates a massive volume of individual scenarios, which can quickly lead to document clutter and duplicate steps. 

Manual Test Cases
Best for:
Business flow validation
Functional understanding
Exploratory testing
Strong in domain understanding, weak in structure & edge coverage.

Final Test Case (Automation Ready):- 
TC_REG_001: New User Registration & Account Deletion Lifecycle
Pre-conditions: Test data utility must supply a dynamically generated email string to prevent collision loops.
Test Steps:
Navigate to [https://automationexercise.com/]
Click the Signup / Login header navigation link.
Assert element selector .signup-form containing text "New User Signup!" is visible.
Input text Automation User into the signup name field.
Input text auto_test_2026_${Date.now()}@example.com into the signup email field.
Click the selector button button[data-qa="signup-button"].
Assert current URL matches /signup. Assert element .login-form containing text "ENTER ACCOUNT INFORMATION" is visible.
Click radio button #id_gender1 (Mr.).
Input text SecurePass123! into input selector #password.
Select dropdown values: #days -> 15, #months -> 8, #years -> 1995.
Check checkboxes: #newsletter, #optin.
Fill profile data inputs: #first_name (Jane), #last_name (Tester), #company (QA Org), #address1 (123 Automation Way), #country (United States), #state (California), #city (San Jose), #zipcode (95112), #mobile_number (1234567890).
Click action button button[data-qa="create-account"].
Assert current URL matches /account_created. Assert selector b containing text "ACCOUNT CREATED!" is visible.
Click anchor element [data-qa="continue-button"].
Assert text selector containing content "Logged in as Automation User" is visible in the header bar.
Click anchor element link a[href="/delete_account"].
Assert current URL matches /delete_account. Assert text "ACCOUNT DELETED!" is visible.
Click anchor element [data-qa="continue-button"].
TC_REG_002: Re-registration Block via Existing Email Validation
Pre-conditions: A baseline user profile with email existing_qa_2026@example.com must exist in the system.
Test Steps:
Navigate to [https://automationexercise.com/login](https://automationexercise.com/login)
Input text Duplicate Name into the signup name text field.
Input text existing_qa_2026@example.com into the signup email text field.
Click button selector button[data-qa="signup-button"].
Assert form submission is halted. Assert text content of selector .signup-form p matches precisely: "Email Address already exist!".
TC_REG_003: Step-2 Read-Only Data Attribute Verification
Test Steps:
Initiate registration with a unique identity and advance to the /signup configuration view.
Locate input selector #email.
Assert that the DOM element selector #email possesses the functional property parameter attribute value disabled or readonly.
Suite 2: Session & Identity (authentication.spec.js)
TC_AUTH_001: Successful Account Login with Valid Credentials
Test Steps:
Navigate to [https://automationexercise.com/login]
Assert element .login-form containing text "Login to your account" is visible.
Input text valid_user@example.com into text box #login-form input[data-qa="login-email"].
Input text ValidPassword123 into text box #login-form input[data-qa="login-password"].
Click button selector button[data-qa="login-button"].
Assert current URL matches base landing path.
Assert text locator containing "Logged in as [Username]" is verified active on the page layout.
TC_AUTH_002: Login Rejection Handling via Mismatched Credentials
Test Steps:
Navigate to [https://automationexercise.com/login]
Input text valid_user@example.com into email field.
Input text WrongPassword!!! into password field.
Click button selector button[data-qa="login-button"].
Assert system state does not redirect.
Assert text content of selector .login-form p matches precisely: "Your email or password is incorrect!".
TC_AUTH_003: Client-Side Input Masking & Security Property Verification
Test Steps:
Navigate to [https://automationexercise.com/login](https://automationexercise.com/login)
Locate target element selector #login-form input[data-qa="login-password"].
Assert that the element's attribute property value type is strictly equal to "password".
TC_AUTH_004: Post-Logout Session & Back-Buffer Termination
Test Steps:
Log into the system using the steps mapped in TC_AUTH_001.
Click the navbar anchor link a[href="/logout"].
Assert current URL matches /login.
Trigger browser driver navigation commands to execute a sequential path Page.back().
Assert that the session does not restore, and the application safely routes or forces the browser view back to the unauthenticated login landing page state.
Suite 3: E2E Checkout Flows (checkout.spec.js)
TC_E2E_001: Place Order - Post-Registration Workflow Path
Test Steps:
Complete user setup via execution paths defined in TC_REG_001, stopping right after asserting the header text "Logged in as [Username]".
Navigate to [https://automationexercise.com/products].
Hover on the first product node, click a.add-to-cart. Click "Continue Shopping" on the overlay selector modal.
Hover on the second product node, click a.add-to-cart. Click "View Cart" link on the overlay selector modal.
Assert current URL matches /view_cart. Verify element grid item rows equal 2.
Click anchor link button selector .check_out.
Assert current URL matches /checkout.
Scrape string value from element #address_delivery. Assert address line matches input variables used during account creation.
Input text description comment into target selector textarea .form-control.
Click anchor action button a[href="/payment"].
Input payment mock parameters into input selectors: .card-name, .card-number, .card-cvc, .card-expiry-month, .card-expiry-year.
Click action button selector #submit.
Assert system safely transitions to URL path /payment_done. Assert container success elements reveal text message: "Your order has been placed successfully!".
Execute cleanup: Click a[href="/delete_account"] to reset DB footprint state.
TC_E2E_002: Place Order - Mid-Checkout Gateway Registration Path
Test Steps:
Navigate directly as an unauthenticated guest to [https://automationexercise.com/products]
Add selected item structures to the active shopping session cart, then click through to open /view_cart.
Click button selector .check_out.
Assert transactional modal intercept popup reveals on-screen. Click the text link parameter node "Register / Login".
Complete full registration configurations using a runtime unique dynamic email string.
After account creation confirmation, click back to /view_cart.
Assert cart context state persistence: Verify that the items added prior to authentication remain listed inside the cart table layout configuration untouched.
Click button selector .check_out.
Complete payment fields via credentials mapped in TC_E2E_001. Confirm success output message state.






 









