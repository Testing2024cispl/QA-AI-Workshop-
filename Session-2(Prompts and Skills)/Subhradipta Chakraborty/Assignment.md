QA Manual Test Cases:-

Project: DemoBlaze Testing
Application: https://www.demoblaze.com/
Tester: Subhradipta Chakraborty

Human Thinking Test Cases

TestCases_001:- Home page checking
Open https://www.demoblaze.com/
Verify by default, it is “Home” page
Verify all the menus i.e Home, Contact, About us, cart, Login, About us
Verify all the menus are clickable
Verify the filters i.e phone, mobile,monitors
Verify after clicking any specific filter, it is showing specific product according to that


TestCases_002:- Product page
 Click any product.
Verify it is product details page
Verify the image, price , description according to product
Verify the add to cart button

TestCases_003:- Cart page
Verify proper message if no product is added
Verify product(s) details on cart page which are added
Verify delete button
Verify total price
Verify Place order button

TestCases_004:- Place order 
Open the pop up
Fill up name, country, city, credit card, month, year
Check the purchase button functionality
Verify the order details
Verify purchase functionality with all blank fields


TestCases_005:- Login
Verify with valid credentials
Verify with wrong username/password
Verify with blank fields

TestCases_006:- Sign up
Verify with blank fields
Verify with correct username & password
Verify with duplicate credentials


AI Manual Test Cases:- 

Project: DemoBlaze Testing
Application: https://www.demoblaze.com/
Tester: Subhradipta Chakraborty
Home Page
TestCases_001: Verify Home Page Loads Successfully
Open https://www.demoblaze.com/
Verify the homepage loads successfully.
Verify the logo is displayed.
Verify navigation menu is visible.
Verify product categories are displayed.
Verify product listings are displayed.
Suitable 

TestCases_002: Verify Navigation Menu Links
Open the website.
Click Home.
Verify user is redirected to Home page.
Click Contact.
Verify Contact popup opens.
Click About Us.
Verify About Us popup opens.
Click Cart.
Verify Cart page opens.
Suitable 

Sign Up Module
TestCases_003: Verify Successful User Registration
Open website.
Click Sign Up.
Enter unique username.
Enter valid password.
Click Sign Up.
Verify success message is displayed.
Suitable 

TestCases_004: Verify Registration with Existing Username
Click Sign Up.
Enter existing username.
Enter password.
Click Sign Up.
Verify error message appears.
Suitable 

TestCases_005: Verify Registration with Blank Username
Click Sign Up.
Leave username blank.
Enter password.
Click Sign Up.
Verify validation message appears.
Suitable 

TestCases_006: Verify Registration with Blank Password
Click Sign Up.
Enter username.
Leave password blank.
Click Sign Up.
Verify validation message appears.
Suitable 

Login Module
TestCases_007: Verify Login with Valid Credentials
Click Log In.
Enter valid username.
Enter valid password.
Click Log In.
Verify successful login.
Verify Welcome Username is displayed.
Suitable 

TestCases_008: Verify Login with Invalid Credentials
Click Log In.
Enter invalid username/password.
Click Log In.
Verify error message appears.
Suitable 
TestCases_009: Verify Logout Functionality
Login successfully.
Click Log Out.
Verify user is logged out.
Verify Log In button appears.
Suitable 

Product Module
TestCases_010: Verify Product Details Page
Click any product.
Verify product details page opens.
Verify product image is displayed.
Verify product title is displayed.
Verify product price is displayed.
Verify product description is displayed.
Suitable 

TestCases_011: Verify Product Image Visibility
Open product details page.
Verify image loads properly.
Verify image is not broken.
Suitable 

Category Module
TestCases_012: Verify Phones Category Filter
Click Phones category.
Verify only phone products appear.
Suitable 

TestCases_013: Verify Laptops Category Filter
Click Laptops category.
Verify only laptop products appear.
Suitable 

TestCases_014: Verify Monitors Category Filter
Click Monitors category.
Verify only monitor products appear.
Suitable 

Cart Module
TestCases_015: Verify Add Product to Cart
Open product details page.
Click Add to Cart.
Accept confirmation alert.
Open Cart page.
Verify product is added.
Suitable 

TestCases_016: Verify Multiple Products in Cart
Add multiple products.
Open Cart page.
Verify all products are displayed.
Suitable 

TestCases_017: Verify Delete Product from Cart
Add product to cart.
Open Cart page.
Click Delete.
Verify product is removed.
Suitable 

TestCases_018: Verify Cart Total Calculation
Add multiple products.
Open Cart page.
Verify total amount equals sum of product prices.
Suitable 

Checkout / Place Order Module
TestCases_019: Verify Place Order Popup
Add product to cart.
Open Cart.
Click Place Order.
Verify order popup appears.
Suitable 

TestCases_020: Verify Successful Order Placement
Open Place Order popup.
Enter Name.
Enter Country.
Enter City.
Enter Credit Card.
Enter Month.
Enter Year.
Click Purchase.
Verify success message appears.
Verify order ID is generated.
Suitable

TestCases_021: Verify Purchase with Empty Mandatory Fields
Open Place Order popup.
Leave mandatory fields blank.
Click Purchase.
Verify validation message appears.
Suitable 

Contact Module
TestCases_022: Verify Contact Form Submission
Click Contact.
Enter email.
Enter name.
Enter message.
Click Send Message.
Verify success alert appears.
Suitable 

About Us Module
TestCases_023: Verify About Us Popup
Click About Us.
Verify popup opens.
Verify video is displayed.
Verify popup closes successfully.
Suitable 

UI & Responsive Testing
TestCases_024: Verify Website Layout
Open website.
Verify alignment of all elements.
Verify no overlapping elements.
Suitable 

TestCases_025: Verify Responsive Design
Open website on mobile viewport.
Verify menu is accessible.
Verify products display correctly.
Suitable 





Final Test Case:-
Project: DemoBlaze Testing
Application: https://www.demoblaze.com/
Tester: Subhradipta Chakraborty

Module 1: Home Page & Navigation
TC_001: Verify Home Page Loads Successfully
Steps:
Open https://www.demoblaze.com/
Observe the landing page.
Expected Result:
Homepage loads successfully.
Logo is displayed.
Home menu is selected by default.
Product listings are visible.

TC_002: Verify Navigation Menu Availability
Steps:
Open homepage.
Verify presence of Home, Contact, About Us, Cart, Log In, and Sign Up menus.
Expected Result:
All navigation menus are visible and enabled.

TC_003: Verify Navigation Menu Functionality
Steps:
Click Home.
Click Contact.
Click About Us.
Click Cart.
Expected Result:
Home redirects to homepage.
Contact popup opens.
About Us popup opens.
Cart page opens successfully.

Module 2: Category Filters
TC_004: Verify Phones Category Filter
Steps:
Click "Phones".
Expected Result:
Only phone products are displayed.

TC_005: Verify Laptops Category Filter
Steps:
Click "Laptops".
Expected Result:
Only laptop products are displayed.

TC_006: Verify Monitors Category Filter
Steps:
Click "Monitors".
Expected Result:
Only monitor products are displayed.

Module 3: Product Details
TC_007: Verify Product Details Page
Steps:
Click any product from homepage.
Expected Result:
Product detail page opens.
Product name is displayed.
Product image is displayed.
Product price is displayed.
Product description is displayed.

TC_008: Verify Product Image Rendering
Steps:
Open any product page.
Expected Result:
Product image loads successfully.
No broken image is displayed.

TC_009: Verify Add To Cart Button Availability
Steps:
Open any product page.
Expected Result:
Add to Cart button is visible and enabled.

Module 4: Cart Functionality
TC_010: Verify Empty Cart Behavior
Steps:
Open Cart without adding any product.
Expected Result:
Cart page opens successfully.
No products are displayed.
Total amount displays zero or remains empty.

TC_011: Verify Add Product To Cart
Steps:
Open product page.
Click Add to Cart.
Accept confirmation alert.
Open Cart page.
Expected Result:
Selected product is displayed in Cart.

TC_012: Verify Multiple Products In Cart
Steps:
Add multiple products.
Open Cart page.
Expected Result:
All added products are displayed.

TC_013: Verify Cart Total Calculation
Steps:
Add multiple products.
Open Cart page.
Expected Result:
Total amount equals sum of all product prices.

TC_014: Verify Delete Product From Cart
Steps:
Add product to Cart.
Click Delete.
Expected Result:
Product is removed from Cart.
Total amount updates accordingly.

Module 5: Place Order
TC_015: Verify Place Order Popup
Precondition: Product exists in Cart.
Steps:
Open Cart.
Click Place Order.
Expected Result:
Place Order popup appears.

TC_016: Verify Successful Purchase
Precondition: Product exists in Cart.
Steps:
Open Place Order popup.
Enter Name.
Enter Country.
Enter City.
Enter Credit Card.
Enter Month.
Enter Year.
Click Purchase.
Expected Result:
Purchase completes successfully.
Confirmation popup appears.
Order ID is generated.
Purchase details are displayed.

TC_017: Verify Purchase With Blank Fields
Precondition: Product exists in Cart.
Steps:
Open Place Order popup.
Leave all fields blank.
Click Purchase.
Expected Result:
Application behavior should be validated.
Order should not be processed or appropriate validation should be displayed.

Module 6: Login
TC_018: Verify Login With Valid Credentials
Steps:
Click Log In.
Enter valid username.
Enter valid password.
Click Log In.
Expected Result:
User logs in successfully.
Welcome Username message is displayed.

TC_019: Verify Login With Invalid Credentials
Steps:
Click Log In.
Enter invalid username/password.
Click Log In.
Expected Result:
Error message is displayed.
User remains logged out.

TC_020: Verify Login With Blank Credentials
Steps:
Click Log In.
Leave username blank.
Leave password blank.
Click Log In.
Expected Result:
Appropriate validation/error message is displayed.

TC_021: Verify Logout Functionality
Precondition: User logged in.
Steps:
Click Log Out.
Expected Result:
User is logged out successfully.
Log In menu becomes visible.

Module 7: Sign Up
TC_022: Verify Successful User Registration
Steps:
Click Sign Up.
Enter unique username.
Enter password.
Click Sign Up.
Expected Result:
Registration success message is displayed.

TC_023: Verify Registration With Duplicate Username
Steps:
Click Sign Up.
Enter existing username.
Enter password.
Click Sign Up.
Expected Result:
Duplicate user error message is displayed.

TC_024: Verify Registration With Blank Fields
Steps:
Click Sign Up.
Leave username and password blank.
Click Sign Up.
Expected Result:
Validation/error message is displayed.

Module 8: Contact Us
TC_025: Verify Contact Form Submission
Steps:
Click Contact.
Enter Email.
Enter Name.
Enter Message.
Click Send Message.
Expected Result:
Success alert/message is displayed.

Module 9: About Us
TC_026: Verify About Us Popup
Steps:
Click About Us.
Expected Result:
About Us popup opens successfully.
Video is displayed.

TC_027: Verify About Us Popup Close
Steps:
Open About Us popup.
Click Close.
Expected Result:
Popup closes successfully.

Module 10: UI & Responsive Testing
TC_028: Verify UI Layout
Steps:
Open homepage.
Expected Result:
Elements are aligned properly.
No overlap or broken layout is observed.

TC_029: Verify Responsive Design
Steps:
Open application on mobile viewport.
Navigate through pages.
Expected Result:
Layout adjusts properly.
Menus and products remain usable.


===========================================================Session 2===========================================================
** QA Test Case Design & Website Testing Specification**

## Skill Name
QA Test Case Design & Website Functional Testing

## Tester
**Subhradipta Chakraborty**

---

# Purpose

This skill defines the standard process for performing comprehensive manual testing of a web application by analyzing requirements, identifying user workflows, designing detailed test cases, and validating website functionality.

The objective is to ensure that every major feature of a web application behaves correctly from an end-user perspective while maintaining usability, reliability, and functional quality.

---

# Target Application

DemoBlaze

https://www.demoblaze.com/

---

# Scope

This skill covers complete functional testing of an e-commerce web application including:

- Homepage verification
- Navigation testing
- Product category filtering
- Product detail validation
- Shopping cart functionality
- Order placement
- User authentication
- User registration
- Contact module
- About Us module
- UI testing
- Responsive testing

---

# Testing Objectives

The testing process validates:

- Website accessibility
- Navigation correctness
- Functional behavior
- Business workflow
- User interaction
- Data validation
- UI consistency
- Responsive behavior
- Error handling
- Positive and negative scenarios

---

# Modules Covered

## Module 1 — Home Page & Navigation

### Test Coverage

- Homepage loads successfully
- Logo visibility
- Default Home selection
- Product list visibility
- Navigation menu availability
- Navigation menu functionality
- Contact popup
- About Us popup
- Cart navigation

---

## Module 2 — Product Categories

### Test Coverage

- Phones filter
- Laptops filter
- Monitors filter

Validation includes:

- Correct products displayed
- Incorrect category products hidden

---

## Module 3 — Product Details

### Test Coverage

- Product details page
- Product image rendering
- Product price
- Product description
- Add To Cart button availability

---

## Module 4 — Shopping Cart

### Test Coverage

- Empty cart
- Single product addition
- Multiple product addition
- Cart total calculation
- Delete product
- Total update after deletion

---

## Module 5 — Place Order

### Test Coverage

- Place Order popup
- Successful purchase
- Purchase confirmation
- Order ID generation
- Purchase with blank fields
- Validation handling

---

## Module 6 — Login

### Test Coverage

Positive Scenario

- Valid username
- Valid password

Negative Scenario

- Invalid credentials
- Blank credentials

Additional

- Logout functionality

---

## Module 7 — Sign Up

### Test Coverage

- Successful registration
- Duplicate username
- Blank username
- Blank password

---

## Module 8 — Contact Us

### Test Coverage

- Contact popup
- Email entry
- Name entry
- Message entry
- Successful submission

---

## Module 9 — About Us

### Test Coverage

- About Us popup
- Video display
- Popup close functionality

---

## Module 10 — UI & Responsive Testing

### Test Coverage

UI

- Alignment
- Layout consistency
- Broken elements
- Visual validation

Responsive

- Mobile viewport
- Navigation usability
- Product visibility
- Layout adaptation

---

# Testing Types Covered

## Functional Testing

Verification of all application features against expected behavior.

Examples

- Login
- Signup
- Cart
- Purchase
- Product filtering

---

## UI Testing

Verification of

- Alignment
- Buttons
- Images
- Fonts
- Menus
- Popups

---

## Validation Testing

Verification of

- Blank inputs
- Invalid credentials
- Duplicate users
- Required fields

---

## Navigation Testing

Verification of

- Internal links
- Menus
- Page transitions
- Popups

---

## End-to-End Testing

Complete user journey including

Homepage

↓

Browse Product

↓

View Details

↓

Add To Cart

↓

Place Order

↓

Purchase Confirmation

---

## Responsive Testing

Validation across

- Mobile
- Tablet
- Desktop

---

## Regression Testing

Re-execution of all major test cases after application updates.

---

# Test Design Approach

The test suite follows industry-standard manual testing practices.

Each test case contains

- Test Case ID
- Module
- Objective
- Preconditions
- Test Steps
- Expected Result

---

# Test Case Coverage Summary

| Module | Test Cases |
|----------|-----------|
| Home & Navigation | 3 |
| Categories | 3 |
| Product Details | 3 |
| Cart | 5 |
| Place Order | 3 |
| Login | 4 |
| Sign Up | 3 |
| Contact | 1 |
| About Us | 2 |
| UI & Responsive | 2 |

**Total Test Cases:** **29**

---

# Positive Scenarios Covered

- Successful login
- Successful signup
- Successful purchase
- Product addition
- Category filtering
- Contact form submission

---

# Negative Scenarios Covered

- Invalid login
- Blank login
- Duplicate signup
- Blank signup
- Blank purchase form

---

# Validation Scenarios Covered

- Mandatory fields
- User authentication
- Duplicate account validation
- Purchase validation

---

# Deliverables

This testing skill produces:

- Functional Test Cases
- Manual Test Execution
- Bug Reports
- Validation Reports
- UI Review
- Regression Checklist
- Test Summary Report

---

# Expected Outcome

After executing this testing specification, the application should demonstrate:

- Stable navigation
- Correct product filtering
- Accurate cart calculations
- Reliable order processing
- Secure authentication
- Proper validation handling
- Responsive user interface
- Consistent user experience

---

# Best Practices Followed

- Requirement-based testing
- User-centric scenarios
- Positive and negative testing
- Boundary validation
- Functional verification
- UI consistency checks
- Reusable test design
- Modular test organization
- Clear expected results
- Industry-standard documentation

---

# Conclusion

This skill provides a structured methodology for designing and executing comprehensive manual test cases for an e-commerce web application. It emphasizes complete functional coverage, validation testing, usability verification, and end-to-end workflow testing while following standard QA documentation practices.
