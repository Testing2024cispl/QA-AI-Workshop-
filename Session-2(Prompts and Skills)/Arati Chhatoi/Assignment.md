DemoBlaze Manual Test Cases
Application URL: https://www.demoblaze.com
Username: aratitest2026
Password: Test@123456
Test Case 1 - Verify DemoBlaze Website Launch
Open a browser and navigate to https://www.demoblaze.com. Verify that the homepage loads successfully, the logo is displayed, product categories are visible, and no error message appears.
Test Case 2 - Verify User Login
Click the Login option. Enter the username 'aratitest2026' and valid password. Click the Login button and verify that the user is logged in successfully and the username is displayed in the header.
Test Case 3 - Verify Product Details Page
From the homepage, select the Samsung Galaxy S6 product. Verify that the product details page opens and displays the product name, description, price, and Add to Cart button.
Test Case 4 - Verify Add to Cart Functionality
On the product details page, click Add to Cart. Verify that the product is successfully added to the cart and a confirmation message is displayed.
Test Case 5 - Verify Cart Page
Click the Cart menu from the navigation bar. Verify that the added product is listed in the cart with the correct product name, quantity, and price.
Test Case 6 - Verify Place Order Popup
On the Cart page, click the Place Order button. Verify that the order popup/modal is displayed with fields such as Name, Country, City, Credit Card, Month, and Year.
Test Case 7 - Verify Closing Order Popup
When the Place Order popup is displayed, click the Close (X) button. Verify that the popup closes successfully and the user remains on the Cart page.
DemoBlaze – AI Generated Manual Test Cases
Application Information
URL: https://www.demoblaze.com
Test Environment
Browser: Chrome / Edge / Firefox
Internet Connection Required
Test Type: Functional Testing

Module 1: Homepage Validation
Test Case 1: Verify Homepage Loading
Objective
Verify that the DemoBlaze homepage loads successfully.
Steps
Open browser.
Enter DemoBlaze URL.
Press Enter.
Expected Result
Homepage loads successfully.
Logo is displayed.
Categories section is visible.
Product list is displayed.

Test Case 2: Verify Navigation Menu
Steps
Open homepage.
Verify Home, Contact, About Us, Cart, Login, and Sign Up links.
Expected Result
All navigation links should be visible and clickable.

Module 2: User Authentication
Test Case 3: Verify User Registration
Steps
Click Sign Up.
Enter unique username.
Enter password.
Click Sign Up button.
Expected Result
User account should be created successfully.

Test Case 4: Verify Login with Valid Credentials
Steps
Click Login.
Enter valid username.
Enter valid password.
Click Login.
Expected Result
User should be logged in successfully. Welcome username should appear.

Test Case 5: Verify Login with Invalid Credentials
Steps
Click Login.
Enter invalid username/password.
Click Login.
Expected Result
Appropriate error message should be displayed.

Test Case 6: Verify Logout Functionality
Steps
Login successfully.
Click Logout.
Expected Result
User should be logged out successfully.

Module 3: Product Validation
Test Case 7: Verify Product Details Page
Steps
Select Samsung Galaxy S6.
Open product details page.
Expected Result
Product name, image, description, and price should be displayed.

Test Case 8: Verify Product Category Filtering
Steps
Click Phones category.
Click Laptops category.
Click Monitors category.
Expected Result
Only relevant products should be displayed.

Module 4: Add To Cart
Test Case 9: Verify Add Product to Cart
Steps
Open any product.
Click Add to Cart.
Expected Result
Success confirmation message should appear.

Test Case 10: Verify Multiple Products Can Be Added
Steps
Add first product.
Add second product.
Open Cart page.
Expected Result
Both products should appear in cart.

Test Case 11: Verify Same Product Added Multiple Times
Steps
Add same product twice.
Open Cart.
Expected Result
Application should handle duplicate products correctly.

Module 5: Cart Validation
Test Case 12: Verify Cart Page
Steps
Add product.
Open Cart page.
Expected Result
Correct product should be displayed.

Test Case 13: Verify Product Price in Cart
Steps
Add product.
Open Cart.
Expected Result
Cart price should match product price.

Test Case 14: Verify Product Deletion from Cart
Steps
Add product.
Open Cart.
Click Delete.
Expected Result
Product should be removed successfully.

Module 6: Place Order
Test Case 15: Verify Place Order Popup
Steps
Add product to cart.
Open Cart.
Click Place Order.
Expected Result
Order popup should appear.

Test Case 16: Verify Mandatory Fields
Steps
Open Place Order popup.
Leave fields blank.
Click Purchase.
Expected Result
Validation message should be displayed.

Test Case 17: Verify Successful Order Placement
Steps
Enter Name.
Enter Country.
Enter City.
Enter Credit Card Number.
Enter Month and Year.
Click Purchase.
Expected Result
Order should be placed successfully. Confirmation message should be displayed.

Test Case 18: Verify Order Confirmation Details
Steps
Complete purchase.
Expected Result
Confirmation popup should display:
Order ID
Amount
Card Number
Date

Test Case 19: Verify OK Button on Confirmation Popup
Steps
Complete purchase.
Click OK button.
Expected Result
User should return to homepage.

Module 7: Negative Testing
Test Case 20: Verify Application Behavior Without Internet
Steps
Disconnect internet.
Open application.
Expected Result
Appropriate browser/network error should appear.

Test Case 21: Verify Invalid Credit Card Number
Steps
Open Place Order popup.
Enter invalid card number.
Click Purchase.
Expected Result
System should handle invalid input appropriately.

Test Case 22: Verify Empty Cart Checkout
Steps
Open Cart with no products.
Click Place Order.
Expected Result
User should not be allowed to complete purchase without products.

Test Coverage Summary
Covered Modules
✔ Homepage
✔ Registration
✔ Login
✔ Logout
✔ Product Details
✔ Category Filtering
✔ Add To Cart
✔ Cart Management
✔ Delete Product
✔ Place Order
✔ Purchase Confirmation
✔ Negative Testing
Priority
High
Test Type
Manual Functional Testing
