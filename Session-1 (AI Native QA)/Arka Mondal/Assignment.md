# QA Manual Test Cases

**Member:** Arka Mondal

---

# Human Thinking Test Cases

## TestCases_1

1. Go to Home Page
2. Click on User Icon On Navigation
3. Click on "Create New Account"
4. Leave all mandatory fields blank
5. Click on Register
6. Verify validation messages are displayed or not
7. Enter valid data in the fields
8. Verify validation messages disappear

---

## TestCases_2

1. Go to Home Page
2. Click on User Icon On Navigation
3. Click on "Create New Account"
4. Enter Username
5. Enter invalid email address (abc.com)
6. Verify validation message is displayed
7. Verify email format validation message
8. Enter valid email address
9. Verify validation message disappears

---

## TestCases_3

1. Go to Registration Page
2. Enter a valid unique Username
3. Enter a valid Email Address
4. Enter a valid Password
5. Enter matching Confirm Password
6. Enter valid First Name and Last Name
7. Enter valid Phone Number
8. Enter valid Address Information
9. Accept Terms and Conditions
10. Click REGISTER
11. Verify successful registration

---

## TestCases_4

1. Go to Registration Page
2. Enter valid Username and Email
3. Enter Password = Test@1234
4. Enter Confirm Password = ABC@1234
5. Verify validation message
6. Verify password mismatch error message
7. Verify REGISTER button status

---

## TestCases_5

1. Go to Registration Page
2. Enter all valid mandatory data
3. Leave Terms & Conditions unchecked
4. Scroll to REGISTER button
5. Verify validation message
6. Verify REGISTER button is disabled

---

## TestCases_6

1. Register a user successfully
2. Open Registration Page again
3. Enter same Email Address
4. Complete remaining fields
5. Click REGISTER
6. Verify duplicate email validation message

---

## TestCases_7

1. Register a user successfully
2. Open Registration Page again
3. Enter same Username
4. Complete remaining fields
5. Click REGISTER
6. Verify duplicate username validation message

---

## TestCases_8

1. Navigate to Registration Page
2. Enter valid Username
3. Enter valid Email
4. Enter valid Password
5. Enter valid Personal Details
6. Enter valid Address Details
7. Accept Terms & Conditions
8. Click REGISTER

---

## TestCases_9

1. Login successfully
2. Click Search icon
3. Search for "Tablet"
4. Verify search results

---

## TestCases_10

1. Open Tablet Category
2. Select HP ElitePad 1000 G2 Tablet
3. Verify Product Details Page
4. Verify Product Name, Image, Price and Description

---

## TestCases_11

1. Open Product Details Page
2. Select Product Color
3. Set Quantity = 1
4. Click Add To Cart
5. Verify Product Added Successfully
6. Verify Cart Count Increased

---

## TestCases_12

1. Add Product To Cart
2. Open Cart
3. Verify Product Name
4. Verify Quantity
5. Verify Price
6. Verify Total Amount

---

## TestCases_13

1. Click Checkout
2. Verify Shipping Details Section
3. Verify Registered User Information
4. Verify Address Information

---

## TestCases_14

1. Proceed to Payment Method
2. Select SafePay
3. Enter Valid SafePay Username
4. Enter Valid SafePay Password
5. Click Pay Now
6. Verify Payment Success
7. Verify Order Confirmation Page

---

## TestCases_15

1. Complete Payment Successfully
2. Verify Success Message
3. Verify Tracking Number
4. Verify Order Number
5. Verify Order Summary

---

## TestCases_16

1. Complete an Order
2. Open User Menu
3. Click My Orders
4. Verify Ordered Product Appears
5. Verify Order Number
6. Verify Order Date
7. Verify Product Name
8. Verify Total Price

# QA Manual Test Cases

**Member 1:** Arka Mondal

# AI-Generated Test Cases

## TestCases_001

**Title:** Verify clicking the User icon opens the Login modal

1. Go to advantageonlineshopping.com
2. Click on the User Icon in the navigation bar
3. Verify the Login modal is displayed
4. Verify the modal contains:

   * SIGN IN WITH FACEBOOK button
   * Username field
   * Password field
   * REMEMBER ME checkbox
   * SIGN IN button
   * Forgot your password? link
   * CREATE NEW ACCOUNT button

---

## TestCases_002

**Title:** Verify "SIGN IN WITH FACEBOOK" button is clickable

1. Go to advantageonlineshopping.com
2. Click on the User Icon
3. Click on "SIGN IN WITH FACEBOOK" button
4. Verify the user is redirected to the Facebook OAuth login page

---

## TestCases_003

**Title:** Verify "Forgot your password?" link works

1. Go to advantageonlineshopping.com
2. Click on the User Icon
3. Click on the "Forgot your password?" link
4. Verify the password recovery page is displayed

---

## TestCases_004

**Title:** Verify "REMEMBER ME" checkbox can be checked and unchecked

1. Go to advantageonlineshopping.com
2. Click on the User Icon
3. Click on the REMEMBER ME checkbox
4. Verify the checkbox is checked
5. Click on the checkbox again
6. Verify the checkbox is unchecked

---

## TestCases_005

**Title:** Verify "CREATE NEW ACCOUNT" navigates to the Registration page

1. Go to advantageonlineshopping.com
2. Click on the User Icon
3. Click on "CREATE NEW ACCOUNT" button
4. Verify the URL changes to /#/register
5. Verify the CREATE ACCOUNT heading is visible
6. Verify all sections are displayed:

   * Account Details
   * Personal Details
   * Address

---

## TestCases_006

**Title:** Verify "X" (close) button closes the Login modal

1. Go to advantageonlineshopping.com
2. Click on the User Icon
3. Click on the X (close) icon on the modal
4. Verify the Login modal is closed
5. Verify the homepage is visible

---

## TestCases_007

**Title:** Verify successful registration with all valid fields

1. Go to advantageonlineshopping.com/#/register
2. Enter a unique Username
3. Enter a valid Email
4. Enter a valid Password
5. Enter the same password in Confirm Password
6. Enter First Name
7. Enter Last Name
8. Enter a valid Phone Number
9. Select Country from dropdown
10. Enter City
11. Enter Address
12. Enter State / Province / Region
13. Enter Postal Code
14. Tick "I agree to the Conditions of Use and Privacy Notice"
15. Click REGISTER
16. Verify the user account is created successfully
17. Verify the user is logged in automatically

---

## TestCases_008

**Title:** Verify successful registration with minimum mandatory fields only

1. Go to advantageonlineshopping.com/#/register
2. Enter a unique Username
3. Enter a valid Email
4. Enter a valid Password
5. Enter the same password in Confirm Password
6. Tick "I agree to the Conditions of Use and Privacy Notice"
7. Click REGISTER
8. Verify registration is successful
9. Verify Personal Details and Address are optional

---

## TestCases_009

**Title:** Verify successful registration with "Receive exclusive offers" checked

1. Go to advantageonlineshopping.com/#/register
2. Fill all mandatory fields with valid data
3. Tick "Receive exclusive offers and promotions from Advantage"
4. Tick "I agree to the Conditions of Use and Privacy Notice"
5. Click REGISTER
6. Verify registration is successful and promotional subscription is enabled

---

## TestCases_010

**Title:** Verify Country dropdown contains valid options

1. Go to advantageonlineshopping.com/#/register
2. Click on the Country dropdown
3. Verify a list of countries is displayed
4. Select a country
5. Verify the selected country is displayed in the field

---

## TestCases_011

**Title:** Verify user can log in after successful registration

1. Register a new account using TestCases_007
2. Click on the User Icon
3. Enter the registered Username
4. Enter the Password
5. Click SIGN IN
6. Verify the user is logged in successfully

---

## TestCases_012

**Title:** Verify "ALREADY HAVE AN ACCOUNT?" link navigates back to login

1. Go to advantageonlineshopping.com/#/register
2. Click on "ALREADY HAVE AN ACCOUNT?"
3. Verify the user is redirected to the login page/modal

---

## TestCases_013

**Title:** Verify "HOME" breadcrumb navigates back to homepage

1. Go to advantageonlineshopping.com/#/register
2. Click on the HOME breadcrumb
3. Verify the user is redirected to the homepage

---

## TestCases_014

**Title:** Verify "CREATE ACCOUNT" breadcrumb is visible and highlighted

1. Go to advantageonlineshopping.com/#/register
2. Verify breadcrumb shows HOME / CREATE ACCOUNT
3. Verify CREATE ACCOUNT is highlighted

---

## TestCases_015

**Title:** Verify NOTICE message is displayed

1. Go to advantageonlineshopping.com/#/register
2. Verify NOTICE banner is displayed
3. Verify the text reads:
   "This is a demo site. Do not use real data."

---

## TestCases_016

**Title:** Verify navigation from Homepage to Product Details page

1. Go to advantageonlineshopping.com
2. Verify user is logged in
3. Click TABLETS category
4. Verify Tablets listing page opens
5. Verify HP ElitePad 1000 G2 Tablet is displayed
6. Click the product
7. Verify Product Details page is displayed

---

## TestCases_017

**Title:** Verify adding a product to the cart and initiating checkout

1. Navigate to Product Details page
2. Verify price is displayed
3. Click ADD TO CART
4. Open Shopping Cart
5. Verify cart popup is displayed
6. Verify product and price details
7. Click CHECKOUT
8. Verify ORDER PAYMENT page opens

---

## TestCases_018

**Title:** Verify Shipping Details step during checkout

1. Navigate to ORDER PAYMENT page
2. Verify SHIPPING DETAILS tab is active
3. Verify shipping information is auto-populated
4. Verify ORDER SUMMARY details
5. Click NEXT
6. Verify PAYMENT METHOD tab opens

---

## TestCases_019

**Title:** Verify successful order completion using SafePay

1. Proceed to PAYMENT METHOD
2. Select SafePay
3. Verify username and password fields appear
4. Enter valid credentials
5. Click PAY NOW
6. Verify order confirmation page
7. Verify success message is displayed
8. Verify tracking number and order number are generated
9. Verify receipt details are correct

---

## TestCases_020

**Title:** Verify newly placed order is recorded in My Orders

1. Complete a purchase
2. Copy the Order Number
3. Click User Profile
4. Click My Orders
5. Verify navigation to MY ORDERS page
6. Search for the Order Number
7. Verify Order Date, Product Name, Quantity and Total Price match the purchase

**QA Manual Test Cases**

**Member 1: Arka Mondal**

Website: advantageonlineshopping.com

**Final Test Cases (AI + Manual Combined, Automation Ready)**

**TestCase_001**
Title: Verify successful user registration with valid data

Precondition:
User is on Registration Page.

Steps:

1. Navigate to advantageonlineshopping.com/#/register
2. Enter a unique Username.
3. Enter a valid Email Address.
4. Enter a valid Password.
5. Enter the same Password in Confirm Password field.
6. Enter First Name and Last Name.
7. Enter Phone Number.
8. Select Country.
9. Enter City.
10. Enter Address.
11. Enter State/Province.
12. Enter Postal Code.
13. Accept Terms and Conditions.
14. Click REGISTER.

Expected Result:

1. Registration should be completed successfully.
2. User should be automatically logged in.
3. Username should appear in the header section.

---

**TestCase_002**
Title: Verify duplicate username validation

Precondition:
A user account already exists.

Steps:

1. Open Registration page.
2. Enter an existing Username.
3. Fill all remaining mandatory fields.
4. Click REGISTER.

Expected Result:

1. Duplicate Username validation message should be displayed.
2. Registration should not be completed.

---

**TestCase_003**
Title: Verify duplicate email validation

Precondition:
A user account already exists.

Steps:

1. Open Registration page.
2. Enter a unique Username.
3. Enter an already registered Email Address.
4. Fill remaining fields.
5. Click REGISTER.

Expected Result:

1. Duplicate Email validation should appear.
2. Registration should fail.

---

**TestCase_004**
Title: Verify successful login

Precondition:
User account exists.

Steps:

1. Click User Icon.
2. Enter valid Username.
3. Enter valid Password.
4. Click SIGN IN.

Expected Result:

1. User should be logged in successfully.
2. Username should be displayed in the header.

---

**TestCase_005**
Title: Verify product search functionality

Precondition:
User is logged in.

Steps:

1. Click Search icon.
2. Search for "Tablet".
3. Submit search.

Expected Result:

1. Relevant Tablet products should be displayed.

---

**TestCase_006**
Title: Verify navigation to product details page

Steps:

1. Open Tablet category.
2. Select HP ElitePad 1000 G2 Tablet.

Expected Result:

1. Product details page should open.
2. Product image, name, description and price should be displayed.

---

**TestCase_007**
Title: Verify add product to cart

Steps:

1. Open product details page.
2. Select Color.
3. Select Quantity = 1.
4. Click ADD TO CART.

Expected Result:

1. Product should be added successfully.
2. Cart count should increase by 1.

---

**TestCase_008**
Title: Verify checkout process

Steps:

1. Open Cart.
2. Verify Product Name.
3. Verify Quantity.
4. Verify Total Price.
5. Click CHECKOUT.

Expected Result:

1. User should be redirected to Order Payment page.

---

**TestCase_009**
Title: Verify shipping details during checkout

Steps:

1. Navigate to Order Payment page.
2. Verify Shipping Details section.

Expected Result:

1. User information should be displayed correctly.
2. Address information should match profile data.
3. Order Summary should display correct amount.

---

**TestCase_010**
Title: Verify successful SafePay payment

Steps:

1. Proceed to Payment Method step.
2. Select SafePay.
3. Enter valid SafePay Username.
4. Enter valid SafePay Password.
5. Click PAY NOW.

Expected Result:

1. Payment should be successful.
2. Order Confirmation page should be displayed.

---

**TestCase_011**
Title: Verify order confirmation details

Steps:

1. Complete successful payment.

Expected Result:

1. Thank You message should be displayed.
2. Tracking Number should be generated.
3. Order Number should be generated.
4. Order Summary should display correct information.

---

**TestCase_012**
Title: Verify order appears in My Orders

Steps:

1. Complete purchase.
2. Open User Menu.
3. Click My Orders.

Expected Result:

1. Newly created order should be listed.
2. Product Name should match purchased item.
3. Quantity should match.
4. Order Number should match confirmation page.
5. Total Price should match purchased amount.

---

**TestCase_013**
Title: Verify logout functionality

Steps:

1. Click User Menu.
2. Click Sign Out.

Expected Result:

1. User should be logged out successfully.
2. Login option should be visible again.

---

**TestCase_014**
Title: Verify registration without mandatory fields

Steps:

1. Open Registration page.
2. Leave mandatory fields blank.
3. Click REGISTER.

Expected Result:

1. Validation messages should be displayed.
2. Registration should not proceed.

---

**TestCase_015**
Title: Verify password mismatch validation

Steps:

1. Enter Password.
2. Enter different Confirm Password.
3. Click REGISTER.
   
Expected Result:

1. Password mismatch validation message should appear.
2. Registration should fail.

**Your Thoughts**
---
What I Felt Suitable
AI generated valid positive registration scenarios.
AI covered navigation and E2E flow effectively.
AI helped generate structured test cases quickly.
AI improved coverage of user journey testing.
---
What I Felt Not Suitable
Some test cases were repetitive.
Expected results were missing in several scenarios.
Some test cases were not automation-ready.
Duplicate scenarios required manual refinement.
Final Test Case Approach

I combined Human Thinking Test Cases with AI Generated Test Cases and refined them into automation-ready scenarios by adding Preconditions, Steps, and Expected Results. This approach improved coverage, readability, maintainability, and suitability for future Selenium automation.





