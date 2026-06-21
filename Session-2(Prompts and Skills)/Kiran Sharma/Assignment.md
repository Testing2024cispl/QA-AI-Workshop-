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


Final Test Case After Verifying same with AI—-------------------

Module: Home Page 

TC_HOME_001 : Verify Home Page Loads Successfully 
Steps: Open website URL https://www.demoblaze.com/ 
Expected Result: Home page should load successfully 

TC_HOME_002 : Verify Website Logo Visibility
Steps: Open the home page.
Expected Result: "PRODUCT STORE" logo should be visible on the top left corner. 

TC_HOME_003 : Verify Navigation Menu Options
Steps: Open the home page.
Expected Result: Home, Contact, About Us, Cart, Log In, and Sign Up options should be displayed in the navigation menu. 

TC_HOME_004 : Verify Product Categories Display
Steps: Open the home page and observe the Categories section.
Expected Result: Phones, Laptops, and Monitors categories should be displayed. 

TC_HOME_005 : Verify Product Listings Display
Steps: Open the home page.
Expected Result: Products should display with image, name, description, and price. 


TC_HOME_006 : Verify Carousel Next Button Functionality
Steps: Click the "Next" button on the image slider.
Expected Result: Carousel should move to the next slide. 

TC_HOME_007 : Verify Carousel Previous Button Functionality
Steps: Click the "Previous" button on the image slider.
Expected Result: Carousel should move to the previous slide. 
Module: Sign Up

TC_SIGNUP_001 : Verify Sign Up Popup Opens
 Steps: Click on "Sign Up".
 Expected Result: Sign Up popup should open with Username and Password fields.

TC_SIGNUP_002 : Verify Successful User Registration
 Steps:
Click Sign Up.
Enter valid Username.
Enter valid Password.
Click the Sign Up button.
Expected Result: User account should be created successfully.


TC_SIGNUP_003 : Verify Sign Up with Blank Username
 Steps:
Click Sign Up.
Leave Username blank.
Enter Password.
Click Sign Up.
Expected Result: Appropriate validation message should appear.

TC_SIGNUP_004 : Verify Sign Up with Blank Password
 Steps:
Click Sign Up.
Enter Username.
Leave Password blank.
Click Sign Up.
Expected Result: Appropriate validation message should appear.
Module:Login Test

TC_LOGIN_001 : Verify Login Popup Opens
 Steps: Click Log In.
 Expected Result: Login popup should open with Username and Password fields.

TC_LOGIN_002 : Verify Login with Valid Credentials
 Steps:
Click Log In.
Enter valid Username.
Enter valid Password.
Click Log In.
Expected Result: User should log in successfully and username should be displayed.

TC_LOGIN_003 : Verify Login with Invalid Credentials
 Steps:
Click Log In.
Enter invalid Username/Password.
Click Log In.
Expected Result: Error message should be displayed.
Module: Product Details Page 

TC_PRODUCT_001 : Verify Product Details Page Opens
 Steps: Click on any product from the home page.
 Expected Result: Product details page should open successfully.

TC_PRODUCT_002 : Verify Product Name Display
 Steps: Open any product details page.
 Expected Result: Product name should be displayed correctly.

TC_PRODUCT_003 : Verify Product Price Display
 Steps: Open any product details page.
 Expected Result: Product price should be displayed correctly.

TC_PRODUCT_004 : Verify Product Description Display
 Steps: Open any product details page.
 Expected Result: Product description should be displayed.

TC_PRODUCT_005 : Verify Product Image Display
 Steps: Open any product details page.
 Expected Result: Product image should load without distortion or broken image icon.

Module: Category

TC_CATEGORY_001 : Verify Phones Category Filter
 Steps: Click on "Phones" category.
 Expected Result: Only phone products should be displayed.

TC_CATEGORY_002 : Verify Laptops Category Filter
 Steps: Click on "Laptops" category.
 Expected Result: Only laptop products should be displayed.

TC_CATEGORY_003 : Verify Monitors Category Filter
 Steps: Click on "Monitors" category.
 Expected Result: Only monitor products should be displayed.

TC_CATEGORY_004 : Verify Category Switching
 Steps: Click Phones → Laptops → Monitors.
 Expected Result: Products should refresh according to selected category.
Module: Add To Cart 

TC_CART_001 : Verify Add Product To Cart
 Steps:
Open any product.
Click Add To Cart.
Expected Result: Product should be added successfully to the cart.

TC_CART_002 : Verify Product Display In Cart
 Steps:
Add a product to cart.
Open Cart page.
Expected Result: Added product should be displayed in cart with correct details.

TC_CART_003 : Verify Delete Product From Cart
 Steps:
Add product to cart.
Open Cart page.
Click Delete.
Expected Result: Product should be removed from the cart.

TC_CART_004 : Verify Cart Page Accessibility
 Steps: Click the Cart menu.
 Expected Result: Cart page should open successfully.

TC_CART_005 : Verify Product Name in Cart
 Steps: Add product to cart and open Cart page.
 Expected Result: Correct product name should be displayed.

TC_CART_006 : Verify Product Price in Cart
 Steps: Add product to cart and open Cart page.
 Expected Result: Correct product price should be displayed.

TC_CART_007 : Verify Total Price Calculation
 Steps: Add multiple products to cart.
 Expected Result: Total amount should equal sum of all product prices.

TC_CART_008 : Verify Cart Persistence After Refresh
 Steps: Add product to cart and refresh the page.
 Expected Result: Product should remain in cart.

Module: Place Order 

TC_ORDER_001 : Verify Place Order Popup Opens
 Steps:
Add product to cart.
Open Cart page.
Click Place Order.
Expected Result: Place Order form should be displayed.

TC_ORDER_002 : Verify Successful Purchase
 Steps:
Add product to cart.
Open Cart page.
Click Place Order.
Fill all mandatory fields.
Click Purchase.
Expected Result: Order confirmation message should be displayed with Order ID and Amount.

TC_ORDER_003 : Verify Purchase With Empty Mandatory Fields
 Steps:
Open Place Order form.
Leave mandatory fields blank.
Click Purchase.
Expected Result: Validation message should appear.

TC_ORDER_004 : Verify Purchase with Valid Data
 Steps: Enter valid order details and click Purchase.
 Expected Result: Purchase should complete successfully.

TC_ORDER_005 : Verify Order Confirmation Popup
 Steps: Complete purchase process.
 Expected Result: Confirmation popup should display order details.

TC_ORDER_006 : Verify Generated Order ID
 Steps: Complete purchase process.
 Expected Result: Unique Order ID should be generated.

TC_ORDER_007 : Verify Purchase Amount
 Steps: Complete purchase process.
 Expected Result: Purchase amount should match cart total.

TC_ORDER_008 : Verify Confirmation Popup Close Button
 Steps: Complete purchase and click OK.
 Expected Result: Popup should close and user should return to home page.

UI / UX Test Cases---------------------------------------

TC_UI_001 : Verify Website Responsive Layout
 Steps: Resize browser window.
 Expected Result: Website layout should adjust properly.

TC_UI_002 : Verify Navigation Menu Alignment
 Steps: Open website.
 Expected Result: Navigation menu should be properly aligned.

TC_UI_003 : Verify Product Card Alignment
 Steps: Open home page.
 Expected Result: Product cards should be aligned consistently.

TC_UI_004 : Verify Broken Images
 Steps: Navigate through all products.
 Expected Result: No broken images should be displayed.

TC_UI_005 : Verify Hyperlinks Functionality
 Steps: Click all navigation links.
 Expected Result: All links should navigate correctly.

Negative Test Cases------------------------

TC_NEG_001 : Verify Login with Invalid Username
 Steps: Enter invalid username and valid password.
 Expected Result: Error message should be displayed.

TC_NEG_002 : Verify Login with Invalid Password
 Steps: Enter valid username and invalid password.
 Expected Result: Error message should be displayed.

TC_NEG_003 : Verify Add Product Without Internet Connection
 Steps: Disconnect internet and click Add to Cart.
 Expected Result: Appropriate error handling should occur.

TC_NEG_004 : Verify Multiple Rapid Clicks on Add to Cart
 Steps: Click Add to Cart button multiple times rapidly.
 Expected Result: Application should handle duplicate requests properly.

TC_NEG_005 : Verify Session After Logout
 Steps: Login → Logout → Use browser Back button.
 Expected Result: User should not access authenticated session.

Security Test Case----------------------
TC_SEC_001 : Verify Password Masking
 Steps: Open Login/Sign Up popup and enter password.
 Expected Result: Password should be masked.




