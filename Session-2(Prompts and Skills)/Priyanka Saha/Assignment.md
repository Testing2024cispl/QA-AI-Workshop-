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






