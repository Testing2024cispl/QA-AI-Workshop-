# **Human/AI Test Case Assignment**

Member: Nilanjan Chakraborty  
URL: [https://automationexercise.com/](https://automationexercise.com/)

# Human Thinking Test Cases:-

\*Pre-requisite: The URL opens and works.

**TestCase_001 – New User Registration with Valid Data**

**Test Steps:**

1. Open the Automation Exercise website.
2. Click on Signup / Login.
3. Provide valid name and email address on the respective field.
4. Click on the “Signup” Button.
5. “Enter Account Information” section came.
6. Complete the Required information with the valid data.
7. Click on the “Create Account” Button.
8. Verify that “Account Created\!” message is displayed.
9. Click on the “Continue” Button.
10. Verify that “Logged in as username” is displayed.

**TestCase_002 – New User Registration with Empty Field**

**Test Steps:**

1. Open the Automation Exercise website.
2. Click on Signup / Login.
3. Keep the field empty as it is.
4. Click on the “Signup & Create Account” Button respectively.
5. Verify that mandatory fields validation messages are displayed.

**TestCase_003 – New User Registration with Existing data**

**Test Steps:**

1. Open the Automation Exercise website
2. Click on Signup / Login
3. Provide existing name and email address on the respective field.
4. Click on the “Signup & Create Account” Button respectively.
5. Verify that proper error messages are displayed

**TestCase_004 – New User Registration with invalid data**

**Test Steps:**

1. Open the Automation Exercise website
2. Click on Signup / Login
3. Provide invalid name and email address on the respective field.
4. Click on the “Signup & Create Account” Button respectively.
5. Verify that proper error messages are displayed.

**TestCase_005 – Login with valid Credentials.**

**Test Steps:**

1. Open the Automation Exercise website
2. Click on Signup / Login
3. Enter the registered email.
4. Enter valid password.
5. Click on the “Login” Button.
6. Verify that logged in Successfully and “Logged in as username” is displayed.

**TestCase_006 – Verify the all products page.**

1. Open the Automation Exercise website
2. Click on the “Products” option from the navbar.
3. Verify that Navigate to “All Products” Page.

**TestCase_007 – Verify the product detail page.**

**Test Steps:**

1. Open the Automation Exercise website
2. Click on the “Products” option from the navbar.
3. Navigate to the “All Products” Page.
4. Verify that the product list is available.
5. Click on the “View Product” Button of any product.
6. Verify that the product detail is available.

**TestCase_008 – Verify the search product options.**

**Test Steps:**

1. Open the Automation Exercise website
2. Click on the “Products” option from the navbar.
3. Navigate to the “All Products” Page.
4. Verify that the product list is available.
5. Click on the Search Box named “Search product”.
6. Enter a valid product name in the search box.
7. Verify that the searched product is displayed in the page
8. Click on the Search Box named “Search product” again.
9. Enter an invalid product name in the search box.
10. Verify that none of the product is displayed in the page

**TestCase_009 – add product in cart from featured section.**

**Test Steps:**

1. Open the Automation Exercise website
2. Add to cart any product from the featured section of the home page.
3. Verify that the selected product is available in the cart with maintaining proper quantity & proper Price as per the selection.

**TestCase_010 – add product in cart from all products page.**

**Test Steps:**

1. Open the Automation Exercise website
2. Click on the “Products” option from the navbar.
3. Navigate to the “All Products” Page.
4. Add to cart any product from the All Products page.
5. Verify that the selected product is available in the cart with maintaining proper quantity & proper Price as per the selection.

**TestCase_011 – Verify product details in the cart page.**

**Test Steps:**

1. Open the Automation Exercise website
2. Click on the “View Product” of any products.
3. Select the desired quantity of that product
4. Click on the “Add to cart” button from the Product details page
5. Verify that the selected product, selected quantity and proper price is available.

**TestCase_012 – Order Placement for signed-up users.**

**Test Steps:**

1. Open the Automation Exercise website
2. Click on Signup / Login
3. Enter the registered email.
4. Enter valid password.
5. Click on the “Login” Button.
6. Add to cart the desired products.
7. Go to the cart pages.
8. Click the “Proceed To Checkout” Button.
9. Verify the delivery & billing address details.
10. Verify the products & prices details.
11. Click on the “Place Order” button
12. Keep the field empty as it is for the payment details.
13. Verify that mandatory fields validation messages are displayed.
14. Provide the invalid information of the payment details.
15. Verify that proper error messages are displayed.
16. Provide the valid information of the payment details.
17. Click on the “Pay and Confirm Order” button.
18. Verify that “Order Placed\!” message is displayed.

**TestCase_013 – Order Placement for without signed-up users.**

**Test Steps:**

1. Open the Automation Exercise website.
2. Go to the Features Items section of the home page or all products pages
3. Add to cart the desired products.
4. Click on the “View Cart” Button.
5. Go to the cart pages.
6. Click the “Proceed To Checkout” Button.
7. Click the “Register / Login” options.
8. Complete the registration process.
9. Verify the “Account Created\!” message.
10. Click on the “Continue” Button.
11. Verify that “Logged in as username” is displayed.
12. Go to the cart page again.
13. Click the “Proceed To Checkout” Button.
14. Verify the delivery & billing address details.
15. Verify the products & prices details.
16. Click on the “Place Order” button
17. Keep the field empty as it is for the payment details.
18. Verify that mandatory fields validation messages are displayed.
19. Provide the invalid information of the payment details.
20. Verify that proper error messages are displayed.
21. Provide the valid information of the payment details.
22. Click on the “Pay and Confirm Order” button.
23. Verify that “Order Placed\!” message is displayed.

**TestCase_014 – Download the invoice after purchase and verify the order details.**

**Test Steps:**

1. Open the Automation Exercise website.
2. Complete the order placing Procedure.
3. Verify that “Order Placed\!” message is displayed.
4. Click on the “Download Invoice” button.
5. Download the invoice file.
6. Open the invoice file.
7. Verify that the provided information is accurate.

#

# Prompt:-

**Role:**  
Act as a 5 years experienced Expert Senior QA Engineer with expertise in Manual Testing, Functional Testing for e-commerce websites.

**Task:**  
Generate comprehensive manual test cases for the Automation Exercise website. Cover all major functionalities including User Registration, Login, product pages, product details, Crat page handling, order placing with signed up user and new user both, order process compling, invoice file download and verify.

**Context:**  
The application under test is:  
https://automationexercise.com/  
Automation Exercise is an e-commerce website where users can:  
Register a new account, Login using registered credentials, Browse available products, Search for products, View products detail, add to cart products, Manage order placement from the cart page etc

The objective is to validate the complete end-to-end all possible functional testing, No need to do UI/UX, Security or any other testing.

**Constraints:**  
Include both Positive and Negative test scenarios.  
Include Validation and Error Handling scenarios.  
Consider real-world user behavior and edge cases.  
Avoid duplicate test cases.  
Write test cases in a clear step-by-step format.  
Ensure test cases are suitable for future automation.  
Cover mandatory field validations wherever applicable.  
Include business-critical scenarios such as duplicate Order prevention and unauthorized access checks etc.

**Output Format:**  
Generate test cases using the following format:  
TestCase_AI_ID:- Test Scenario  
Test Steps:

1.
2.
3.

# **AI Manual Test Cases(E-Commerce Functional Testing)**

## **Module 1: User Registration**

---

### **TestCase_AI_001:- Verify successful user registration with valid mandatory details**

**Test Steps:**

1. Open [https://automationexercise.com/](https://automationexercise.com/)
2. Click "Signup / Login".
3. Enter a unique Name.
4. Enter a unique Email Address.
5. Click "Signup".
6. Fill all mandatory registration fields.
7. Click "Create Account".
8. Verify account creation success message.
9. Verify user is logged in.

---

### **TestCase_AI_002:- Verify registration with all available fields**

**Test Steps:**

1. Navigate to Signup page.
2. Enter unique Name and Email.
3. Fill all mandatory and optional fields.
4. Click "Create Account".
5. Verify account is created successfully.

---

### **TestCase_AI_003:- Verify registration with already registered email**

**Test Steps:**

1. Navigate to Signup page.
2. Enter Name.
3. Enter an existing registered Email.
4. Click "Signup".
5. Verify appropriate error message is displayed.

---

### **TestCase_AI_004:- Verify registration with blank Name field**

**Test Steps:**

1. Navigate to Signup page.
2. Leave Name field blank.
3. Enter Email.
4. Click "Signup".
5. Verify validation message.

---

### **TestCase_AI_005:- Verify registration with blank Email field**

**Test Steps:**

1. Navigate to Signup page.
2. Enter Name.
3. Leave Email field blank.
4. Click "Signup".
5. Verify validation message.

---

### **TestCase_AI_006:- Verify registration using invalid email format**

**Test Steps:**

1. Navigate to Signup page.
2. Enter Name.
3. Enter invalid email format.
4. Click "Signup".
5. Verify validation message.

---

### **TestCase_AI_007:- Verify mandatory field validation during account creation**

**Test Steps:**

1. Start registration process.
2. Leave one mandatory field empty.
3. Click "Create Account".
4. Verify field-specific validation message.
5. Repeat for all mandatory fields.

---

### **TestCase_AI_008:- Verify registration with maximum field length values**

**Test Steps:**

1. Enter maximum allowed values in all text fields.
2. Submit registration.
3. Verify account creation behavior.

---

### **TestCase_AI_009:- Verify registration with special characters in Name field**

**Test Steps:**

1. Enter Name containing special characters.
2. Complete registration.
3. Verify system behavior.

---

### **TestCase_AI_010:- Verify successful account deletion after registration**

**Test Steps:**

1. Register a new user.
2. Login successfully.
3. Click "Delete Account".
4. Confirm deletion.
5. Verify account deleted message.

---

# **Module 2: Login Functionality**

---

### **TestCase_AI_011:- Verify successful login with valid credentials**

**Test Steps:**

1. Open Login page.
2. Enter valid Email.
3. Enter valid Password.
4. Click "Login".
5. Verify user is logged in.

---

### **TestCase_AI_012:- Verify login with invalid password**

**Test Steps:**

1. Open Login page.
2. Enter registered Email.
3. Enter incorrect Password.
4. Click Login.
5. Verify error message.

---

### **TestCase_AI_013:- Verify login with invalid email**

**Test Steps:**

1. Open Login page.
2. Enter unregistered Email.
3. Enter Password.
4. Click Login.
5. Verify error message.

---

### **TestCase_AI_014:- Verify login with blank email**

**Test Steps:**

1. Open Login page.
2. Leave Email blank.
3. Enter Password.
4. Click Login.
5. Verify validation.

---

### **TestCase_AI_015:- Verify login with blank password**

**Test Steps:**

1. Open Login page.
2. Enter Email.
3. Leave Password blank.
4. Click Login.
5. Verify validation.

---

### **TestCase_AI_016:- Verify login with both fields blank**

**Test Steps:**

1. Open Login page.
2. Leave Email and Password blank.
3. Click Login.
4. Verify validation messages.

---

### **TestCase_AI_017:- Verify logout functionality**

**Test Steps:**

1. Login successfully.
2. Click Logout.
3. Verify user is logged out.
4. Verify Login page appears.

---

### **TestCase_AI_018:- Verify session termination after logout**

**Test Steps:**

1. Login successfully.
2. Logout.
3. Use browser Back button.
4. Verify user cannot access authenticated pages.

---

# **Module 3: Product Listing Page**

---

### **TestCase_AI_019:- Verify products page loads successfully**

**Test Steps:**

1. Open Products page.
2. Verify products are displayed.

---

### **TestCase_AI_020:- Verify all products contain mandatory information**

**Test Steps:**

1. Open Products page.
2. Verify product image.
3. Verify product name.
4. Verify product price.
5. Verify product action buttons.

---

### **TestCase_AI_021:- Verify pagination or product loading behavior**

**Test Steps:**

1. Navigate through products.
2. Verify products load correctly.
3. Verify no duplicate products.

---

### **TestCase_AI_022:- Verify category filtering functionality**

**Test Steps:**

1. Select a product category.
2. Verify only relevant products appear.

---

### **TestCase_AI_023:- Verify sub-category filtering**

**Test Steps:**

1. Select category.
2. Select sub-category.
3. Verify filtered products.

---

# **Module 4: Product Search**

---

### **TestCase_AI_024:- Verify search using exact product name**

**Test Steps:**

1. Open Products page.
2. Enter exact product name.
3. Click Search.
4. Verify matching products.

---

### **TestCase_AI_025:- Verify partial keyword search**

**Test Steps:**

1. Enter partial keyword.
2. Click Search.
3. Verify related products appear.

---

### **TestCase_AI_026:- Verify search with non-existing product**

**Test Steps:**

1. Enter random keyword.
2. Click Search.
3. Verify no products found message.

---

### **TestCase_AI_027:- Verify search with special characters**

**Test Steps:**

1. Enter special characters.
2. Search.
3. Verify application behavior.

---

### **TestCase_AI_028:- Verify search with empty value**

**Test Steps:**

1. Leave search box empty.
2. Click Search.
3. Verify validation or default behavior.

---

# **Module 5: Product Details**

---

### **TestCase_AI_029:- Verify navigation to product details page**

**Test Steps:**

1. Open Products page.
2. Click View Product.
3. Verify Product Details page opens.

---

### **TestCase_AI_030:- Verify product details information accuracy**

**Test Steps:**

1. Open Product Details page.
2. Verify product name.
3. Verify category.
4. Verify price.
5. Verify availability.
6. Verify description.

---

### **TestCase_AI_031:- Verify quantity update before add to cart**

**Test Steps:**

1. Open Product Details page.
2. Increase quantity.
3. Add to cart.
4. Verify correct quantity in cart.

---

### **TestCase_AI_032:- Verify minimum quantity validation**

**Test Steps:**

1. Enter quantity as 0\.
2. Add to cart.
3. Verify system behavior.

---

# **Module 6: Cart Functionality**

---

### **TestCase_AI_033:- Verify add single product to cart**

**Test Steps:**

1. Select a product.
2. Click Add to Cart.
3. Open Cart.
4. Verify product added.

---

### **TestCase_AI_034:- Verify add multiple products to cart**

**Test Steps:**

1. Add multiple products.
2. Open Cart.
3. Verify all products appear.

---

### **TestCase_AI_035:- Verify add same product multiple times**

**Test Steps:**

1. Add product.
2. Add same product again.
3. Verify quantity update behavior.

---

### **TestCase_AI_036:- Verify remove product from cart**

**Test Steps:**

1. Add product to cart.
2. Remove product.
3. Verify cart becomes empty.

---

### **TestCase_AI_037:- Verify quantity increase in cart**

**Test Steps:**

1. Add product.
2. Increase quantity.
3. Verify total updates correctly.

---

### **TestCase_AI_038:- Verify quantity decrease in cart**

**Test Steps:**

1. Add product.
2. Reduce quantity.
3. Verify total recalculation.

---

### **TestCase_AI_039:- Verify cart persistence after login**

**Test Steps:**

1. Add product as guest.
2. Login.
3. Verify cart items remain.

---

### **TestCase_AI_040:- Verify cart persistence after logout-login**

**Test Steps:**

1. Add products.
2. Logout.
3. Login again.
4. Verify cart data.

---

### **TestCase_AI_041:- Verify cart total calculation**

**Test Steps:**

1. Add multiple products.
2. Calculate expected total.
3. Verify displayed total.

---

### **TestCase_AI_042:- Verify cart with maximum available quantity**

**Test Steps:**

1. Add high quantity.
2. Verify calculation and behavior.

---

# **Module 7: Checkout \- Existing User**

---

### **TestCase_AI_043:- Verify checkout with logged-in user**

**Test Steps:**

1. Login.
2. Add products.
3. Open Cart.
4. Proceed to Checkout.
5. Verify checkout page.

---

### **TestCase_AI_044:- Verify delivery address displayed correctly**

**Test Steps:**

1. Login.
2. Proceed to Checkout.
3. Verify delivery address.

---

### **TestCase_AI_045:- Verify billing address displayed correctly**

**Test Steps:**

1. Proceed to Checkout.
2. Verify billing address information.

---

### **TestCase_AI_046:- Verify placing order with valid payment details**

**Test Steps:**

1. Proceed to Payment page.
2. Enter valid card details.
3. Click Confirm Order.
4. Verify order success.

---

### **TestCase_AI_047:- Verify order placement with blank card name**

**Test Steps:**

1. Proceed to Payment page.
2. Leave card name blank.
3. Submit order.
4. Verify validation.

---

### **TestCase_AI_048:- Verify order placement with blank card number**

**Test Steps:**

1. Leave card number blank.
2. Submit order.
3. Verify validation.

---

### **TestCase_AI_049:- Verify order placement with blank CVC**

**Test Steps:**

1. Leave CVC blank.
2. Submit order.
3. Verify validation.

---

### **TestCase_AI_050:- Verify order placement with blank expiry date**

**Test Steps:**

1. Leave expiry details blank.
2. Submit order.
3. Verify validation.

---

# **Module 8: Checkout \- New User During Purchase**

---

### **TestCase_AI_051:- Verify checkout after registering during purchase flow**

**Test Steps:**

1. Add product to cart.
2. Proceed to Checkout.
3. Register new account.
4. Continue checkout.
5. Complete payment.
6. Verify order success.

---

### **TestCase_AI_052:- Verify cart retention after registration**

**Test Steps:**

1. Add products before registration.
2. Register account.
3. Verify products remain in cart.

---

### **TestCase_AI_053:- Verify checkout after login from checkout flow**

**Test Steps:**

1. Add products.
2. Proceed to Checkout.
3. Login.
4. Complete checkout.
5. Verify order placed.

---

# **Module 9: Order Management & Completion**

---

### **TestCase_AI_054:- Verify order confirmation page**

**Test Steps:**

1. Complete successful order.
2. Verify confirmation message.
3. Verify order completion.

---

### **TestCase_AI_055:- Verify order details consistency**

**Test Steps:**

1. Complete order.
2. Compare cart details.
3. Verify ordered items match.

---

### **TestCase_AI_056:- Verify order amount consistency**

**Test Steps:**

1. Note cart total.
2. Complete order.
3. Verify final amount matches.

---

### **TestCase_AI_057:- Verify order creation only once on single submission**

**Test Steps:**

1. Fill payment details.
2. Click Confirm Order once.
3. Verify only one order created.

---

### **TestCase_AI_058:- Verify duplicate order prevention on multiple clicks**

**Test Steps:**

1. Click Confirm Order repeatedly.
2. Verify only one order is generated.

---

### **TestCase_AI_059:- Verify duplicate order prevention using browser refresh**

**Test Steps:**

1. Complete order.
2. Refresh confirmation page.
3. Verify duplicate order is not created.

---

### **TestCase_AI_060:- Verify duplicate order prevention using browser back button**

**Test Steps:**

1. Complete order.
2. Navigate back.
3. Attempt resubmission.
4. Verify duplicate order not created.

---

# **Module 10: Invoice Download Verification**

---

### **TestCase_AI_061:- Verify invoice download after successful order**

**Test Steps:**

1. Complete order.
2. Click Download Invoice.
3. Verify file download starts.

---

### **TestCase_AI_062:- Verify invoice file is downloaded successfully**

**Test Steps:**

1. Download invoice.
2. Verify file exists in Downloads folder.

---

### **TestCase_AI_063:- Verify invoice file format**

**Test Steps:**

1. Download invoice.
2. Verify file extension matches expected format.

---

### **TestCase_AI_064:- Verify invoice file is not corrupted**

**Test Steps:**

1. Open downloaded invoice.
2. Verify file opens successfully.

---

### **TestCase_AI_065:- Verify invoice contains ordered product information**

**Test Steps:**

1. Download invoice.
2. Verify product names.
3. Verify quantities.
4. Verify prices.

---

### **TestCase_AI_066:- Verify invoice contains correct customer details**

**Test Steps:**

1. Download invoice.
2. Verify customer information.

---

### **TestCase_AI_067:- Verify invoice total amount accuracy**

**Test Steps:**

1. Compare order amount.
2. Compare invoice amount.
3. Verify both match.

---

# **Module 11: Unauthorized Access & Business Critical Scenarios**

---

### **TestCase_AI_068:- Verify guest user cannot directly access checkout URL**

**Test Steps:**

1. Logout.
2. Enter checkout URL directly.
3. Verify login/signup prompt.

---

### **TestCase_AI_069:- Verify deleted user cannot login**

**Test Steps:**

1. Delete account.
2. Attempt login.
3. Verify login fails.

---

### **TestCase_AI_070:- Verify deleted user cannot place orders**

**Test Steps:**

1. Delete account.
2. Attempt checkout.
3. Verify access restriction.

---

### **TestCase_AI_071:- Verify cart remains empty after removing all items**

**Test Steps:**

1. Add products.
2. Remove all products.
3. Verify empty cart message.

---

### **TestCase_AI_072:- Verify checkout is not allowed with empty cart**

**Test Steps:**

1. Ensure cart is empty.
2. Click Checkout.
3. Verify order placement is restricted.

---

### **TestCase_AI_073:- Verify user can continue shopping from cart page**

**Test Steps:**

1. Add product.
2. Open Cart.
3. Click Continue Shopping.
4. Verify navigation to products page.

---

### **TestCase_AI_074:- Verify browser refresh does not duplicate cart items**

**Test Steps:**

1. Add product.
2. Refresh cart page.
3. Verify quantity remains unchanged.

---

### **TestCase_AI_075:- Verify complete end-to-end purchase journey**

**Test Steps:**

1. Register new user.
2. Login.
3. Browse products.
4. View product details.
5. Add products to cart.
6. Verify cart.
7. Checkout.
8. Complete payment.
9. Verify order confirmation.
10. Download invoice.
11. Delete account.
12. Verify successful completion of entire workflow.

**Total Functional Test Cases: 75**  
 **Coverage:** Registration, Login, Logout, Product Listing, Search, Product Details, Cart, Checkout, Payment, Order Completion, Invoice Download, Session Handling, Duplicate Order Prevention, Unauthorized Access, End-to-End User Journey.

# My Thaught:

**What you felt suitable:-**

1. AI is much faster than our human brain.
2. AI provides in a very structured way.
3. AI can think wider than the human brain.
4. AI can Provide large number of test case

**What you felt not suitable:-**

1. AI can generate generic test scenarios.
2. AI can hallucinate and provide Inauthentic data
3. AI can break down simple steps into Multiple steps which it actually can handle with lesser steps in a real time scenario.

**Final verdict:** We Must use AI as our Helping tool with our Common Sense but we cant trust AI Blindly, and We must review the Work before delivering.

Final Test Cases(AI \+ Manual Combined):-

### **TestCase_Final_001:- Verify successful user registration with valid mandatory details**

Test Steps:

1. Open the Automation Exercise website.
2. Click on "Signup / Login".
3. Enter a unique Name and Email Address.
4. Click on "Signup".
5. Fill all mandatory account information.
6. Click on "Create Account".
7. Verify "Account Created\!" message is displayed.
8. Click on "Continue".
9. Verify "Logged in as username" is displayed.

### **TestCase_Final_002:- Verify successful registration using all available fields**

Test Steps:

1. Navigate to the Signup page.
2. Enter a unique Name and Email Address.
3. Fill all mandatory and optional fields.
4. Click on "Create Account".
5. Verify account is created successfully.

### **TestCase_Final_003:- Verify registration with an existing email address**

Test Steps:

1. Open the Signup page.
2. Enter a Name.
3. Enter an already registered Email Address.
4. Click on "Signup".
5. Verify appropriate error messages are displayed.

### **TestCase_Final_004:- Verify mandatory field validation during registration**

Test Steps:

1. Open the Signup page.
2. Leave Name and/or Email fields blank.
3. Click on "Signup".
4. Verify validation message is displayed.
5. Continue registration and leave mandatory fields blank.
6. Click on "Create Account".
7. Verify mandatory field validation messages are displayed.

### **TestCase_Final_005:- Verify registration with invalid email format**

Test Steps:

1. Open the Signup page.
2. Enter a valid Name.
3. Enter an invalid Email Address format.
4. Click on "Signup".
5. Verify validation message is displayed.

### **TestCase_Final_006:- Verify account deletion after successful registration**

Test Steps:

1. Login using a valid account.
2. Click on "Delete Account".
3. Confirm account deletion.
4. Verify "Account Deleted\!" message is displayed.

### **TestCase_Final_007:- Verify login with valid credentials**

Test Steps:

1. Open the Login page.
2. Enter a registered Email Address.
3. Enter a valid Password.
4. Click on "Login".
5. Verify successful login.
6. Verify "Logged in as username" is displayed.

### **TestCase_Final_008:- Verify login with invalid credentials**

Test Steps:

1. Open the Login page.
2. Enter an invalid Email Address and/or Password.
3. Click on "Login".
4. Verify appropriate error messages are displayed.

### **TestCase_Final_009:- Verify mandatory field validation during login**

Test Steps:

1. Open the Login page.
2. Leave Email and/or Password fields blank.
3. Click on "Login".
4. Verify validation message is displayed.

### **TestCase_Final_010:- Verify logout functionality**

Test Steps:

1. Login successfully.
2. Click on "Logout".
3. Verify Login page is displayed.
4. Verify user session is terminated.

### **TestCase_Final_011:- Verify restricted access after logout**

Test Steps:

1. Login successfully.
2. Click on "Logout".
3. Use the browser Back button or access authenticated pages directly.
4. Verify access to protected functionality is restricted.

### **TestCase_Final_012:- Verify deleted account cannot login**

Test Steps:

1. Delete an existing account.
2. Attempt login using deleted account credentials.
3. Verify login is unsuccessful.

### **TestCase_Final_013:- Verify All Products page loads successfully**

Test Steps:

1. Open the website.
2. Click on "Products".
3. Verify All Products page is displayed.
4. Verify product list is available.

### **TestCase_Final_014:- Verify product information on Products page**

Test Steps:

1. Open the Products page.
2. Verify product image is displayed.
3. Verify product name is displayed.
4. Verify product price is displayed.
5. Verify action buttons are available.

### **TestCase_Final_015:- Verify category and sub-category filtering**

Test Steps:

1. Open the Products page.
2. Select a category.
3. Select a sub-category.
4. Verify only relevant products are displayed.

### **TestCase_Final_016:- Verify product search with valid keyword**

Test Steps:

1. Open the Products page.
2. Enter a valid product name or partial keyword.
3. Click on "Search".
4. Verify matching products are displayed.

### **TestCase_Final_017:- Verify product search with invalid keyword**

Test Steps:

1. Open the Products page.
2. Enter an invalid or non-existing product keyword.
3. Click on "Search".
4. Verify no matching products are displayed.

---

### **TestCase_Final_018:- Verify product search with empty search input**

Test Steps:

1. Open the Products page.
2. Leave search field empty.
3. Click on "Search".
4. Verify expected application behavior.

### **TestCase_Final_019:- Verify navigation to Product Details page**

Test Steps:

1. Open the Products page.
2. Click on "View Product" for any product.
3. Verify Product Details page is displayed.

### **TestCase_Final_020:- Verify product details information**

Test Steps:

1. Open a Product Details page.
2. Verify product name.
3. Verify category.
4. Verify availability.
5. Verify description.
6. Verify price.

### **TestCase_Final_021:- Verify quantity selection before adding product to cart**

Test Steps:

1. Open a Product Details page.
2. Change product quantity.
3. Click on "Add to Cart".
4. Open Cart page.
5. Verify selected quantity is added correctly.

**TestCase_Final_022:- Verify invalid quantity handling**

Test Steps:

1. Open a Product Details page.
2. Enter invalid quantity value such as 0\.
3. Attempt to add product to cart.
4. Verify application handles invalid quantity appropriately.

### **TestCase_Final_023:- Verify add product to cart from Home page**

Test Steps:

1. Open the Home page.
2. Add a product from Featured Items section.
3. Open Cart page.
4. Verify product is added successfully.
5. Verify quantity and price are correct.

### **TestCase_Final_024:- Verify add product to cart from Products page**

Test Steps:

1. Open the Products page.
2. Add a product to cart.
3. Open Cart page.
4. Verify product is added successfully.
5. Verify quantity and price are correct.

### **TestCase_Final_025:- Verify adding multiple products to cart**

Test Steps:

1. Add multiple products to cart.
2. Open Cart page.
3. Verify all selected products are displayed.

### **TestCase_Final_026:- Verify adding same product multiple times**

Test Steps:

1. Add a product to cart.
2. Add the same product again.
3. Open Cart page.
4. Verify quantity is updated correctly.

### **TestCase_Final_027:- Verify cart details and total calculation**

Test Steps:

1. Add multiple products with different quantities.
2. Open Cart page.
3. Verify product quantities.
4. Verify unit prices.
5. Verify total amount calculation.

### **TestCase_Final_028:- Verify removing products from cart**

Test Steps:

1. Add products to cart.
2. Remove one or more products.
3. Verify removed products are no longer displayed.
4. Verify cart updates correctly.

### **TestCase_Final_029:- Verify empty cart behavior**

Test Steps:

1. Add products to cart.
2. Remove all products.
3. Verify empty cart message is displayed.
4. Verify checkout is not allowed.

### **TestCase_Final_030:- Verify cart persistence during guest to login flow**

Test Steps:

1. Add products as a guest user.
2. Login or register.
3. Open Cart page.
4. Verify products remain in the cart.

### **TestCase_Final_031:- Verify checkout with logged-in user**

Test Steps:

1. Login with valid credentials.
2. Add products to cart.
3. Open Cart page.
4. Click on "Proceed To Checkout".
5. Verify Checkout page is displayed.

### **TestCase_Final_032:- Verify delivery and billing information during checkout**

Test Steps:

1. Proceed to Checkout.
2. Verify delivery address details.
3. Verify billing address details.
4. Verify order summary details.

### **TestCase_Final_033:- Verify successful order placement with valid payment details**

Test Steps:

1. Proceed to the Payment page.
2. Enter valid payment information.
3. Click on "Pay and Confirm Order".
4. Verify "Order Placed\!" message is displayed.

### **TestCase_Final_034:- Verify payment mandatory field validations**

Test Steps:

1. Proceed to the Payment page.
2. Leave one or more mandatory payment fields blank.
3. Click on "Pay and Confirm Order".
4. Verify validation messages are displayed.

### **TestCase_Final_035:- Verify payment with invalid details**

Test Steps:

1. Proceed to the Payment page.
2. Enter invalid payment details.
3. Click on "Pay and Confirm Order".
4. Verify appropriate validation or error messages are displayed.

### **TestCase_Final_036:- Verify guest user checkout flow**

Test Steps:

1. Add products to cart as a guest user.
2. Click on "Proceed To Checkout".
3. Click on "Register / Login".
4. Complete registration.
5. Return to checkout.
6. Complete payment.
7. Verify order is placed successfully.

### **TestCase_Final_037:- Verify cart retention after registration during checkout**

Test Steps:

1. Add products to cart as a guest user.
2. Start registration from checkout flow.
3. Complete registration.
4. Open Cart page.
5. Verify products remain in the cart.

### **TestCase_Final_038:- Verify direct checkout access without login**

Test Steps:

1. Logout from the application.
2. Access the checkout page directly using the URL.
3. Verify Login/Registration prompt is displayed.

### **TestCase_Final_039:- Verify order confirmation details**

Test Steps:

1. Complete a successful order.
2. Verify order confirmation page is displayed.
3. Verify order completion message is displayed.

### **TestCase_Final_040:- Verify order details consistency**

Test Steps:

1. Note cart products and total amount.
2. Complete order placement.
3. Verify ordered products match cart products.
4. Verify order total matches cart total.

### **TestCase_Final_041:- Verify duplicate order prevention**

Test Steps:

1. Enter valid payment details.
2. Click "Pay and Confirm Order" multiple times.
3. Refresh or resubmit the page.
4. Verify only one order is created.

### **TestCase_Final_042:- Verify invoice download after successful purchase**

Test Steps:

1. Complete order placement.
2. Click on "Download Invoice".
3. Verify invoice file is downloaded successfully.

### **TestCase_Final_043:- Verify invoice file integrity**

Test Steps:

1. Download invoice file.
2. Open downloaded invoice.
3. Verify file opens successfully without corruption.

### TestCase_Final_044:- Verify invoice content accuracy

Test Steps:

1. Download invoice file.
2. Verify customer details.
3. Verify ordered products.
4. Verify quantities and prices.
5. Verify total amount matches placed order.

### **TestCase_Final_045:- Verify complete end-to-end guest purchase journey**

Test Steps:

1. Browse products as a guest user.
2. View product details.
3. Add products to cart.
4. Proceed to Checkout.
5. Register a new account.
6. Complete payment.
7. Verify order confirmation.
8. Download invoice.
9. Verify invoice details.

### **TestCase_Final_046:- Verify complete end-to-end registered user purchase journey**

Test Steps:

1. Login using a registered account.
2. Search and browse products.
3. View product details.
4. Add products to cart.
5. Complete checkout.
6. Place order successfully.
7. Download invoice.
8. Verify order and invoice details.

### **TestCase_Final_047:- Verify complete account lifecycle**

Test Steps:

1. Register a new account.
2. Login successfully.
3. Add products to cart.
4. Complete order placement.
5. Download invoice.
6. Delete account.
7. Attempt login using deleted account.
8. Verify login is unsuccessful.

