Manual Test Cases - Rahul Mathur  [ Manual Cognitive Validation Test Cases]

Module: Authentication & Login  

**TC_AUTH_001: Verify successful opening and UI layout of the Login Functionality**

Precondition: User is on the homepage and is not logged in.

Test Steps:
Navigate to advantageonlineshopping.com.
Click on the User Icon in the top navigation bar.
The Login modal should be displayed successfully.
The modal should contain:
Sign In with “Facebook” - social functionality
“Username” field
“Password” field
“Remember Me” checkbox
“Sign In” button
“Forgot Your Password?” hyperlink

**TC_AUTH_002 : Title: Verify "Sign In with Facebook" Button Redirects to Facebook Login.**

Steps:
Navigate to advantageonlineshopping.com.
Click the User icon.
Click the Sign In with Facebook button.
Expected Result:
User should be redirected to the Facebook authentication/login page.


**TC_AUTH_003 : Title: Verify "Forgot Your Password?" Link Navigates to Password Recovery Page.**

Steps:
Navigate to advantageonlineshopping.com.
Click the User icon.
Click the Forgot Your Password? link.
Expected Result:
The Password Recovery page should be displayed successfully.

**TC_AUTH_004 : Title: Verify Create New Account Button Navigates to Registration Page**

Steps:
Navigate to advantageonlineshopping.com.
Click the User icon.
Click the Create New Account button.
Expected Result:
User should be redirected to the Registration page.
URL should contain /#/register.
"Create Account" heading should be displayed.
The following sections should be visible:
Account Details
Personal Details
Address

**TC_AUTH_005 :  Title: Verify Successful User Registration with Valid Information**

Precondition: User is on the Registration page at advantageonlineshopping.com/#/register.

Steps:
Fill in account credentials — enter a unique Username, valid Email Address, Password, and re-enter the same password in the Confirm Password field.
Fill in personal details — enter First Name, Last Name, and a valid Phone Number, then select a Country.
Fill in address details — enter City, Address, State/Province, and Postal Code.
Check the "I agree to the Conditions of Use and Privacy Notice" checkbox, then click Register.
Expected Result:
Registration completes successfully and the user account is created.
User is automatically logged in, with their Username displayed in the header.

**TC_AUTH_006: Verify "Remember Me" Checkbox Toggle functionality.**

Precondition: The login pop-up is being open.

Steps:
Click the Remember Me checkbox to select it, then click it again to deselect it.
Expected Result:
On the first click, the checkbox displays a checkmark (selected state).
On the second click, the checkmark disappears (unselected state).

**TC_AUTH_006: Verify Successful User Login with Valid user Credentials.**

Precondition: A registered user account exists, and the Login modal is open.

Steps:
Enter a valid Username and corresponding Password, then click Sign In.
Expected Result:
The login modal closes and the user is authenticated successfully.
The user's Username appears in the header navigation bar, confirming the active session.

**TC_AUTH_007: Verify Successful User Logout.**

Precondition: User is actively logged into the application.

Steps:
Click on the Username in the header navigation bar to open the User Menu, then select Sign Out.
Expected Result:
The user session is terminated and the user is logged out successfully.
The Username in the header is replaced by the generic User Icon, and login options become accessible again.

Module: User Registration  

**TC_REG_003: Verify Successful Registration Using Mandatory Fields Only**

Precondition: User is on the registration page (register).

Steps:
Enter a unique Username and a valid Email Address, then set a valid Password and re-enter it in the Confirm Password field.
Leave all optional fields blank (Personal Details and Address sections), check the I Agree to the Conditions of Use and Privacy Notice checkbox, and click Register.
Expected Result:
Registration completes successfully, confirming that the Personal Details and Address sections are optional.
The user is automatically logged in and their Username is displayed in the header.

**TC_REG_004: Verify Registration with Promotional Subscription Preference Enabled**

Precondition: User is on the registration page (register).

Steps:
Fill in all mandatory fields with valid data and check the Receive Exclusive Offers and Promotions from Advantage checkbox.
Check the I Agree to the Conditions of Use and Privacy Notice checkbox and click Register.
Expected Result:
The account is created successfully.
The promotional subscription preference is saved to the user profile, confirming the opt-in was recorded.

**TC_REG_005: Verify Country Dropdown Population and Selection Behavior functionality.**

Precondition: User is on the registration page (register).

Steps:
Click on the Country dropdown and select any country from the list.
Expected Result:
The dropdown expands and displays a list of valid, selectable countries.
The selected country name is correctly populated and displayed within the Country field.

**TC_REG_006: Verify "Already Have an Account?" Link Redirects to Login functionality.**

Precondition: User is on the registration page (Register).

Steps:
Click the Already Have an Account? link.
Expected Result:
The user is redirected to the homepage and the Login modal is automatically displayed, allowing the user to sign in.

**TC_REG_007: Verify Navigation and Notice Banner Visibility in all aspects .**

Precondition: User is on the registration page (register).

Steps:
Observe the breadcrumb trail and the Notice banner displayed on the page.
Click the Home link within the breadcrumb trail.
Expected Result:
The breadcrumb correctly reads HOME / CREATE ACCOUNT, with Create Account visually highlighted as the active page.
A Notice banner reading "This is a demo site. Do not use real data." is clearly visible on the page.
Clicking Home successfully redirects the user back to the homepage without any errors.

**TC_REG_008: Verify Validation Error When Registering with a Duplicate Username**

Precondition: User is on the registration page. An existing account with the username TestUser123 is already registered.

Steps:
Enter TestUser123 in the Username field, fill in all remaining mandatory fields with valid data, and click Register.
Expected Result:
Registration fails and the form is not submitted.
An inline or banner validation error message is displayed, indicating that the Username is already taken.

**TC_REG_009: Verify Validation Error When Registering with a Duplicate Email Address.**

Precondition: User is on the registration page. An existing account with the email test01@mailinator.com is already registered.

Steps:
Enter a unique Username, enter test01@mailinator.com in the Email field, complete all remaining mandatory fields with valid data, and click Register.
Expected Result:
Registration fails and the form is not submitted.
A validation error message is displayed, indicating that the email address is already associated with an existing account.

**TC_REG_010: Verify Validation Errors Are Displayed When All Mandatory Fields Are Left Blank.**

Precondition: User is on the registration page (/#/register).

Steps:
Leave all mandatory fields blank and click Register.
Expected Result:
Registration fails and the form is not submitted.
Inline validation error messages appear beneath each mandatory field, clearly indicating which fields are required.

**TC_REG_011: Verify Validation Error When Password and Confirm Password Do Not Match.**

Precondition: User is on the registration page (/#/register).

Steps:
Enter Password123 in the Password field and Password321 in the Confirm Password field, complete all remaining mandatory fields with valid data, and click Register.
Expected Result:
Registration fails and the form is not submitted.
A validation error message is displayed, indicating that the passwords do not match.

Module: Search, Navigation & E-Commerce Flow and add to cart  

**TC_NAV_001: Verify Global Product Search Functionality.**

Precondition: User is on the homepage.

Steps:
Click the Search icon in the header, type Tablet into the search bar, and submit the query.
Expected Result:
The search results page loads and displays all products matching the keyword "Tablet", confirming the search function returns relevant results.

**TC_NAV_002: Verify Homepage Category Navigation to Product Details Page.**

Precondition: User is on the homepage.

Steps:
Click the Tablets category block and from the listing page, click on the HP ElitePad 1000 G2 Tablet product card.
Expected Result:
The Tablets category listing page opens, displaying the correct product inventory for that category.
The Product Details page loads, accurately showing the item's image, name, description, and price.

**TC_CART_001: Verify Adding an Item to the Shopping Cart.**

Precondition: User is on the Product Details page for the HP ElitePad 1000 G2 Tablet.

Steps:
Select an available Color swatch, set the Quantity field to 1, and click Add to Cart.
Expected Result:
The product is successfully added to the cart.
The cart icon in the header increments by 1, reflecting the newly added item.

**TC_ORDER_001: Verify Initiating Checkout from the Shopping Cart.**

Precondition: At least one item has been added to the shopping cart.

Steps:
Open the Shopping Cart, verify that the Product Name, Quantity, and Price are correct, then click Checkout.
Expected Result:
The cart displays the correct product details and pricing.
The user is redirected to the Order Payment wizard page to proceed with checkout.

**TC_ORDER_002: Verify Shipping Details Auto-Population and Checkout Step Progression**

Precondition: User is logged in and on the Order Payment page.

Steps:
Observe the active tab step and confirm that the shipping information panel is pre-populated with the user's registered profile data.
Verify the Order Summary totals and calculations are accurate, then click Next.
Expected Result:
The Shipping Details tab is highlighted as the active step upon landing on the page.
Shipping information is automatically populated using the user's registration profile data, requiring no manual entry.
Clicking Next successfully advances the wizard to the Payment Method tab.

**TC_ORDER_003: Verify Successful Checkout Completion Using SafePay Payment Method.**

Precondition: User is on the Payment Method step of the checkout wizard.

Steps:
Select the SafePay payment option, enter valid credentials into the SafePay Username and Password fields, and click Pay Now.
Expected Result:
The transaction is processed successfully without any errors.
The Order Confirmation page is displayed, showing a "Thank You" message along with an auto-generated Tracking Number, Order Number, and a full cost summary breakdown.

**TC_ORDER_004: Verify Newly Placed Order Appears in Order History.**

Precondition: User has successfully completed TC_ORDER_003 and has noted the generated Order Number.

Steps:
Click the User Profile Menu in the header, select My Orders, and locate the Order Number from the recently completed transaction.
Expected Result:
The user is redirected to the My Orders history page listing all past purchases.
The newly placed order is present in the list, with the Order Date, Product Name, Quantity, and Total Price exactly matching the details from the completed purchase.

==================================================================================================================================================================

