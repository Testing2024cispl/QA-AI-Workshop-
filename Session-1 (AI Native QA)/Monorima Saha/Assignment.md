# Table of Contents

- [QA Manual Test Cases](#QA_manual_test_cases)
- [Human Thinking Test Cases](#human-thinking-test-cases)
- [AI Manual Test Cases](#ai-manual-test-cases)
- [Prompt ](#prompt)
- [My Thoughts](#my-thoughts)
- [Final Test Cases (AI + Manual Combined) – Automation Ready](#final-test-cases-ai--manual-combined--automation-ready)


# QA Manual Test Cases:- 

Member 1:-Monorima Saha
Query/Test cases:- https://automationexercise.com/ 


# Human Thinking Test Cases 


Test Cases_001:- (User registration) 


1. Open the browse
2. Navigate to url 'http://automationexercise.com' 
3. Verify that home page is visible successfully
4. Click on 'Signup / Login' button
5. Verify 'New User Signup!' is visible
6. Enter name and email address
7. Click 'Signup' button
8. Verify that 'ENTER ACCOUNT INFORMATION' is visible 
9. Enter name and already registered email address
10. Click 'Signup' button
11. Verify error 'Email Address already exist!' is visible
12. Enter name and unique email address 
13. Then click on “Signup
14. Verify that 'ENTER ACCOUNT INFORMATION' is visible” 
15. Fill the following details: Title, Name, Email, Password, Date of birth
16. Select checkbox 'Sign up for our newsletter!'
17. Select checkbox 'Receive special offers from our partners!'
18. Fill details: First name, Last name, Company, Address, Address2, Country, State, City, Zipcode, Mobile Number
19. Click 'Create Account button'
20. Verify that 'ACCOUNT CREATED!' is visible
21. Click 'Continue' button
22. Verify that 'Logged in as username' is visible 




*Test Cases_002:- (User login with correct email address and password)* 




1. Open the browse
2. Navigate to url 'http://automationexercise.com' 
3. Verify that home page is visible successfully
4. Click on 'Signup / Login' button
5. Verify 'Login to your account' is visible
6. Enter correct email address and password
7. Click 'login' button
8. Verify that 'Logged in as username' is visible


*Test Cases_003:- (User login with incorrect email address and password)* 
1. Open the browse
2. Navigate to url 'http://automationexercise.com' 
3. Verify that home page is visible successfully
4. Click on 'Signup / Login' button
5. Verify 'Login to your account' is visible
6. Enter incorrect email address and password
7. Click 'login' button
8. Verify error 'Your email or password is incorrect!' is visible 
Test Cases_004:- (Place order after registration) 
1. Open the browser 
2. Navigate  to [http://automationexercise.com ].
3. Confirm that the home page loads and is fully visible.
4. Click on the 'Signup / Login' button.
5. Fill in all required registration details (Name, Email, Password, Address, Date of Birth,Company, Address, Address 2, Country, State,City, Zipcode,Mobile Number)
6. Click the 'Create Account' button.
7. Verify that the 'ACCOUNT CREATED!' message is displayed, then click the 'Continue' button.
8. Confirm that 'Logged in as [username]' is visibly displayed at the top of the page.
9. Browse the store and add desired products to the shopping cart.
10. Click the 'Cart' button in the header.
11. Confirm that the cart page displays the correct selected items.
12. IClick the 'Proceed To Checkout' button.
13. Verify that the delivery/billing Address Details are correct and review the order items.
14. Enter a description/instruction in the comment text area and click 'Place Order'.
15. Enter the payment details (Name on Card, Card Number, CVC, and Expiration Date) and click the 'Pay and Confirm Order' button.
16. Verify the success message 'Your order has been placed successfully!' 

*Test Cases_005:- (Place order: Register while Checkout)*


1. Open the browser 
2. Navigate to (http://automationexercise.com ).
3. Confirm that the home page loads successfully.
4. Select and add the desired products to the shopping cart.
5. Click the 'Cart' button and verify that the cart page is correctly displayed with the selected items.
6. Authentication Interception (Sign Up)
7. Click the 'Proceed To Checkout' button.
8. From the checkout prompt, click the 'Register / Login' button.
9. Fill in all required signup information and complete the account creation process.
10. Verify that 'ACCOUNT CREATED!' is displayed, and click 'Continue'.
11. Confirm that the header displays 'Logged in as [username]'.
12. Order Completion & Payment
13. Click the 'Cart' button to return to the active session's cart.
14. Click 'Proceed To Checkout' again.
15. Verify that the registered Address Details match and review the order summary.
16. Input an optional description in the comment text box and click 'Place Order'.
17. Enter the payment details (Name on Card, Card Number, CVC, and Expiration Date) and click 'Pay and Confirm Order'. 
18. Verify the success message 'Your order has been placed successfully!' 
# AI Manual Test Cases:- 
User login 


# Prompt : Act as an expert Manual QA . I need you to generate a comprehensive suite of test cases for the login functionality of the website "Automation Exercise".






Reference URL: https://automationexercise.com/login  

*TC_LOG_001: Successful Login with Valid Credentials (Positive)*
* Pre-conditions: The user must have a previously registered and active account on the platform.
* Test Steps:
   * Open the browser and navigate to https://automationexercise.com/login.
   * Locate the "Login to your account" section.
   * Enter a valid registered email into the Email Address field.
   * Enter the matching valid password into the Password field.
   * Click the Login button.
* Test Data: * Email: valid_user@example.com
   * Password: ValidPassword123
* Expected Result: The user is redirected to the home page. The header displays "Logged in as [Username]" and a "Logout" button becomes visible.

*TC_LOG_002: Login Attempt with Incorrect Password (Negative)*
* Pre-conditions: The email address used must be a valid, registered account.
* Test Steps:
   * Navigate to https://automationexercise.com/login.
   * Enter the valid registered email into the Email Address field.
   * Enter an incorrect/invalid string into the Password field.
   * Click the Login button.
* Test Data: * Email: valid_user@example.com
   * Password: WrongPassword!!!
* Expected Result: Login fails. The user remains on the login page. A visible red error message is displayed: "Your email or password is incorrect!".

*TC_LOG_003: Login Attempt with Unregistered Email (Negative)*

* Pre-conditions: The email address used must not exist in the database.
* Test Steps:
   * Navigate to https://automationexercise.com/login.
   * Enter an unregistered email address into the Email Address field.
   * Enter any random characters into the Password field.
   * Click the Login button.
* Test Data: * Email: nonexistent_qa_user_2026@domain.com
   * Password: RandomPassword
* Expected Result: Login fails. The application displays the validation error: "Your email or password is incorrect!".
TC_LOG_004: Validation of Blank Inputs (Negative)
* Pre-conditions: User is on the login/signup page.
* Test Steps:
   1. Clear any pre-filled data from the Email Address and Password text fields.
   2. Leave both fields completely empty.
   3. Click the Login button.
* Test Data: None (Blank fields)
* Expected Result: The form is not submitted. Browser/HTML5-native validation triggers, highlighting the empty field with a validation prompt (e.g., "Please fill out this field").

*TC_LOG_005: Validation of Empty Password Field (Negative)*

* Pre-conditions: User is on the login/signup page.
* Test Steps:
   1. Enter a valid email format into the Email Address field.
   2. Leave the Password field completely empty.
   3. Click the Login button.
* Test Data: * Email: valid_user@example.com
* Expected Result: Submission is blocked. The browser focuses on the password field displaying a standard prompt requesting input.

*TC_LOG_006: Invalid Email Format Handling (Boundary/Validation)*
* Pre-conditions: User is on the login page.
* Test Steps:
   * Enter a malformed string missing standard syntax (e.g., no @ symbol or no top-level domain) into the Email Address field.
   * Enter a value into the Password field.
   * Click the Login button.
* Test Data: * Email: test_user_at_domain.com or test_user@domain
   * Password: Password123
* Expected Result: HTML5 form validation intercepts the submission, displaying a notice indicating that the input format is invalid (e.g., "Please include an '@' in the email address").

*TC_LOG_007: Password Field Character Masking (Security)*

* Pre-conditions: User is on the login page.
* Test Steps:
   1. Click inside the Password field under the "Login to your account" section.
   2. Type alphanumeric and special characters.
   3. Observe how characters are displayed on the UI.
* Test Data: SecretP@$$w0rd
* Expected Result: All characters entered are instantly masked using bullet points (•) or asterisks (*). Plain text must not be exposed. The HTML element must possess the property type="password".

*TC_LOG_008: Basic SQL Injection Vulnerability Test (Security)*

* Pre-conditions: User is on the login page.
* Test Steps:
   1. Enter a typical SQL injection payload into both the Email Address and Password fields.
   2. Click the Login button.
* Test Data: * Input: ' OR '1'='1
* Expected Result: The system securely treats the payload as a generic literal string. System logs no database exceptions to the client UI, authentication fails, and the default message "Your email or password is incorrect!" appears.
TC_LOG_009: Post-Logout Session Restriction (Functional)
* Pre-conditions: The user is actively logged into their account.
* Test Steps:
   1. Click the Logout button located in the top navigation header bar.
   2. Verify redirection back to https://automationexercise.com/login.
   3. Click the browser's Back arrow button.
* Test Data: N/A
* Expected Result: Clicking logout tears down the active session. Attempting to click the browser's back button should either keep the user on the login page or redirect them back to the landing page as an unauthenticated guest; they must not access the previously authenticated session views.

*TC_LOG_010: UI Verification & Layout Check (UI/UX)*

* Pre-conditions: Access the site using standard desktop and laptop screen resolutions (e.g., 1920x1080, 1366x768).
* Test Steps:
   1. Navigate directly to https://automationexercise.com/login.
   2. Inspect the presentation layout.
   3. Verify the existence of the "Login to your account" block on the left side and "New User Signup!" on the right.
   4. Ensure placeholders ("Email Address", "Password") exist inside the entry inputs.
* Expected Result: Text descriptions are spelled cleanly without typos. Structural elements do not overlap, forms are correctly aligned, and fields are fully clickable/accessible. 


User registration 
# Prompt: Act as a Senior Manual QA Engineer. I need you to generate a robust suite of test cases for the Signup functionality of the website "Automation Exercise".






Reference URL: https://automationexercise.com/login 


*TC_SIGN_001: Initial Signup Step-1 with Unique Credentials (Positive)*

* Pre-conditions: The user is on the login/signup landing page, and the email address used must not exist in the database.
* Test Steps:
   * Navigate to [https://automationexercise.com/login](https://automationexercise.com/login).
   * Locate the "New User Signup!" section on the right-hand side.
   * Enter a valid name in the Name field.
   * Enter a unique, unregistered email address in the Email Address field.
   * Click the Signup button.
* Test Data:
   * Name: John Doe
   * Email: johndoe_qa_2026@example.com
* Expected Result: The user is successfully redirected to the detailed registration page ([https://automationexercise.com/signup](https://automationexercise.com/signup)), and the section header "ENTER ACCOUNT INFORMATION" is visible.

*TC_SIGN_002: Initial Signup Step-1 with Existing Email (Negative)*

* Pre-conditions: An account with the chosen email address must already be fully registered and active on the system.
* Test Steps:
   * Navigate to [https://automationexercise.com/login](https://automationexercise.com/login).
   * Go to the "New User Signup!" section.
   * Enter any name in the Name field.
   * Enter an already registered email address in the Email Address field.
   * Click the Signup button.
* Test Data:
   * Name: John Duplicate
   * Email: already_registered_user@example.com
* Expected Result: Form submission fails. The page does not redirect, and a red error message is clearly displayed below the signup form: "Email Address already exist!".

*TC_SIGN_003: Step-2 Complete Account Creation with All Fields (Positive)*

* Pre-conditions: User has successfully passed Step-1 and is currently viewing the /signup form.
* Test Steps:
   1. Select a title radio button (e.g., Mr. or Mrs.).
   2. Verify that Name and Email fields are pre-populated.
   3. Enter a valid string into the Password field.
   4. Select Day, Month, and Year dropdown values under Date of Birth.
   5. Select both checkboxes: "Sign up for our newsletter!" and "Receive special offers from our partners!".
   6. Fill out all address profile information fields: First name, Last name, Company, Address, Address 2, select a Country, State, City, Zipcode, and Mobile Number.
   7. Click the Create Account button.
* Test Data: Comprehensive dummy datasets matching standard address structures.
* Expected Result: The account is generated cleanly. The application redirects to [https://automationexercise.com/account_created](https://automationexercise.com/account_created), displaying a large green/black confirmation header text: "ACCOUNT CREATED!".
TC_SIGN_004: Step-2 Mandatory Field Validation (Negative)
* Pre-conditions: User has successfully completed Step-1 and is on the /signup page.
* Test Steps:
   1. Leave the Password field entirely empty.
   2. Leave critical address information fields (First name, Last name, Address, State, City, Zipcode, Mobile Number) blank.
   3. Click the Create Account button.
* Expected Result: Page validation halts form submission. The browser intercepts the action using standard HTML5 constraints, flashing a validation tooltip over the first missing mandatory text input field (e.g., "Please fill out this field"). No account is created in the database.

*TC_SIGN_005: Step-2 Read-Only Email Integrity Check (UI/UX / Security)*
* Pre-conditions: User has successfully passed Step-1 and is on the /signup page.
* Test Steps:
   1. Locate the Email text box under the "Enter Account Information" block.
   2. Attempt to click into the field, clear the text, or type new characters inside it.
   3. Inspect the underlying DOM element for the field using browser DevTools.
* Expected Result: The Email field must be visually grayed out/immutable and completely non-editable by the user. The HTML element must contain either the disabled or readonly attribute, ensuring user data continuity from Step-1.

*TC_SIGN_006: Step-2 Checkbox Selection Independency (Functional)*
* Pre-conditions: User is on the /signup page.
* Test Steps:
   1. Click the label or checkbox for "Sign up for our newsletter!" and verify it becomes marked active.
   2. Click it a second time to uncheck it.
   3. Click the checkbox for "Receive special offers from our partners!" while leaving the newsletter checkbox unchecked.
   4. Proceed to fill out mandatory data fields and click Create Account.
* Expected Result: Both checkboxes must act independently (not behaving like exclusive radio items). The system successfully records the state where only one selection is saved upon profile confirmation.

*TC_SIGN_007: Validation of Invalid Email Formatting in Step-1 (Boundary)*

* Pre-conditions: User is on the login/signup page.
* Test Steps:
   1. In the "New User Signup!" box, enter a valid name.
   2. Input a bad syntax string into the Email Address field (e.g., testuser@, @domain.com, or testuser.domain.com).
   3. Click the Signup button.
* Expected Result: Browser-native email type validation blocks form submission, displaying a localized warning indicating that the text is missing an @ symbol or domain configuration. The user is not allowed to reach Step-2. 
Place order after registration


# Prompt: Act as a Senior QA Automation Engineer. Generate a comprehensive suite of test cases for the End-to-End (E2E) "Register and Place Order" workflow on Automation Exercise.


Reference URL: https://automationexercise.com/   

*TC_M_E2E_01: Register While Checkout (Mid-Stream User Journey)*  

* Pre-conditions: Access to a modern desktop web browser. Use a new, unique email address for this run.
Execution Steps:
1. Open your browser and navigate to [https://automationexercise.com/]
2. Verify: The home page loads successfully; banners and the main navigation header are visible.
3. Scroll down to the products list, hover over the first product, and click "Add to Cart".
4. When the confirmation modal appears, click the "View Cart" button.
5. Verify: The page redirects to /view_cart. The correct product, quantity (1), and price are present.
6. Click the "Proceed To Checkout" button.
7. On the checkout modal popup, click the "Register / Login" text link.
8. Under "New User Signup!" on the right, input a name and a unique email address. Click "Signup".
9. Complete all fields on the /signup detailed registration form (Title, Password, Date of Birth, Full Address, and Mobile Number). Click "Create Account".
10. Verify: The page updates to /account_created, displaying "ACCOUNT CREATED!". Click "Continue".
11. Verify: The top navigation bar displays a user icon with the text "Logged in as [Your Name]".
12. Click the "Cart" button in the header menu, then click "Proceed To Checkout".
13. Verify: The checkout page displays two panels: "Address Details" and "Review Your Order".
14. Enter a text comment in the description text area (e.g., "Leave at the front door"), then click "Place Order".
15. On the payment page, fill in dummy inputs for Name on Card, Card Number, CVC, and Expiration Date. Click "Pay and Confirm Order".
16. Verify: A confirmation layout appears stating "ORDER PLACED!" with a success message: "Your order has been placed successfully!".
17. Click "Delete Account" in the top navigation bar.
18. Verify: The page updates to display "ACCOUNT DELETED!". Click "Continue" to return to the anonymous home screen state.
* Expected Result: The user completes the entire flow from guest to paying customer, and the account is cleanly purged at the end without database or session errors.
*TC_M_E2E_02: Register Before Checkout (Pre-Authenticated Journey)*

* Pre-conditions: Ensure you have a new email address ready for registration.
Execution Steps:
1. Navigate to [https://automationexercise.com/]
2. Click the "Signup / Login" button in the top navigation header.
3. Under "New User Signup!", input a name and email, then complete the full account registration form immediately.
4. Verify: Upon clicking "Continue" on the Account Created screen, you are returned to the home page with the header displaying "Logged in as [Your Name]".
5. Click the "Products" button in the navigation header.
6. Search or scroll for any item, click "Add to Cart", and then click "View Cart" on the confirmation popup.
7. Click the "Proceed To Checkout" button.
8. Verify: The system bypasses the authentication intercept modal and directs you straight to the /checkout page showing your address details.
9. Enter an order comment, click "Place Order", fill out the credit card form, and confirm payment.
10. Verify: The order successfully completes with the confirmation message displayed.
11. Click "Delete Account" to restore clean test data conditions.
* Expected Result: A pre-authenticated user builds a cart and checks out directly without hitting intercept barriers or losing cart items.
TC_M_E2E_03: Checkout Address & Data Integrity Verification
* Pre-conditions: User is executing Step 1 of registration.
Execution Steps:
1. Advance through the initial registration step until you reach the detailed registration form (/signup).
2. Input highly specific, contrasting strings into the address lines:
   * First Name / Last Name: Jane / Tester
   * Address 1: 456 Manual Verification Lane
   * Address 2: Suite 9B (Upper Level)
   * State / City / Zip: New York / Brooklyn / 11201
3. Complete account creation and navigate back to the Cart page with items added.
4. Click "Proceed To Checkout".
5. Verify (Address Block Mapping):
   * Check the "Your Delivery Address" block. Confirm it reads exactly as input in Step 2.
   * Check the "Your Billing Address" block. Confirm it perfectly mirrors the delivery address text strings.
   * Look for truncated lines, missing details, or misaligned text spacing.
* Expected Result: Custom registration metrics map exactly to the checkout invoice page without any truncated words or format issues.
TC_M_E2E_04: Payment Form Field Validation (Negative Boundary Case)
* Pre-conditions: The tester is logged in and has reached the payment processing page (/payment).
Execution Steps:
1. Leave the Card Number and CVC text input boxes completely empty.
2. Fill out valid entries for Name on Card and Expiration Date.
3. Click the "Pay and Confirm Order" button.
4. Verify: Look for native browser validation alerts or on-page form alerts. The application must prevent navigation to /payment_done.
5. Fill in an invalid alphabetical string into the CVC text input (e.g., ABC).
6. Click "Pay and Confirm Order".
7. Verify: The application prevents payment processing or reports formatting problems.
* Expected Result: The order processing step blocks incomplete data entry and prevents submission to protect payment data integrity. 
Place order: Register while Checkout 


# Prompt: Act as a Senior Manual QA Engineer. Generate a detailed test suite for the End-to-End (E2E) workflow: "Place Order: Register while Checkout" on Automation Exercise.






Reference URL: https://automationexercise.com/ 


*TC_RWC_001: Place Order - Register while Checkout (Happy Path E2E)*

* Pre-conditions: Access to a modern desktop browser with a cleared cache. Prepare a unique email address prefix (e.g., qa_register_checkout_2026@example.com).
Execution Steps:
1. Open the browser and navigate to [https://automationexercise.com/]
2. Verify: The home page loads successfully; product categories and the main navbar are visible.
3. Hover over the first available product card and click "Add to Cart".
4. When the confirmation popup appears, click "Continue Shopping".
5. Hover over a second product card and click "Add to Cart".
6. When the confirmation popup appears, click the "View Cart" link text.
7. Verify: The app navigates to /view_cart. Both items are present with a total quantity of 1 each.
8. Click the "Proceed To Checkout" button on the right side of the cart summary.
9. On the popup modal overlay, click the "Register / Login" text link.
10. Under the "New User Signup!" column on the right, input a name and your prepared unique email. Click "Signup".
11. On the detailed registration form (/signup), fill out all mandatory information: Select Title, enter Password (• masked), Date of Birth, First Name, Last Name, Address, Country, State, City, Zipcode, and Mobile Number.
12. Click the "Create Account" button.
13. Verify: The page redirects to /account_created with the header "ACCOUNT CREATED!". Click "Continue".
14. Verify: The header navigation bar now displays "Logged in as [Your Name]".
15. Click the "Cart" button in the top menu, then click "Proceed To Checkout".
16. Verify: The page shifts to /checkout. Both the "Address Details" and "Review Your Order" tables are loaded.
17. Type a custom message in the comment description text area, then click "Place Order".
18. On the /payment page, fill in valid dummy credit card details (Name on Card, Card Number, CVC, Expiration Date).
19. Click the "Pay and Confirm Order" button.
20. Verify: The application displays "ORDER PLACED!" with a success message stating your order has been placed successfully.
21. Click "Delete Account" in the top navigation bar.
22. Verify: The page updates to show "ACCOUNT DELETED!". Click "Continue" to return safely to the anonymous homepage.
* Expected Result: The user successfully moves from anonymous cart building to registration, finishes the payment transaction, and cleans up the test data footprints without errors.

*TC_RWC_002: Cart State Persistence Across Authentication Boundary* 

* Pre-conditions: The user must be unauthenticated and have items in their cart.
Execution Steps:
1. Navigate to [https://automationexercise.com/] and select "Products" from the top menu.
2. Add three distinct products to the cart, then go to the /view_cart page.
3. Click "Proceed To Checkout" and click "Register / Login" on the intercept modal.
4. Complete the entire signup process using unique credentials and click "Continue" on the final confirmation screen.
5. Click back on the "Cart" link in the navigation header.
6. Verify: Look closely at the cart table grid. It must retain exactly the same three distinct items added when you were an anonymous guest. No items should be dropped, missing, or duplicated into higher quantities.
* Expected Result: The application merges or retains anonymous cart items cleanly after a user registers mid-session.

*TC_RWC_003: Checkout Address Profile Data Integrity Verification*

* Pre-conditions: The tester is executing the signup phase of the Register while Checkout journey.
Execution Steps:
1. Progress through the cart checkout process until you reach the detailed registration layout form (/signup).
2. Input highly descriptive, distinct alpha-numeric characters inside the address parameters:
   * First/Last Name: Jordan / Automation
   * Address 1: 777 Integration Boulevard
   * Address 2: Apartment Block 4C
   * State / City / Zip: Texas / Austin / 73301
3. Complete the account creation screen, return to the Cart page, and click "Proceed To Checkout".
4. Verify (Delivery Panel Check): Read line-by-line the strings inside the "Your Delivery Address" element container. Ensure name, addresses, and geographic coordinates perfectly match the strings from Step 2.
5. Verify (Billing Panel Check): Read line-by-line the strings inside the "Your Billing Address" element container. Confirm they match your input and mirror the delivery data exactly.
* Expected Result: Profile parameters map directly into the functional invoice panels without truncating text lines or scrambling data fields.

*TC_RWC_004: Payment Screen Missing Data Constraints (Negative Case)*
* Pre-conditions: The user is logged in, has a populated cart, and has advanced past the checkout overview down to the /payment node.
Execution Steps:
1. Intentionally leave the Name on Card and Card Number text input boxes blank.
2. Enter values into the CVC, Expiration Month, and Expiration Year inputs.
3. Click the "Pay and Confirm Order" button.
4. Verify: Ensure the application intercepts the processing attempt. It must show a missing field warning or an active HTML5 form warning, blocking advancement to /payment_done.
5. Enter alphabetical characters into the Card Number field (e.g., THISISNOTACARD).
6. Click "Pay and Confirm Order".
7. Verify: The application highlights layout errors or rejects the entry formatting.
* Expected Result: The order processing step drops or halts invalid financial execution paths to preserve database data integrity.

# My thoughts:- 
● What you felt Suitable:- 
The AI provided clean metadata outlines including explicit Pre-conditions, distinct Test Data, and isolated Expected Results, which keeps a testing repository organized. 


AI Test Cases
Best for:
* Structured documentation
* Negative testing
* Automation preparation
Strong in coverage & structure, weak in practical prioritization.


● What you felt Not suitable:- 
Generates a massive volume of individual scenarios, which can quickly lead to document clutter and duplicate steps. 


Manual Test Cases
Best for:
* Business flow validation
* Functional understanding
* Exploratory testing
Strong in domain understanding, weak in structure & edge coverage.


# Final Test Case (Automation Ready):- 
TC_REG_001: New User Registration & Account Deletion Lifecycle
* Pre-conditions: Test data utility must supply a dynamically generated email string to prevent collision loops.
* Test Steps:
   1. Navigate to [https://automationexercise.com/]
   2. Click the Signup / Login header navigation link.
   3. Assert element selector .signup-form containing text "New User Signup!" is visible.
   4. Input text Automation User into the signup name field.
   5. Input text auto_test_2026_${Date.now()}@example.com into the signup email field.
   6. Click the selector button button[data-qa="signup-button"].
   7. Assert current URL matches /signup. Assert element .login-form containing text "ENTER ACCOUNT INFORMATION" is visible.
   8. Click radio button #id_gender1 (Mr.).
   9. Input text SecurePass123! into input selector #password.
   10. Select dropdown values: #days -> 15, #months -> 8, #years -> 1995.
   11. Check checkboxes: #newsletter, #optin.
   12. Fill profile data inputs: #first_name (Jane), #last_name (Tester), #company (QA Org), #address1 (123 Automation Way), #country (United States), #state (California), #city (San Jose), #zipcode (95112), #mobile_number (1234567890).
   13. Click action button button[data-qa="create-account"].
   14. Assert current URL matches /account_created. Assert selector b containing text "ACCOUNT CREATED!" is visible.
   15. Click anchor element [data-qa="continue-button"].
   16. Assert text selector containing content "Logged in as Automation User" is visible in the header bar.
   17. Click anchor element link a[href="/delete_account"].
   18. Assert current URL matches /delete_account. Assert text "ACCOUNT DELETED!" is visible.
   19. Click anchor element [data-qa="continue-button"].
TC_REG_002: Re-registration Block via Existing Email Validation
* Pre-conditions: A baseline user profile with email existing_qa_2026@example.com must exist in the system.
* Test Steps:
   1. Navigate to [https://automationexercise.com/login](https://automationexercise.com/login)
   2. Input text Duplicate Name into the signup name text field.
   3. Input text existing_qa_2026@example.com into the signup email text field.
   4. Click button selector button[data-qa="signup-button"].
   5. Assert form submission is halted. Assert text content of selector .signup-form p matches precisely: "Email Address already exist!".
TC_REG_003: Step-2 Read-Only Data Attribute Verification
* Test Steps:
   1. Initiate registration with a unique identity and advance to the /signup configuration view.
   2. Locate input selector #email.
   3. Assert that the DOM element selector #email possesses the functional property parameter attribute value disabled or readonly.
Suite 2: Session & Identity (authentication.spec.js)
TC_AUTH_001: Successful Account Login with Valid Credentials
* Test Steps:
   1. Navigate to [https://automationexercise.com/login]
   2. Assert element .login-form containing text "Login to your account" is visible.
   3. Input text valid_user@example.com into text box #login-form input[data-qa="login-email"].
   4. Input text ValidPassword123 into text box #login-form input[data-qa="login-password"].
   5. Click button selector button[data-qa="login-button"].
   6. Assert current URL matches base landing path.
   7. Assert text locator containing "Logged in as [Username]" is verified active on the page layout.
TC_AUTH_002: Login Rejection Handling via Mismatched Credentials
* Test Steps:
   1. Navigate to [https://automationexercise.com/login]
   2. Input text valid_user@example.com into email field.
   3. Input text WrongPassword!!! into password field.
   4. Click button selector button[data-qa="login-button"].
   5. Assert system state does not redirect.
   6. Assert text content of selector .login-form p matches precisely: "Your email or password is incorrect!".
TC_AUTH_003: Client-Side Input Masking & Security Property Verification
* Test Steps:
   1. Navigate to [https://automationexercise.com/login](https://automationexercise.com/login)
   2. Locate target element selector #login-form input[data-qa="login-password"].
   3. Assert that the element's attribute property value type is strictly equal to "password".
TC_AUTH_004: Post-Logout Session & Back-Buffer Termination
* Test Steps:
   1. Log into the system using the steps mapped in TC_AUTH_001.
   2. Click the navbar anchor link a[href="/logout"].
   3. Assert current URL matches /login.
   4. Trigger browser driver navigation commands to execute a sequential path Page.back().
   5. Assert that the session does not restore, and the application safely routes or forces the browser view back to the unauthenticated login landing page state.
Suite 3: E2E Checkout Flows (checkout.spec.js)
TC_E2E_001: Place Order - Post-Registration Workflow Path
* Test Steps:
   1. Complete user setup via execution paths defined in TC_REG_001, stopping right after asserting the header text "Logged in as [Username]".
   2. Navigate to [https://automationexercise.com/products].
   3. Hover on the first product node, click a.add-to-cart. Click "Continue Shopping" on the overlay selector modal.
   4. Hover on the second product node, click a.add-to-cart. Click "View Cart" link on the overlay selector modal.
   5. Assert current URL matches /view_cart. Verify element grid item rows equal 2.
   6. Click anchor link button selector .check_out.
   7. Assert current URL matches /checkout.
   8. Scrape string value from element #address_delivery. Assert address line matches input variables used during account creation.
   9. Input text description comment into target selector textarea .form-control.
   10. Click anchor action button a[href="/payment"].
   11. Input payment mock parameters into input selectors: .card-name, .card-number, .card-cvc, .card-expiry-month, .card-expiry-year.
   12. Click action button selector #submit.
   13. Assert system safely transitions to URL path /payment_done. Assert container success elements reveal text message: "Your order has been placed successfully!".
   14. Execute cleanup: Click a[href="/delete_account"] to reset DB footprint state.
TC_E2E_002: Place Order - Mid-Checkout Gateway Registration Path
* Test Steps:
   1. Navigate directly as an unauthenticated guest to [https://automationexercise.com/products]
   2. Add selected item structures to the active shopping session cart, then click through to open /view_cart.
   3. Click button selector .check_out.
   4. Assert transactional modal intercept popup reveals on-screen. Click the text link parameter node "Register / Login".
   5. Complete full registration configurations using a runtime unique dynamic email string.
   6. After account creation confirmation, click back to /view_cart.
   7. Assert cart context state persistence: Verify that the items added prior to authentication remain listed inside the cart table layout configuration untouched.
   8. Click button selector .check_out.
   9. Complete payment fields via credentials mapped in TC_E2E_001. Confirm success output message state.
