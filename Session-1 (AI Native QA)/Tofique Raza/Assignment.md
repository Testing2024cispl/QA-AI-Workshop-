**QA Manual Test Cases:-**
**Member:-Tofique RAZA**
Query/Test cases:-  https://demowebshop.tricentis.com/

**Human Thinking Test Cases**

TC_DWT_001:-
Verify successful user registration
1.Navigate to the ""https://demowebshop.tricentis.com/""
2.Click the ""Register"" link.
3. Fill in all required fields with valid data (Gender,First name, Last name, Email, Password, Confirm password).
4. Click the ""Register"" button.
5. Verify the ""Your registration completed"" message.

TC_DWT_002:-
Verify user login with valid credentials
1. Navigate to the ""https://demowebshop.tricentis.com/""
2. Click the ""Log in"" link.
3. Enter valid ""Email"" and 'Password'.
4. Click the 'Remember me?' checkbox.
5. Click the ""Log in"" button.
6. Verify successful login.

TC_DWT_003:-
Verify login with invalid password
1. Navigate to the ""https://demowebshop.tricentis.com/""
2. Click the ""Log in"" link.
3. Enter valid ""Email"" and an invalid 'Password'.
4. Click the ""Log in"" button.
5. Verify the ""The credentials provided are incorrect"" message.

TC_DWT_004:-
Verify that the initial shopping cart shows zero items.
1. Navigate to the ""https://demowebshop.tricentis.com/""
2. hover on the ""Shopping cart"".
3. verify that ""You have no items in your shopping cart."" message.

TC_DWT_005:-
Verify search functionality with a valid product name
1. Navigate to the ""https://demowebshop.tricentis.com/""
2. Enter a valid product name into the search bar.
3. Click the ""Search"" button.
4. Verify that the search results page displays the relevant product.

TC_DWT_006:-
Verify search functionality with an invalid product name
1. Enter an invalid product name or special charecter into the search bar.
2. Click the 'Search' button.
3. Verify the ""No products were found that matched your criteria."" message.

TC_DWT_007:-
Verify adding a product to the shopping cart
1. Navigate to the ""https://demowebshop.tricentis.com/""
2. Search for the ""14.1-inch Laptop"" product.
3. Click the ""Add to cart"" button.
4. Verify that the shopping cart icon updates to show ""1""or(increases to 1).

TC_DWT_008:-
Verify adding a '$25 Virtual Gift Card' to the shopping cart
1. Navigate to the ""https://demowebshop.tricentis.com/""
2. Search for the ""$25 Virtual Gift Card"" product.
3. Click the ""Add to cart"" button for the gift card.
4. Enter the ""Recipient's Name"" and ""Recipient's Email"".
5. Verify that the shopping cart icon updates to show '1' or(increases to 1)

TC_DWT_009:-
Verify viewing the shopping cart contents
1. Navigate to the ""https://demowebshop.tricentis.com/""
2. Click the ""Shopping cart"" link.
3. Verify that the added items are displayed in the cart with correct product name,price and quantity.

"TC_DWT_010:-
Verify updating quantity in the shopping cart
1. Navigate to the shopping cart page.
2. Change the quantity of an item (from 1 to 2).
3. Click the ""Update shopping cart"" button.
4. Verify the item's price and the subtotal are updated accordingly."

"TC_DWT_011:-
Verify removing an item from the shopping cart
1. Navigate to the shopping cart page.
2. Click the 'Remove' checkbox for one of the items.
3. Click the ""Update shopping cart"" button.
4. Verify that the selected item is no longer displayed in the cart."

"TC_DWT_012:-
Verify checkout process for registered users
1. Navigate to the shopping cart.
2. Click on the ""terms of service"" checkbox.
3. Click the 'Checkout' button.
4. Fill in all required billing and shipping details and click on the ""Continue"" button.
5. Select a payment method click on the ""Continue"" button.
6. Fill the Payment information and click on the ""Continue"" button.
7. Verify that the selected product name,price and quantity.
8. Confirm the order.
9. Verify that same product name, price and quantity.

TC_DWT_013:-
Verify checkout process for guest users
1. Navigate to the ""https://demowebshop.tricentis.com/""
2. Add any product to the shopping cart.
3. Navigate to the shopping cart.
4. Click on the ""terms of service"" checkbox.
5. Click the ""Checkout"" button.
6. Select the ""Checkout as Guest"" option.
5. Fill in all required billing address details and click on the ""Continue"" button.
6. Fill in all required shipping address details or select ""In-Store Pickup"" and click on the ""Continue"" button.
6. Select a payment method click on the ""Continue"" button.
7. Fill the Payment information and click on the ""Continue"" button.
8. Verify that the selected product name,price and quantity.
9. Confirm the order.
10. Verify that same product name, price and quantity.

TC_DWT_014:-
Verify navigation to different product categories
1. Navigate to the ""https://demowebshop.tricentis.com/""
2. Click on the ""Categories"" Section.
3. Select a category (""Books"").
4. Verify that the page navigates to the selected category's listing page.

TC_DWT_015:-
Verify registration with existing email
1. Navigate to the ""https://demowebshop.tricentis.com/""
2. Click the ""Register"" link.
3. Fill in all required fields, using an email address that is already registered.
4. Click the 'Register' button.
5. Verify the ""The specified email already exists"" message.

TC_DWT_016:-
Verify that the copyright year displayed in the footer is 2026.
1. Navigate to the ""https://demowebshop.tricentis.com/""
2. Scroll to the footer and verify that the copyright year is 2026 and that the website name matches the domain name.

TC_DWT_017:-
Verify that selected product in the cart and thank you page.
1. Navigate to the shopping cart.
2. Click on the """"terms of service"""" checkbox.
3. Click the 'Checkout' button.
4. Fill in all required billing and shipping details and click on the """"Continue"""" button.
5. Select a payment method click on the """"Continue"""" button.
6. Fill the Payment information and click on the """"Continue"""" button.
7. Verify that the selected product name,price and quantity.
8. Confirm the order.
9. Verify that same product name, price and quantity.
10. Click here for order details.

TC_DWT_018:-
Validate the Responsive Design – Desktop View
1. Navigate to the ""https://demowebshop.tricentis.com/""
2. Scroll through the entire site on all browsers and verify that the design and functionality are working correctly.
3. Check that the product titles, descriptions, and prices on each browser and verify that the text remains clearly readable.
4. Check that the ""Add to Cart"" button and interact with the checkout form fields on each browser to check that buttons are comfortably tappable and keyboard open across all screen sizes.
5. Scroll to the footer to verify that the layout does not break, content does not overlap, and all footer links remain fully visible

TC_DWT_019:-
Validate the Responsive Design and functionality -- Mobile and ipad view
1. Navigate to the ""https://demowebshop.tricentis.com/""
2. Scroll through the entire site on each device and verify that the design and functionality work correctly on mobile and iPad devices (iPhone 16 Plus, iPhone 13, Samsung S21 FE, iPad Pro, and iPad Air).
3. Check that the product titles, descriptions, and prices on each device and verify that the text remains clearly readable.
4. Check that the ""Add to Cart"" button and interact with the checkout form fields on each device to check that buttons are comfortably tappable and keyboard open across all screen sizes.
5. Rotate each device to landscape mode and scroll to the footer to verify that the layout does not break, content does not overlap, and all footer links remain fully visible.

**AI Manual Test Cases:-**
Prompt:- write the functional test cases for "https://demowebshop.tricentis.com/". format should be : TestCases 001:- _ 
1. Go to Amazon.com 
2. Click on Sign In 
3. Enter a valid registered email/mobile number 
4. Click on Continue 
5. Enter a valid password 
6. Click on Sign In 
7. Verify that the user is logged in successfully 
8. Verify that the Account & Lists section displays the logged-in user name


Below are sample **Functional Test Cases** for **[https://demowebshop.tricentis.com/](https://demowebshop.tricentis.com/)** in your requested format.

TestCases
001:-
Verify User Registration
1. Go to [https://demowebshop.tricentis.com/](https://demowebshop.tricentis.com/)
2. Click on Register
3. Select Gender
4. Enter First Name
5. Enter Last Name
6. Enter a valid Email Address
7. Enter Password
8. Confirm Password
9. Click on Register
10. Verify that the registration is successful
11. Verify that the confirmation message is displayed

002:-
Verify User Login
1. Go to [https://demowebshop.tricentis.com/](https://demowebshop.tricentis.com/)
2. Click on Log in
3. Enter a valid Email
4. Enter a valid Password
5. Click on Log in
6. Verify that the user is logged in successfully
7. Verify that the Logout link is displayed

003:-
Verify User Logout
1. Login with valid credentials
2. Click on Logout
3. Verify that the user is logged out successfully
4. Verify that the Log in link is displayed

004:-
Verify Search Functionality
1. Go to the Home Page
2. Enter a valid product name in the search box
3. Click on Search
4. Verify that matching products are displayed
5. Verify that the searched product appears in the results

005:-
Verify Product Details Page
1. Go to the Home Page
2. Select any product
3. Click on the product name/image
4. Verify that the product details page opens
5. Verify product name, price, description, and availability

006:-
Verify Add Product to Cart
1. Login to the application
2. Navigate to a product category
3. Select a product
4. Click on Add to cart
5. Verify that the success message is displayed
6. Verify that the cart count is increased

007:-
Verify Shopping Cart Page
1. Add a product to the cart
2. Click on Shopping Cart
3. Verify that the selected product is displayed
4. Verify product quantity and price
5. Verify total amount calculation

008:-
Verify Update Product Quantity in Cart
1. Add a product to the cart
2. Open Shopping Cart
3. Change product quantity
4. Click on Update Shopping Cart
5. Verify that the quantity is updated
6. Verify that the total amount is recalculated

009:-
Verify Remove Product from Cart
1. Add a product to the cart
2. Open Shopping Cart
3. Select the Remove checkbox
4. Click on Update Shopping Cart
5. Verify that the product is removed from the cart

010:-
Verify Add Product to Wishlist
1. Login to the application
2. Open a product page
3. Click on Add to Wishlist
4. Verify that the success message is displayed
5. Open Wishlist
6. Verify that the product is added successfully

011:-
Verify Email a Friend Feature
1. Login to the application
2. Open a product page
3. Click on Email a Friend
4. Enter a friend's email address
5. Enter a message
6. Click on Send Email
7. Verify that the email is sent successfully

012:-
Verify Product Comparison
1. Open Product A
2. Click on Add to Compare List
3. Open Product B
4. Click on Add to Compare List
5. Open Compare Products page
6. Verify that both products are displayed for comparison

013:-
Verify Category Navigation
1. Go to the Home Page
2. Click on any product category
3. Verify that the category page opens
4. Verify that related products are displayed

014:-
Verify Sort Products
1. Open a product category
2. Select "Price: Low to High" from Sort By
3. Verify products are sorted correctly
4. Select "Price: High to Low"
5. Verify products are sorted correctly

015:-
Verify Checkout Process
1. Login to the application
2. Add a product to the cart
3. Open Shopping Cart
4. Accept Terms of Service
5. Click on Checkout
6. Enter Billing Address details
7. Select Shipping Method
8. Select Payment Method
9. Confirm the Order
10. Verify that the order is placed successfully
11. Verify that the order confirmation message is displayed

016:-
Verify My Account Details
1. Login to the application
2. Click on My Account
3. Verify that account details are displayed
4. Update account information
5. Save changes
6. Verify that the information is updated successfully

017:-
Verify Change Password
1. Login to the application
2. Open My Account
3. Click on Change Password
4. Enter Current Password
5. Enter New Password
6. Confirm New Password
7. Click on Change Password
8. Verify that the password is changed successfully

018:-
Verify Contact Us Form
1. Go to Contact Us page
2. Enter Name
3. Enter Email
4. Enter Enquiry Message
5. Click on Submit
6. Verify that the enquiry is submitted successfully

019:-
Verify Newsletter Subscription
1. Enter a valid email address in the Newsletter field
2. Click on Subscribe
3. Verify that the subscription success message is displayed

020:-
Verify Order History
1. Login to the application
2. Navigate to My Account
3. Click on Orders
4. Verify that previous orders are displayed
5. Verify order details are accessible

These cover the main functional areas: **Registration, Login, Search, Product Details, Cart, Wishlist, Compare Products, Checkout, My Account, Contact Us, Newsletter, and Orders**.

**Your Thoughts for Test Cases:-**
Generating test cases with the help of AI including manual written test cases provides almost 100% test caverage.
The AI-generated test cases covered most of the critical business flows such as Registration, Login, Search, Shopping Cart, Wishlist, Checkout, and Order Placement.
The test cases were structured in a step-by-step format, making them easy to understand and suitable for both manual execution and future automation implementation.

**What I Felt Suitable:**
Covered major end-to-end flow.
Included both positive and negative scenarios (e.g:- valid login and invalid login).
Test steps were clear and easy to execute.
Most test cases were reusable for automation with minor modifications.
Functional coverage was good for an e-commerce application.
Included verification points for critical functionalities such as cart updates, checkout, and order confirmation.

**What I Felt Not Suitable:**
Generated too many test cases for a single flow. some of there were not that much useful with respect to the application.
Some AI-generated test cases lacked detailed expected results.
A few scenarios were too generic and required additional validation checkpoints.
Edge cases and boundary validations were limited.
Responsive design and UI validation were mixed with functional test cases and should ideally be maintained separately.
Some test cases contained hardcoded values that may require dynamic test data for automation.
Negative scenarios for registration, checkout, and form validations were not sufficiently covered.
Accessibility, performance, and security-related test scenarios were not included.
Certain test cases required refinement to make them fully automation-ready and maintainable.

**Final Test Case:-**
**AI+Manual, Combine them and make a proper test case
for Automation ready.**
https://demowebshop.tricentis.com/ - Functional Test Cases

TC_DWT_001: Verify Successful User Registration
Precondition: User is not already registered.
1. Navigate to https://demowebshop.tricentis.com/
2. Click the "Register" link.
3. Select Gender.
4. Enter First Name.
5. Enter Last Name.
6. Enter a unique Email Address.
7. Enter Password.
8. Enter Confirm Password.
9. Click the "Register" button.
10. Verify registration success message is displayed.
11. Verify user is logged in successfully.


TC_DWT_002: Verify Registration with Existing Email Address
Precondition: Email address already exists.
1. Navigate to the application.
2. Click the "Register" link.
3. Enter valid registration details using an existing email.
4. Click the "Register" button.
5. Verify duplicate email validation message is displayed.


TC_DWT_003: Verify Login with Valid Credentials
Precondition: Registered user exists.
1. Navigate to the application.
2. Click the "Log in" link.
3. Enter valid Email.
4. Enter valid Password.
5. Select "Remember me".
6. Click the "Log in" button.
7. Verify user is successfully logged in.
8. Verify "Log out" link is displayed.


TC_DWT_004: Verify Login with Invalid Password
Precondition: Registered user exists.
1. Navigate to the application.
2. Click the "Log in" link.
3. Enter valid Email.
4. Enter invalid Password.
5. Click the "Log in" button.
6. Verify login error message is displayed.

TC_DWT_005: Verify Logout Functionality
Precondition: User is logged in.
1. Click the "Log out" link.
2. Verify user is logged out successfully.
3. Verify the "Log in" link is displayed.
4. Verify user session is terminated.

TC_DWT_006: Verify Empty Shopping Cart
1. Navigate to the application.
2. Hover over the "Shopping Cart" icon.
3. Verify cart item count is zero.
4. Verify empty cart message is displayed.

TC_DWT_007: Verify Product Search with Valid Product Name
1. Navigate to the application.
2. Enter a valid product name in the search field.
3. Click the "Search" button.
4. Verify search results page is displayed.
5. Verify matching product appears in search results.

TC_DWT_008: Verify Product Search with Invalid Product Name
1. Navigate to the application.
2. Enter an invalid product name.
3. Click the "Search" button.
4. Verify no-result message is displayed.

TC_DWT_009: Verify Add Product to Shopping Cart
1. Navigate to the application.
2. Search for "14.1-inch Laptop".
3. Open the product details page.
4. Click "Add to cart".
5. Verify success notification is displayed.
6. Verify shopping cart count increases by 1.

TC_DWT_010: Verify Add Virtual Gift Card to Shopping Cart
1. Navigate to the application.
2. Search for "$25 Virtual Gift Card".
3. Open the product details page.
4. Enter Recipient Name.
5. Enter Recipient Email.
6. Click "Add to cart".
7. Verify success notification is displayed.
8. Verify shopping cart count increases.

TC_DWT_011: Verify Shopping Cart Contents
Precondition: Product exists in cart.
1. Open Shopping Cart.
2. Verify product name.
3. Verify quantity.
4. Verify unit price.
5. Verify subtotal calculation.

TC_DWT_012: Verify Update Product Quantity in Shopping Cart
Precondition: Product exists in cart.
1. Open Shopping Cart.
2. Change quantity from 1 to 2.
3. Click "Update Shopping Cart".
4. Verify quantity is updated.
5. Verify subtotal is recalculated correctly.

TC_DWT_013: Verify Remove Product from Shopping Cart
Precondition: Product exists in cart.
1. Open Shopping Cart.
2. Select Remove checkbox.
3. Click "Update Shopping Cart".
4. Verify product is removed from cart.
5. Verify cart count is updated.

TC_DWT_014: Verify Wishlist Functionality
Precondition: User is logged in.
1. Search for a product.
2. Open the product details page.
3. Click "Add to wishlist".
4. Verify success notification is displayed.
5. Navigate to Wishlist.
6. Verify selected product is present in the wishlist.

TC_DWT_015: Verify Compare Products Functionality
1. Navigate to the application.
2. Open Product A.
3. Click "Add to compare list".
4. Open Product B.
5. Click "Add to compare list".
6. Navigate to Compare Products page.
7. Verify both products are displayed for comparison.

TC_DWT_016: Verify Checkout Process for Registered User
Precondition: Logged-in user and product exists in cart.
1. Open Shopping Cart.
2. Accept Terms of Service.
3. Click "Checkout".
4. Complete Billing Address.
5. Complete Shipping Method.
6. Select Payment Method.
7. Enter Payment Information.
8. Review Order Summary.
9. Verify product name, quantity and price.
10. Click "Confirm".
11. Verify order success message.
12. Verify order details match cart details.

TC_DWT_017: Verify Checkout Process as Guest User
Precondition: Product exists in cart.
1. Add product to cart.
2. Open Shopping Cart.
3. Accept Terms of Service.
4. Click "Checkout".
5. Select "Checkout as Guest".
6. Enter Billing Address.
7. Enter Shipping Details.
8. Select Payment Method.
9. Enter Payment Information.
10. Review Order Summary.
11. Confirm Order.
12. Verify order success message.
13. Verify order details are correct.

TC_DWT_018: Verify Order Summary Consistency
Precondition: Product exists in cart.
1. Add product to cart.
2. Proceed through checkout.
3. Verify product details on Order Review page.
4. Complete order placement.
5. Verify same product details on Thank You page.
6. Click Order Details.
7. Verify product name, quantity and price remain unchanged.

TC_DWT_019: Verify Product Category Navigation
1. Navigate to the application.
2. Click the "Books" category.
3. Verify Books category page opens.
4. Verify product listing is displayed.
5. Repeat for Computers and Electronics categories.

TC_DWT_020: Verify Forgot Password Functionality
1. Navigate to the application.
2. Click the "Log in" link.
3. Click "Forgot password?".
4. Enter a registered email address.
5. Click "Recover".
6. Verify password recovery confirmation message is displayed.

TC_DWT_021: Verify Newsletter Subscription
1. Navigate to the application.
2. Scroll to Newsletter section.
3. Enter a valid email address.
4. Click "Subscribe".
5. Verify subscription success message is displayed.

TC_DWT_022: Verify Contact Us Form
1. Navigate to the Contact Us page.
2. Enter Name.
3. Enter Email.
4. Enter Enquiry Message.
5. Click "Submit".
6. Verify enquiry submission success message is displayed.

TC_DWT_023: Verify Footer Copyright Information
1. Navigate to the application.
2. Scroll to footer section.
3. Verify copyright year is "2026".
4. Verify website name is displayed correctly.
5. Verify website name matches domain name.

TC_DWT_024: Verify Responsive Layout and Core Functionality
1. Open the application on Desktop Chrome browser.
2. Open the application on Firefox browser.
3. Open the application on Edge browser.
4. Verify header, navigation menu and footer are displayed correctly.
5. Verify product listings render properly.
6. Verify text remains readable.
7. Verify buttons and links are clickable.
8. Verify Shopping Cart functionality works correctly.
9. Verify Checkout page renders correctly.
10. Verify no overlapping, broken or truncated UI elements are present.
11. Verify page scrolling works properly throughout the site.
