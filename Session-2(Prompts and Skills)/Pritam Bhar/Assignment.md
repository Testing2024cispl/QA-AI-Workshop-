# QA Manual Test Cases

**Member Name: Pritam Bhar**

**URL: https://advantageonlineshopping.com/**

Human Thinking Test Cases
## Module Name - Registration
### TestCase001 (Navigate to Create Account page)
1. Go to Advantage Online Shopping.
2. Click on the profile icon in the header section.
3. Click on the “Create Account” option.
4. The Create Account page should be displayed.
### TestCase002 (Register with valid details)
1. Go to Advantage Online Shopping.
2. Click on the profile icon in the header section.
3. Click on the “Create Account” option.
4. Fill in all the details correctly.
5. Click on the Register button.
6. The user should be redirected to the home page, and the profile name should be shown beside the profile icon.
### TestCase003 (Register without filling mandatory fields)
1. Go to Advantage Online Shopping.
2. Click on the profile icon in the header section.
3. Click on the “Create Account” option.
4. Leave the username, email, password, and confirm password fields blank.
5. Click on the Register button.
6. The user should not be able to click on the Register button.
### TestCase004 (Register with username less than 5 characters)
1. Go to Advantage Online Shopping.
2. Click on the profile icon in the header section.
3. Click on the “Create Account” option.
4. Enter a username with fewer than 5 characters.
5. A validation message should be displayed below the username field.
### TestCase005 (Register with a password less than 4 characters)
1. Go to Advantage Online Shopping.
2. Click on the profile icon in the header section.
3. Click on the “Create Account” option.
4. Navigate to the password field.
5. Enter a password with fewer than 4 characters.
6. A validation message should be displayed below the password field.
### TestCase006 (Register with a password of more than 12 characters)
1. Go to Advantage Online Shopping.
2. Click on the profile icon in the header section.
3. Click on the “Create Account” option.
4. Navigate to the password field.
5. Enter a password with more than 12 characters.
6. A validation message should be displayed below the password field.
### TestCase007 (Register with a mismatched password and confirm password)
1. Go to Advantage Online Shopping.
2. Click on the profile icon in the header section.
3. Click on the “Create Account” option.
4. Navigate to the password field.
5. Enter different values in the password and confirm password fields.
6. A validation message should be displayed below the password field.
### TestCase008 (Register with a password containing only lower-case letters)
1. Go to Advantage Online Shopping.
2. Click on the profile icon in the header section.
3. Click on the “Create Account” option.
4. Enter a password with more than 4 characters using only lower-case letters.
5. A validation message should prompt the user to include numbers and at least one upper-case character.
### TestCase009 (Register with a password containing only upper-case letters)
1. Go to Advantage Online Shopping.
2. Click on the profile icon in the header section.
3. Click on the “Create Account” option.
4. Enter a password with more than 4 characters using only upper-case letters.
5. A validation message should prompt the user to include numbers and at least one lower-case character.
### TestCase010 (Register with a password containing only numbers)
1. Go to Advantage Online Shopping.
2. Click on the profile icon in the header section.
3. Click on the “Create Account” option.
4. Enter a password with more than 4 digits, using numbers only.
5. A validation message should prompt the user to include at least one upper-case and one lower-case character.
### TestCase011 (Register with phone number exceeding 10 digits)
1. Go to Advantage Online Shopping.
2. Click on the profile icon in the header section.
3. Click on the “Create Account” option.
4. Try to enter a phone number with more than 10 digits.
5. The user should not be able to enter more than 10 digits in the phone number field.
### TestCase012 (Register with an alphabetic or alphanumeric phone number)
1. Go to Advantage Online Shopping.
2. Click on the profile icon in the header section.
3. Click on the “Create Account” option.
4. Try to enter alphabetic or alphanumeric characters in the phone number field.
5. The user should not be able to enter alphabetic or alphanumeric characters in the phone number field.
### TestCase013 (Register without accepting Terms and Conditions)
1. Go to Advantage Online Shopping.
2. Click on the profile icon in the header section.
3. Click on the “Create Account” option.
4. Fill in all the details correctly.
5. Do not check the “I agree to the www.AdvantageOnlineShopping.com Conditions of Use and Privacy Notice” checkbox.
6. Try to click on the Register button.
7. The user should not be able to click on the Register button.
### TestCase014 (Navigate to the Login page from the Create Account page)
1. Go to Advantage Online Shopping.
2. Click on the profile icon in the header section.
3. Click on the “Create Account” option.
4. Navigate to the footer section.
5. Click on the “Already have an account?” button.
6. The user should be navigated to the Login page.
### TestCase015 (Verify social media links on Create Account page)
1. Go to Advantage Online Shopping.
2. Click on the profile icon in the header section.
3. Click on the “Create Account” option.
4. Navigate to the footer section.
5. Click on the Facebook, Twitter, and LinkedIn icons.
6. Each icon should redirect to its respective page.
### TestCase016 (Navigate to registration via checkout flow)
1. Go to Advantage Online Shopping.
2. Select any product category.
3. Select a product.
4. Click on the “Add To Cart” button on the product details page.
5. Click on Checkout.
6. Click on the “Registration” button.
7. The user should be redirected to the Create Account page.
### TestCase017 (Verify order cannot be placed without login or registration)
1. Go to Advantage Online Shopping.
2. Select any product category.
3. Select a product.
4. Click on the “Add To Cart” button on the product details page.
5. Click on Checkout.
6. Without registering or logging in, the user should not be able to place an order.
### TestCase018 (Login via checkout flow with correct credentials)
1. Go to Advantage Online Shopping.
2. Select any product category.
3. Select a product.
4. Click on the “Add To Cart” button on the product details page.
5. Click on Checkout.
6. Enter correct credentials (Username, Password).
7. Click on the Login button.
8. The Login page should be displayed.
### TestCase019 (Register using already existing username or email)
1. Go to Advantage Online Shopping.
2. Click on the profile icon in the header section.
3. Fill in all the details correctly and create the profile.
4. Log out of the profile.
5. Try to register again using the same email and username.
6. After clicking the Register button, a validation message should appear stating that the email or username already exists.
## Module Name - Login
### TestCase020 (Verify login pop-up fields and options)
1. Go to Advantage Online Shopping.
2. Click on the profile icon in the header section.
3. A login pop-up should open.
4. The login pop-up should display the username field, password field, “Remember Me” checkbox, Login button, and “Login with Facebook” option.
### TestCase021 (Login with valid credentials)
1. Go to Advantage Online Shopping.
2. Click on the profile icon in the header section.
3. Enter the correct credentials and click on the Submit button.
4. The user should be redirected to the home page, and the username should be displayed in the profile section.
### TestCase022 (Login with invalid username and password)
1. Go to Advantage Online Shopping.
2. Click on the profile icon in the header section.
3. Enter an invalid username and password.
4. Click on the Submit button.
5. A validation message should be displayed below the respective fields.
### TestCase023 (Login with invalid username and valid password)
1. Go to Advantage Online Shopping.
2. Click on the profile icon in the header section.
3. Enter an invalid username and a correct password.
4. A validation message should be displayed below the username field.
### TestCase024 (Login with a valid username and an invalid password)
1. Go to Advantage Online Shopping.
2. Click on the profile icon in the header section.
3. Enter a correct username and an invalid password.
4. A validation message should be displayed below the password field.
### TestCase025 (Login without entering username and password)
1. Go to Advantage Online Shopping.
2. Click on the profile icon in the header section.
3. Without entering the username and password, click on the Submit button.
4. A validation message should be displayed below both the username and password fields.
## Module Name -  Log Out
### TestCase026 (Logout by confirming Yes on the pop-up)
1. Go to Advantage Online Shopping.
2. Log in to the site.
3. Click on the profile icon in the top-right corner.
4. Click on the Sign Out button from the dropdown.
5. A confirmation pop-up should appear with “Yes” and “No” options.
6. Click on “Yes”.
7. The user should be logged out successfully.
### TestCase027 (Cancel logout by clicking No on the pop-up)
1. Go to Advantage Online Shopping.
2. Log in to the site.
3. Click on the profile icon in the top-right corner.
4. Click on the Sign Out button from the dropdown.
5. A confirmation pop-up should appear with “Yes” and “No” options.
6. Click on “No”.
7. The user should remain on the home page.
### TestCase028 (Verify back navigation after logout does not restore session)
1. Go to Advantage Online Shopping.
2. Log in to the site.
3. Click on the profile icon in the top-right corner.
4. Click on the Sign Out button from the dropdown.
5. A confirmation pop-up should appear with “Yes” and “No” options.
6. Click on “Yes”.
7. While on the Login page after logout, try to forcefully navigate back to the previous page.
8. The user should not be redirected back to the logged-in session.
### TestCase029 (Verify logout in one tab logs out the session in another tab (same browser))
1. Go to Advantage Online Shopping.
2. Log in to the site.
3. Note the profile icon present in the top-right corner.
4. Open another tab in the same browser and log out from that tab.
5. Return to the previous tab and try to perform any activity.
6. The user should be redirected to the Login page.
### TestCase030 (Verify logout in another browser does not affect current browser session)
1. Go to Advantage Online Shopping.
2. Log in to the site.
3. Note the profile icon present in the top-right corner.
4. Open another browser, log in, and log out from that browser.
5. Return to the previous browser and perform any activity.
6. The user should not be redirected to the Login page and should be able to continue the activity.
## Module Name - Dashboard
### TestCase031 (Verify category listing on home page after login)
1. Go to Advantage Online Shopping.
2. Log in with correct credentials.
3. The user should be redirected to the home page.
4. All categories should be listed.
### TestCase032 (Verify newly added category appears on dashboard)
1. Add a new category from the Admin panel.
2. Go to Advantage Online Shopping.
3. Log in with correct credentials.
4. The newly added category should be listed and displayed correctly in the dashboard section.
### TestCase033 (Verify navigation to product listing on selecting a category)
1. Go to Advantage Online Shopping.
2. Log in with correct credentials.
3. Select any category from the home page.
4. The user should be redirected to the product listing page for the selected category.
## Module Name -  Add to Cart
### TestCase034 (Add a product to the cart)
1. Go to Advantage Online Shopping.
2. Log in with correct credentials.
3. Navigate to the product listing section.
4. Select any product.
5. Click on “Add to Cart”.
6. The product should be added, and the updated cart count should be displayed in the cart section.
### TestCase035 (Add a product with selected color to the cart)
1. Go to Advantage Online Shopping.
2. Log in with correct credentials.
3. Navigate to the product listing section.
4. Select any product.
5. Select the product color.
6. Click on “Add to Cart”.
7. The selected color of the product should be displayed correctly on the cart page.
### TestCase036 (Verify correct price of added product in cart)
1. Go to Advantage Online Shopping.
2. Log in with correct credentials.
3. Navigate to the product listing section.
4. Select any product and add it to the cart.
5. The price of the added product in the cart should be correct.
### TestCase037 (Verify out-of-stock product cannot be added to cart)
1. From the Admin portal, reduce the product quantity to 0.
2. Go to Advantage Online Shopping.
3. Log in with correct credentials.
4. Navigate to the product listing section.
5. Select the out-of-stock product.
6. Try to add the product to the cart.
7. The user should not be able to add the product to the cart.
### TestCase038 (Verify multiple products added in different tabs reflect in same cart)
1. Go to Advantage Online Shopping.
2. Log in with correct credentials.
3. Add a product to the cart.
4. Open the site in a different tab.
5. Add a different product to the cart.
6. Both products should be displayed in the cart with the correct price and color.
### TestCase039 (Verify products added from different browsers (same account) reflect in the same cart)
1. Go to Advantage Online Shopping.
2. Log in with correct credentials.
3. Add a product to the cart from one browser.
4. Log in to Advantage Online Shopping in a different browser with the same credentials.
5. Add a different product to the cart.
6. Both the previously added product and the newly added product should be displayed in the cart section.
### TestCase040 (Decrease product quantity in the cart)
1. Go to Advantage Online Shopping.
2. Log in with correct credentials.
3. Add a product to the cart.
4. Decrease the quantity on the cart page.
5. The updated quantity should be reflected correctly in the cart.
### TestCase041 (Increase product quantity in the cart)
1. Go to Advantage Online Shopping.
2. Log in with correct credentials.
3. Add a product to the cart.
4. Increase the quantity on the cart page.
5. The updated quantity should be reflected correctly in the cart.
## Module Name - Order Placement
### TestCase042 (Verify checkout page displays shipping, payment, and order summary)
1. Go to Advantage Online Shopping.
2. Log in with correct credentials.
3. Add a product to the cart.
4. Navigate to the cart page.
5. Click on the Checkout button.
6. The order payment page should display shipping details, payment method, and order summary.
### TestCase043 (Verify shipping details match profile information)
1. Go to Advantage Online Shopping.
2. Log in with correct credentials.
3. Add one product to the cart.
4. Click on the Checkout button.
5. Verify that the name, shipping details, and phone number match those given in the profile.
### TestCase044 (Verify validation on removing mandatory shipping field)
1. Go to Advantage Online Shopping.
2. Log in with correct credentials.
3. Add one product to the cart.
4. Click on the Checkout button.
5. Click on “Edit Shipping Details”.
6. Remove a mandatory field and click on Next.
7. A validation message should be displayed below the respective field.
### TestCase045 (Verify shipping details display correctly with long text input)
1. Go to Advantage Online Shopping.
2. Log in with correct credentials.
3. Add one product to the cart.
4. Click on the Checkout button.
5. Click on “Edit Shipping Details”.
6. Edit the shipping details with long text values.
7. Click on Next.
8. All data should be displayed correctly without breaking the layout.
### TestCase046 (Verify product price on checkout page matches listing price)
1. Go to Advantage Online Shopping.
2. Log in with correct credentials.
3. Add one product to the cart.
4. Click on the Checkout button.
5. Check the product price.
6. The price should match the price listed on the product listing page.
### TestCase047 (Verify total price on checkout matches cart page for multiple products)
1. Go to Advantage Online Shopping.
2. Log in with correct credentials.
3. Add multiple products to the cart.
4. Click on the Checkout button.
5. The total price should match the cart page and should be correct.
### TestCase048 (Verify payment method page fields and options)
1. Go to Advantage Online Shopping.
2. Log in with correct credentials.
3. Add one product to the cart.
4. Click on the Checkout button.
5. Click on the Next button.
6. The payment method page should display various payment gateways, along with fields for card number, CVV, expiry month and year, and cardholder name, plus a “Pay Now” button.
### TestCase049 (Verify validation for invalid card number)
1. Go to Advantage Online Shopping.
2. Log in with correct credentials.
3. Add one product to the cart.
4. Click on the Checkout button.
5. Click on the Next button.
6. Enter an invalid card number.
7. Click on the Pay Now button.
8. A validation message should be displayed for the card number field.
### TestCase050 (Verify validation for multiple invalid payment fields)
1. Go to Advantage Online Shopping.
2. Log in with correct credentials.
3. Add one product to the cart.
4. Click on the Checkout button.
5. Click on the Next button.
6. Enter an invalid card number, CVV, and expiry year, then click on Next.
7. A validation message should be displayed for all the invalid fields.
### TestCase051 (Verify validation when payment fields are left blank)
1. Go to Advantage Online Shopping.
2. Log in with correct credentials.
3. Add one product to the cart.
4. Click on the Checkout button.
5. Click on the Next button.
6. Without filling in the card number, CVV, expiry year, and cardholder name, click on the Submit button.
7. A validation message should be displayed for the blank fields.
### TestCase052 (Verify out-of-stock product cannot be ordered at payment stage)
1. Open the Admin panel.
2. Change the quantity of the product (already added to cart) to 0.
3. Go to Advantage Online Shopping.
4. Log in with correct credentials.
5. Try to place an order for that product on the order payment page.
6. An out-of-stock message should appear, and the user should not be able to place the order.
### TestCase053 (Verify validation for past expiry date on card)
1. Go to Advantage Online Shopping.
2. Log in with correct credentials.
3. Add one product to the cart.
4. Click on the Checkout button.
5. Click on the Next button.
6. Select a past expiry month and year.
7. Click on the Pay Now button.
8. A validation message should be displayed for the invalid expiry date.
### TestCase054 (Verify validation for invalid CVV number)
1. Go to Advantage Online Shopping.
2. Log in with correct credentials.
3. Add one product to the cart.
4. Click on the Checkout button.
5. Click on the Next button.
6. Enter an invalid CVV number.
7. Click on the Pay Now button.
8. A validation message should be displayed for the invalid CVV.
### TestCase055 (Verify validation when cardholder name is missing)
1. Go to Advantage Online Shopping.
2. Log in with correct credentials.
3. Add one product to the cart.
4. Click on the Checkout button.
5. Click on the Next button.
6. Try to place an order without entering the cardholder's name.
7. A validation message should be displayed for the cardholder name field.
### TestCase056 (Verify saved card details are retained for future use)
1. Go to Advantage Online Shopping.
2. Log in with correct credentials.
3. Add one product to the cart.
4. Click on the Checkout button.
5. Click on the Next button.
6. Check the “Save changes in the profile for future use” checkbox.
7. Click on the Pay Now button.
8. When placing an order again, the previously saved card data should be displayed in the fields.
### TestCase057 (Verify edited shipping details persist when navigating back)
1. Go to Advantage Online Shopping.
2. Log in with correct credentials.
3. Add one product to the cart.
4. Click on the Checkout button.
5. Edit the shipping details.
6. Click on the Next button.
7. Click on the “Back to Shipping Details” button.
8. The previously updated shipping details should be present.
### TestCase058 (Verify order placed in another tab invalidates current checkout session)
1. Go to Advantage Online Shopping.
2. Log in with correct credentials.
3. Add one product to the cart.
4. Click on the Checkout button.
5. Click on the Next button.
6. Open another tab in the same browser and go to Advantage Online Shopping.
7. Navigate to the checkout page and place the order using correct card details.
8. Return to the previous tab and try to place the order.
9. The user should not be able to place the order and should be redirected to the home page.
### TestCase059 (Verify cart updates when product is added from another tab)
1. Go to Advantage Online Shopping.
2. Log in with correct credentials.
3. Add one product to the cart.
4. Click on the Checkout button.
5. Click on the Next button.
6. Open another tab in the same browser and log in with correct credentials.
7. Select a product category, select a product and color, and add the product to the cart.
8. Return to the previous tab and refresh the page.
9. The cart product list and price should be updated to reflect the product added in the other tab.
### TestCase060 (Verify order placed in another browser invalidates checkout in original browser)
1. Go to Advantage Online Shopping.
2. Log in with correct credentials.
3. Add one product to the cart.
4. Click on the Checkout button.
5. Click on the Next button.
6. Open another browser and go to Advantage Online Shopping.
7. Log in with the same credentials.
8. Navigate to the checkout page.
9. All product quantities and details should match the previous browser.
10. Place the order using a correct card.
11. Return to the previous browser and try to place the order.
12. The user should not be able to place the order, or should be navigated to an empty cart page.
### TestCase061 (Verify order confirmation (Thank You) page details)
1. Go to Advantage Online Shopping.
2. Log in with correct credentials.
3. Add one product to the cart.
4. Click on the Checkout button.
5. Click on the Next button.
6. Enter a correct card number, expiry date, and CVV.
7. Click on the Pay Now button.
8. The user should be redirected to the Thank You page.
9. Verify that the shipping details, payment method, and order summary are correct.
### TestCase062 (Verify order details in Admin portal match Thank You page)
1. Go to Advantage Online Shopping.
2. Log in with correct credentials.
3. Add one product to the cart.
4. Click on the Checkout button.
5. Click on the Next button.
6. Enter a correct card number, expiry date, and CVV, and place the order.
7. From the Admin portal, check the order details.
8. The order's shipping details, quantity, and other details should match the Thank You page.
### TestCase063 (Verify order confirmation email details)
1. Go to Advantage Online Shopping.
2. Log in with correct credentials.
3. Add one product to the cart.
4. Click on the Checkout button.
5. Click on the Next button.
6. Enter a correct card number, expiry date, and CVV, and place the order.
7. The user should receive a confirmation email containing all the details (shipping, billing, tentative order receipt date, product name with quantity and color, and price breakup).
### TestCase064 (Verify correct amount deducted at payment gateway)
1. Go to Advantage Online Shopping.
2. Log in with correct credentials.
3. Add one product to the cart.
4. Click on the Checkout button.
5. Click on the Next button.
6. Enter a correct card number, expiry date, and CVV, and place the order.
7. After placing the order, verify from the test payment gateway that the correct price was deducted, matching the order summary.
### TestCase065 (Verify transaction decline behavior with a declined card)
1. Go to Advantage Online Shopping.
2. Log in with correct credentials.
3. Add one product to the cart.
4. Click on the Checkout button.
5. Click on the Next button.
6. Enter a card number, expiry date, and CVV that will be declined, and place the order.
7. A pop-up should appear stating that the transaction has been declined and the order cannot be placed.
8. Verify from the payment gateway that no amount was deducted.
### TestCase066 (Verify product quantity reduces in stock after order placement)
1. Go to Advantage Online Shopping.
2. Log in with correct credentials.
3. Add one product to the cart.
4. Click on the Checkout button.
5. Click on the Next button.
6. Enter a correct card number, expiry date, and CVV, and place the order.
7. Check from the store/Admin panel whether the product quantity has reduced accordingly.



# AI Manual Test Cases:-

**Member Name: Pritam Bhar**

Prompt -

Role: -
You are a Senior QA Engineer with expertise in Manual Testing, Functional Testing, Exploratory Testing, Boundary Value Analysis, Negative Testing, and E-commerce Application Testing.
Task:- 
Navigate and analyze the website thoroughly before creating test cases. Understand the actual application flow, fields, validations, navigation, business rules, user journeys, and application behavior.
Context:
Website URL: https://advantageonlineshopping.com/#/

Modules :
1. Registration
2. Login
3. Logout
4. Dashboard
5. Add to Cart
6. Order Placement

Constraints:
- Cover both positive and negative scenarios for each module.
- Include validations for: mandatory fields, invalid data formats (email, phone, password mismatch), duplicate data, boundary conditions, session handling, UI behavior (messages, redirects, masking, counters), and guest vs. logged-in flows where applicable.
- Each module should have a minimum of 5–10 test cases, depending on complexity.
- Do not include Expected Result, Actual Result, Status, or Priority columns.
- Do not use tables — output must be in plain, linear text only.
- Each test case must have a short, descriptive Scenario Name and numbered step-by-step actions, with the verification step included as the last step(s).
- Maintain consistent numbering per module (TestCase 001, 002, 003…).
Output Format:
## Module Name –
### TestCase 001 – (Scenario Name)
1. Step
2. Step
3. Verify ...
### TestCase 002 – (Scenario Name)
1. Step
2. Step
3. Verify ...

# AI-Generated Test Cases 
## Module Name - Registration
### TestCase 001 - Register with valid details
1. Navigate to https://advantageonlineshopping.com/#/
2. Click on the Account icon (top right)
3. Click on the "Register" link
4. Enter a valid First Name, Last Name, Username, Email, Password, Confirm Password, and Phone Number
5. Click the "Register" button
6. Verify the success message/pop-up is displayed
7. Verify user is registered and can log in with the same credentials
### TestCase 002 - Register with already existing username
Navigate to the Registration page
Enter a username that already exists in the system
Fill the remaining mandatory fields with valid data
Click "Register"
Verify error message "Username already exists" (or similar) is displayed
Verify the user is not registered again
### TestCase 003 - Register with mandatory fields left blank
Navigate to the Registration page
Leave First Name/Email/Password blank
Click "Register"
Verify validation error messages appear for each blank mandatory field
Verify registration is not submitted
### TestCase 004 - Register with an invalid email format
Navigate to the Registration page
Enter an invalid email (e.g., "test@@123", "testgmail.com")
Fill other fields with valid data
Click "Register"
Verify validation error "Invalid email format" is shown
### TestCase 005 - Register with mismatched Password and Confirm Password
Navigate to the Registration page
Enter Password as "Test@123" and Confirm Password as "Test@456"
Click "Register"
Verify error message "Passwords do not match" is displayed
### TestCase 006 - Register with weak/short password
Navigate to the Registration page
Enter a password not meeting min length/complexity (e.g., "123")
Click "Register"
Verify the validation message regarding the password policy is displayed
### TestCase 007 - Register with special characters/SQL injection in input fields
Navigate to the Registration page
Enter special characters or SQL injection strings in Name/Username fields (e.g., ' OR 1=1)
Click "Register"
Verify proper validation/error handling (no system crash, no SQL execution)
### TestCase 008 - Field length boundary validation
Navigate to the Registration page
Enter maximum allowed characters in each field (and one character beyond max)
Click "Register"
Verify system restricts input beyond max length or shows error
### TestCase 009 - Phone number field validation
Navigate to the Registration page
Enter alphabets/special characters in the Phone Number field
Click "Register"
Verify validation error is displayed for non-numeric input

## Module Name - Login
### TestCase 001 - Login with valid credentials
Navigate to the homepage
Click Account icon → Sign In
Enter a valid Username and Password
Click the "Login" button
Verify user is redirected to dashboard/home page with username displayed
### TestCase 002 - Login with invalid username
Navigate to the login page
Enter an invalid/non-existent username with any password
Click "Login"
Verify error message "Invalid username or password" is displayed
### TestCase 003 - Login with invalid password
Navigate to the login page
Enter a valid username with an incorrect password
Click "Login"
Verify error message is displayed, and the login fails
### TestCase 004 - Login with blank username/password
Navigate to the login page
Leave Username and/or Password field blank
Click "Login"
Verify the validation message "Field required" is shown
### TestCase 005 - Login with case-sensitive password check
Navigate to the login page
Enter a valid username, enter a password with altered case (e.g., "test@123" vs "TEST@123")
Click "Login"
Verify login fails if the password is case-sensitive
### TestCase 006 - Login with SQL injection / XSS attempt
Navigate to the login page
Enter the SQL injection string in the Username/Password field
Click "Login"
Verify system handles gracefully without exposing data or crashing
### TestCase 007 - Password field masking
Navigate to the login page
Enter the password in the password field
Verify entered password is masked (shown as dots/asterisks)
### TestCase 008 - Login persistence/session check
Log in with valid credentials
Refresh the page
Verify session remains active and user stays logged in

## Module Name - Logout
### TestCase 001 - Logout from active session
Log in with valid credentials
Click on the Account icon/username dropdown
Click "Logout" / "Sign Out"
Verify user is redirected to the homepage/login page
Verify username is no longer displayed in the header
### TestCase 002 - Access restricted pages after logout
Log in and then log out
Try navigating back using the browser back button or directly accessing a logged-in URL (e.g., dashboard)
Verify user is redirected to the login page / restricted page is not accessible
### TestCase 003 - Cart data retention check after logout
Login, add products to the cart
Logout
Log in again with the same credentials
Verify whether cart items persist or are cleared (validate expected behavior)
### TestCase 004 - Logout confirmation/redirection time
Log in with valid credentials
Click Logout
Verify logout action completes within an acceptable time, and no error is thrown

## Module Name - Dashboard
### TestCase 001 - Verify dashboard loads after login
Log in with valid credentials
Verify dashboard/home page loads successfully with all sections (banners, categories, products) visible
### TestCase 002 - Verify product categories are displayed
Navigate to the dashboard
Verify all product categories (e.g., Phones, Laptops, Cameras, etc.) are visible and clickable
### TestCase 003 - Verify category navigation
On the dashboard, click on a specific category (e.g., "Phones")
Verify the user is navigated to the respective category's product listing page
### TestCase 004 - Verify search functionality from the dashboard
On the dashboard, enter a product name in the search bar
Click search/press Enter
Verify relevant search results are displayed
### TestCase 005 - Verify search with invalid/no matching product
Enter an invalid/non-existent product name in the search bar
Click search
Verify "No results found" message is displayed
### TestCase 006 - Verify cart icon and count on dashboard
On the dashboard, verify the cart icon is visible with the correct item count (0 if empty)
### TestCase 007 - Verify top menu/navigation links
On the dashboard, verify all navigation menu links (Home, Account, Cart, etc.) are functional
### TestCase 008 - Verify responsiveness of dashboard
Open the dashboard on different screen resolutions/devices
Verify layout adjusts properly without breaking UI elements
### TestCase 009 - Verify product details on hover/click
On the dashboard, click/hover on a product
Verify product image, name, and price are displayed correctly

## Module Name - Add to Cart
### TestCase 001 - Add a single product to the cart
Login (or as a guest)
Navigate to a product listing/detail page
Click the "Add to Cart" icon for a product
Verify success message "Product Added Successfully" is displayed
Verify cart count increases by 1
### TestCase 002 - Add multiple different products to cart
Navigate to the dashboard
Add 2-3 different products to the cart one by one
Verify cart count updates correctly after each addition
Open the cart and verify all added products are listed
### TestCase 003 - Add the same product multiple times
Add a product to the cart
Add the same product again
Verify quantity is incremented instead of duplicate line entries (validate expected behavior)
### TestCase 004 - Verify product details in cart match selected product
Add a product to the cart
Open cart page
Verify product name, image, price, and quantity match the selected product
### TestCase 005 - Update quantity in cart
Add a product to the cart
On the cart page, increase/decrease quantity using +/- controls
Verify total price updates accordingly
### TestCase 006 - Remove product from cart
Add a product to the cart
Open cart page
Click "Remove"/delete icon for the product
Verify product is removed and cart count/total updates correctly
### TestCase 007 - Add to cart without login (guest user)
Without logging in, navigate to a product
Click "Add to Cart"
Verify the product is successfully added to the cart as a guest
### TestCase 008 - Verify cart total price calculation
Add multiple products with different quantities
Verify subtotal, tax (if any), and total are calculated correctly
### TestCase 009 - Verify "Continue Shopping" and "Proceed to Checkout" buttons in cart
Add product to cart, navigate to cart page
Verify "Continue Shopping" navigates back to product listing
Verify "Proceed to Checkout"/"Buy" button navigates to checkout flow
### TestCase 010 - Add out-of-stock product to cart
Navigate to a product marked out of stock (if available)
Verify "Add to Cart" is disabled or an appropriate message is shown

## Module Name - Order Placement
### TestCase 001 - Place order with valid details (end-to-end)
Log in with valid credentials
Add product(s) to cart
Proceed to checkout
Enter/select a valid shipping address
Select payment method
Confirm and place the order
Verify the order confirmation message/page with the order ID is displayed
### TestCase 002 - Place order without login
As a guest, add the product to the cart
Click "Proceed to Checkout" / "Buy"
Verify user is prompted to log in/register before checkout proceeds
### TestCase 003 - Place order with empty cart
Ensure the cart is empty
Attempt to navigate directly to checkout/order page
Verify appropriate message is shown ("Your cart is empty") and that checkout is blocked
### TestCase 004 - Verify shipping address form validation
Proceed to checkout
Leave mandatory address fields blank
Click "Continue"/"Next"
Verify validation errors are displayed for required fields
### TestCase 005 - Add a new shipping address during checkout
Proceed to checkout
Click "Add new address"
Enter valid address details and save
Verify new address is added and can be selected for the order
### TestCase 006 - Select existing saved address
Proceed to checkout (with previously saved address)
Select an existing saved address from the list
Verify the selected address is correctly applied to the order
### TestCase 007 - Verify order summary before final confirmation
Proceed through checkout to the order review/summary page
Verify product list, quantities, prices, shipping address, and total amount are correctly displayed
### TestCase 008 - Cancel order during checkout process
Start checkout process
Click "Cancel"/navigate away before final confirmation
Verify order is not placed, and the cart items remain unchanged
### TestCase 009 - Verify order confirmation email/notification (if applicable)
Complete order placement successfully
Verify confirmation message is displayed on screen
Verify confirmation email is sent (if feature exists)
### TestCase 010 - Verify order history after placement
Complete an order
Navigate to "My Orders"/Order History section
Verify that the newly placed order appears with the correct details and status
### TestCase 011 - Place order with multiple items and quantities
Add multiple distinct products with varying quantities to the cart
Proceed through checkout and place the order
Verify all items, quantities, and final total are correctly reflected in the order confirmation
### TestCase 012 - Verify back navigation during checkout doesn't duplicate order
Proceed to the final order review step
Click the browser "Back" button, then click "Place Order" again
Verify no duplicate order is created


# My thoughts:-
**What you felt Suitable:-**
1. AI-generated test cases very quickly, which helped reduce the overall test design effort.
2. AI covered the major functional modules and core user workflows of the application.
3. AI included both positive and negative test scenarios.
4. The test cases were structured, readable, and easy to understand.
5. AI helped establish a good baseline test suite for initial testing activities.
6. Common validation and error-handling scenarios were included.
7. AI-assisted test generation improved productivity during the test planning phase.
   
**What you felt Not suitable:-**
1. AI-generated generic test cases without a complete understanding of application-specific business requirements.
2. Some test cases were broad and lacked detailed validation steps.
3. AI did not fully explore business rules, workflows, and application behavior before generating test cases.
4. Edge cases, boundary value scenarios, and real-world user behaviors were limited.
5. Application-specific validations and exceptional user journeys were not adequately covered.
6. Manual review and refinement were still required to improve coverage, remove irrelevant scenarios, and create a production-ready test suite.
7. Certain scenarios appeared repetitive or overlapping in nature.
   
# Final Test Case (AI + Manual):-
## Module Name - Registration
**Source: AI TC001, TC002, TC003, TC004, TC005, TC006, TC007, TC008 | Human TC001, TC002, TC003, TC004, TC005, TC006, TC007, TC008, TC009, TC010, TC011, TC012, TC013, TC014, TC016, TC019**
### TestCase 001 (Verify Registration Page Navigation)
**Classification: Positive**
Launch the application URL.
Click on the Profile icon.
Click on "Create Account".
Verify the Registration page is displayed.
### TestCase 002 (Verify Registration with Valid Details)
**Classification: Positive**
Navigate to the Registration page.
Fill all mandatory fields with valid data.
Accept Terms and Conditions.
Click Register.
Verify the account is created successfully.
### TestCase 003 (Verify Registration with Existing Username or Email)
**Classification: Negative**
Navigate to the Registration page.
Enter an existing username or email.
Fill the remaining fields with valid data.
Click Register.
Verify the validation message is displayed.
### TestCase 004 (Verify Registration Without Mandatory Fields)
**Classification: Negative**
Navigate to the Registration page.
Leave mandatory fields blank.
Verify registration is not allowed.
### TestCase 005 (Verify Username Minimum Length Validation)
**Classification: Negative**
Enter a username with fewer than 5 characters.
Verify the validation message is displayed.
### TestCase 006 (Verify Password Minimum Length Validation)
**Classification: Negative**
Enter a password with fewer than 4 characters.
Verify the validation message is displayed.
### TestCase 007 (Verify Password Maximum Length Validation)
**Classification: Negative**
Enter a password with more than 12 characters.
Verify the validation message is displayed.
### TestCase 008 (Verify Password and Confirm Password Mismatch)
**Classification: Negative**
Enter different values in the Password and Confirm Password fields.
Verify the validation message is displayed.
### TestCase 009 (Verify Password with Only Lowercase Characters)
**Classification: Negative**
Enter the password using only lowercase letters.
Verify the validation message is displayed.
### TestCase 010 (Verify Password with Only Uppercase Characters)
**Classification: Negative**
Enter the password using only uppercase letters.
Verify the validation message is displayed.
### TestCase 011 (Verify Password with Only Numeric Characters)
**Classification: Negative**
Enter the password using only numeric values.
Verify the validation message is displayed.
### TestCase 012 (Verify Phone Number Length Validation)
**Classification: Negative**
Enter a phone number greater than 10 digits.
Verify additional digits are not accepted.
### TestCase 013 (Verify Phone Number Character Validation)
**Classification: Negative**
Enter alphabetic or alphanumeric characters in the phone number field.
Verify input is rejected.
### TestCase 014 (Verify Registration Without Accepting Terms and Conditions)
**Classification: Negative**
Fill all mandatory fields.
Do not select Terms and Conditions.
Verify registration is not allowed.
### TestCase 015 (Verify Navigation to Login Page from Registration Page)
**Classification: Positive**
Open the registration page.
Click "Already Have An Account".
Verify the login page is displayed.
### TestCase 016 (Verify Registration Navigation Through Checkout Flow)
**Classification: Positive**
Add a product to the cart.
Proceed to Checkout.
Click the Registration option.
Verify the Registration page is displayed.

## Module Name - Login
**Source: Human TC020, TC021, TC022, TC023, TC024, TC025**
### TestCase 017 (Verify Login Pop-up Fields and Options)
**Classification: Positive**
Click the Profile icon.
Verify Username, Password, Remember Me checkbox, and Login button are displayed.
### TestCase 018 (Verify Login with Valid Credentials)
**Classification: Positive**
Enter a valid username and password.
Click Login.
Verify the user is logged in successfully.
### TestCase 019 (Verify Login with Invalid Username and Password)
**Classification: Negative**
Enter an invalid username and password.
Click Login.
Verify the validation message is displayed.

### TestCase 020 (Verify Login with Invalid Username)
**Classification: Negative**
Enter an invalid username and a valid password.
Click Login.
Verify the validation message is displayed.
### TestCase 021 (Verify Login with Invalid Password)
**Classification: Negative**
Enter a valid username and an invalid password.
Click Login.
Verify the validation message is displayed.
### TestCase 022 (Verify Login Without Username and Password)
**Classification: Negative**
Leave Username and Password blank.
Click Login.
Verify validation messages are displayed.
### TestCase 023 (Verify Login Through Checkout Flow)
**Classification: Positive**
Add product to cart.
Proceed to Checkout.
Enter valid credentials.
Click Login.
Verify login is successful.

## Module Name - Logout
**Source: Human TC026, TC027, TC028, TC029, TC030**
### TestCase 024 (Verify Successful Logout)
**Classification: Positive**
Log in to the application.
Click Sign Out.
Click Yes on the confirmation pop-up.
Verify user is logged out.
### TestCase 025 (Verify Logout Cancellation)
**Classification: Positive**
Log in to the application.
Click Sign Out.
Click No on confirmation pop-up.
Verify user remains logged in.
### TestCase 026 (Verify Back Navigation After Logout)
**Classification: Negative**
Log in and logout successfully.
Click browser Back button.
Verify logged-in session is not restored.
### TestCase 027 (Verify Logout in One Tab Logs Out Other Tabs)
**Classification: Negative**
Login in two tabs.
Logout from one tab.
Perform action in second tab.
Verify user is redirected to Login page.
### TestCase 028 (Verify Logout in Another Browser Does Not Affect Current Session)
**Classification: Positive**
Login in to Browser A.
Log in and log out in Browser B.
Continue activity in Browser A.
Verify session remains active.

## Module Name - Dashboard
**Source: Human TC031, TC032, TC033 | AI Dashboard TC001, TC002, TC003, TC004, TC005, TC006, TC007**
### TestCase 029 (Verify Dashboard Load After Login)
**Classification: Positive**
Login with valid credentials.
Verify dashboard loads successfully.
### TestCase 030 (Verify Category Listing on Dashboard)
**Classification: Positive**
Login successfully.
Verify all categories are displayed.
### TestCase 031 (Verify Newly Added Category Display)
**Classification: Positive**
Add a category from Admin panel.
Login to application.
Verify category is displayed on dashboard.
### TestCase 032 (Verify Navigation to Product Listing from Category)
**Classification: Positive**
Select any category.
Verify corresponding product listing page opens.
### TestCase 033 (Verify Product Search with Valid Keyword)
**Classification: Positive**
Enter valid product keyword.
Verify matching products are displayed.
### TestCase 034 (Verify Product Search with Invalid Keyword)
**Classification: Negative**
Enter invalid keyword.
Verify no matching result is displayed.
### TestCase 035 (Verify Product Information Display)
**Classification: Positive**
Open product listing page.
Verify product image, name and price are displayed.
### TestCase 036 (Verify Cart Count Display)
**Classification: Positive**
Open the dashboard.
Verify cart count is displayed correctly.

## Module Name - Add To Cart
**Source: AI Add To Cart TC001-TC009 | Human TC034, TC035, TC036, TC037, TC038, TC039, TC040, TC041**
### TestCase 037 (Verify Add Product to Cart)
**Classification: Positive**
Select a product.
Click Add To Cart.
Verify product is added successfully.
### TestCase 038 (Verify Add Product with Selected Color)
**Classification: Positive**
Select product.
Select color.
Click Add To Cart.
Verify selected color is displayed in cart.
### TestCase 039 (Verify Product Price in Cart)
**Classification: Positive**
Add product to cart.
Open cart page.
Verify product price is correct.
### TestCase 040 (Verify Out-of-Stock Product Cannot Be Added)
**Classification: Negative**
Open out-of-stock product.
Click Add To Cart.
Verify product is not added.
### TestCase 041 (Verify Multiple Products Added from Different Tabs)
**Classification: Positive**
Add product in the first tab.
Add another product in the second tab.
Verify both products are displayed in the cart.
### TestCase 042 (Verify Multiple Products Added from Different Browsers)
**Classification: Positive**
Add product from Browser A.
Add another product from Browser B using the same account.
Verify both products appear in the cart.
### TestCase 043 (Verify Decrease Product Quantity)
**Classification: Positive**
Add product to cart.
Decrease quantity.
Verify the updated quantity is displayed.
### TestCase 044 (Verify Increase Product Quantity)
**Classification: Positive**
Add product to cart.
Increase quantity.
Verify the updated quantity is displayed.
### TestCase 045 (Verify Remove Product from Cart)
**Classification: Positive**
Add product to cart.
Remove product.
Verify product is removed successfully.
### TestCase 046 (Verify Empty Cart Message)
**Classification: Positive**
Remove all products from cart.
Verify empty cart message is displayed.
### TestCase 047 (Verify Add Same Product Multiple Times)
**Classification: Positive**
Add same product multiple times.
Verify quantity or cart behavior is updated correctly.
### TestCase 048 (Verify Add Product Without Login)
**Classification: Positive**
Open product page without login.
Add product to cart.
Verify application behavior.

## Module Name - Order Placement
**Source: AI Order Placement TC001-TC010 | Human TC042-TC066**
### TestCase 049 (Verify Checkout Page Details)
**Classification: Positive**
Add product to cart.
Proceed to Checkout.
Verify Shipping Details, Payment Method and Order Summary sections are displayed.
### TestCase 050 (Verify Shipping Details Match User Profile)
**Classification: Positive**
Proceed to Checkout.
Verify shipping details match profile information.
### TestCase 051 (Verify Mandatory Shipping Field Validation)
**Classification: Negative**
Remove mandatory shipping field value.
Click Next.
Verify validation message is displayed.
### TestCase 052 (Verify Long Shipping Details Input)
**Classification: Positive**
Enter long values in shipping fields.
Proceed to next step.
Verify data is displayed correctly.
### TestCase 053 (Verify Product Price on Checkout Page)
**Classification: Positive**
Add product to cart.
Proceed to Checkout.
Verify product price matches listing page.
### TestCase 054 (Verify Total Price for Multiple Products)
**Classification: Positive**
Add multiple products.
Proceed to Checkout.
Verify total amount is correct.
### TestCase 055 (Verify Payment Page Fields and Options)
**Classification: Positive**
Navigate to Payment page.
Verify card fields and Pay Now button are displayed.
### TestCase 056 (Verify Invalid Card Number Validation)
**Classification: Negative**
Enter invalid card number.
Click Pay Now.
Verify validation message.
### TestCase 057 (Verify Multiple Invalid Payment Field Validation)
**Classification: Negative**
Enter invalid Card Number, CVV and Expiry Year.
Click Pay Now.
Verify validation messages.
### TestCase 058 (Verify Blank Payment Field Validation)
**Classification: Negative**
Leave payment fields blank.
Click Pay Now.
Verify validation messages.
### TestCase 059 (Verify Out-of-Stock Product Validation During Checkout)
**Classification: Negative**
Make product out of stock.
Attempt order placement.
Verify order is blocked.
### TestCase 060 (Verify Past Expiry Date Validation)
**Classification: Negative**
Enter expired card details.
Click Pay Now.
Verify the validation message.
### TestCase 061 (Verify Invalid CVV Validation)
**Classification: Negative**
Enter an invalid CVV.
Click Pay Now.
Verify the validation message.
### TestCase 062 (Verify Missing Cardholder Name Validation)
**Classification: Negative**
Leave Cardholder Name blank.
Click Pay Now.
Verify the validation message.
### TestCase 063 (Verify Saved Card Details Persistence)
**Classification: Positive**
Save card details during payment.
Start a new order.
Verify saved card details are displayed.
### TestCase 064 (Verify Edited Shipping Details Persistence)
**Classification: Positive**
Edit shipping details.
Navigate to the payment page.
Return to the shipping page.
Verify changes are retained.
### TestCase 065 (Verify Order Placement from Another Tab)
**Classification: Negative**
Open checkout in two tabs.
Place the order in the first tab.
Attempt order in the second tab.
Verify that duplicate order is prevented.
### TestCase 066 (Verify Cart Updates from Another Tab)
**Classification: Positive**
Add a product in another tab.
Refresh the checkout page.
Verify cart details are updated.
### TestCase 067 (Verify Order Placement from Another Browser)
**Classification: Negative**
Open checkout in two browsers.
Place an order in one browser.
Attempt the order in another browser.
Verify that duplicate order is prevented.
### TestCase 068 (Verify Order Confirmation Page Details)
**Classification: Positive**
Complete successful payment.
Verify the Thank You page is displayed.
Verify shipping details, payment details, and order summary are correct.

