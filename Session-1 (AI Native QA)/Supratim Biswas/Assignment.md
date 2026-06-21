Swag Lab – Test Cases

Test Scenarios:
Verify that the user should be logged in to the application with valid credentials. 
Verify that the user should not be able to log in with a valid username and an invalid password
Verify that the user should not be able to log in with an invalid username and a valid password
Verify that the user should not be able to log in with an invalid username and  password
Verify that the user should add a product to the cart and remove the same product from the cart. 
Verify that the user should add multiple products to the cart.
Verify that the user can filter the product by price, from high to low. 
Verify that the user should filter the products from low to high price. 
Verify that the user should filter the products by Name (A to Z) 
 Verify that the user should filter the products by Name (Z to A)
 Verify that the user should be able to purchase a product using valid prospect information. 
 Verify that the user should not be able to purchase a product using an invalid zip code. 
 Verify that the user should not be able to purchase a product using a completely blank prospect form. 
 Verify that the user should not be able to purchase a product, keeping the first name and last name blank in the prospect form. 
 Verify that the user should not be able to purchase a product, keeping the zip code and last name blank in the prospect form. 
 Verify that the user should not be able to purchase a product, keeping the zip code and first name blank in the prospect form.
 Verify that the user should not be able to purchase a product, keeping only the zip code blank. 
 Verify that the user should not be able to purchase a product, keeping only the first name blank. 
 Verify that the user should not be able to purchase a product, keeping only the first name blank. 
 Verify that the user should add the product to the cart from the respective product page. 
 The user should add the product to the cart from the respective product page, remove the product from the cart, and verify that the user should be able to re-add the same product to the cart from that product page. 
 Verify that the user should not be able to purchase a product by using a 4-digit Zip code in the prospect form. 
 Verify that the user should not be able to purchase a product by using a 6-digit Zip code in the prospect form.
 

Test Cases: 
Verify that the user should be logged in to the application with valid credentials. 

Navigate to the target URL “https://www.saucedemo.com/”. 
Enter the username into the username text field as ${validUsername}. 
Enter the secure string into the password text field as ${validPassword}. 
Click on the “Login” button. 
Verify that the page sub-label is ${Products}. 
Verify that the cart icon is visible in the right corner

Verify that the user should not be able to log in with an invalid username and a valid password. 

Navigate to the target URL “https://www.saucedemo.com/”. 
Enter the username into the username text field as ${invalidUsername}. 
Enter the secure string into the password text field as ${validPassword}. 
Click on the “Login” button. 
Verify that the displayed error message is equal to “Epic sadface: Username and password do not match any user in this service." 

Verify that the user should not be able to log in with a valid username and an invalid password

Navigate to the target URL “https://www.saucedemo.com/”. 
Enter the username into the username text field as ${validUsername}. 
Enter the secure string into the password text field as ${invalidPassword}. 
Click on the “Login” button. 
Verify that the displayed error message is equal to “Epic sadface: Username and password do not match any user in this service."
 
Verify that the user should not be able to log in with an invalid username and password

Navigate to the target URL “https://www.saucedemo.com/”. 
Enter the username into the username text field as ${invalidUsername}. 
Enter the secure string into the password text field as ${invalidPassword}. 
Click on the “Login” button. 
Verify that the displayed error message is equal to “Epic sadface: Username and password do not match any user in this service."

Verify that the user should add a product to the cart and remove the same product from the cart. 

Navigate to the target URL “https://www.saucedemo.com/”. 
Enter the username into the username text field as ${validUsername}. 
Enter the secure string into the password text field as ${validPassword}. 
Click on the “Login” button. 
Verify that the page sub-label is ${Products}. 
Verify that the initial cart count is 0.
Verify that the list of products is visible in grid format. 
Verify that the “Add to cart” button is enabled with respect to each product. 
Store a product name in a variable as ${productName}.  
 Click on the “Add to cart” button of ${productName}. 
 Verify that the “Remove” button is enabled below the ${productname}. 
 Verify that the cart count is increased to 1. 
 Click on the cart icon.
 Verify that the page sub-label is equal to “Your Cart ”. 
 Verify that the ${productName} is equal to the name of the product present on the cart page. 
 Verify that the “Remove” button for that ${productName} is enabled on the cart. 
 Click on the “Remove” button for that ${productName} 
 Verify that the ${productName} is not visible on the cart page. 
 Click on the “Continue Shopping” button. 
 Verify that the “Add to Cart” button is enabled for that ${productName}. 

Verify that the user should add multiple products to the cart.

Navigate to the target URL “https://www.saucedemo.com/”. 
Enter the username into the username text field as ${validUsername}. 
Enter the secure string into the password text field as ${validPassword}. 
Click on the “Login” button. 
Store the 1st product name in a variable as ${productName1}.
Store the 2nd product name in a variable as ${productName2}
Verify that the initial cart count is 0.
Verify that the list of products is visible in grid format. 
Click on the “Add to cart” button of ${productName1}. 
 Click on the “Add to cart” button of ${productName2}.
 Verify that the “Remove” button is enabled for the ${productName1}. 
 Verify that the “Remove” button is enabled for the ${productName2}. 
 Verify that the “Cart” icon count is equal to 2. 
 Click on the “Cart” icon. 
 Verify that the page sub-label is equal to “Your Cart .” 
 Verify that the ${productName1} is equal to the name of the first product present on the cart page. 
 Verify that the ${productName2} is equal to the name of the second product present on the cart page. 

Verify that the user can filter the product by price, from high to low. 

Navigate to the target URL “https://www.saucedemo.com/”. 
Enter the username into the username text field as ${validUsername}. 
Enter the secure string into the password text field as ${validPassword}. 
Click on the “Login” button. 
Verify that the page sub-label is ${Products}. 
Verify that the list of products is visible in grid format. 
Verify that the “filter” icon is enabled. 
 Verify the “Name (A to Z)” is already selected as a filter dropdown option. 
 Click on the “filter” icon. 
 Click on the “Price (high to low)” as a filter dropdown option. 
 Verify that the product prices are shown in descending order.  
 Verify that the first product's price is greater than the second product's price. 
 Verify that the second product's price is greater than the third product's price.  

Verify that the user should filter the products from low to high price. 

Navigate to the target URL “https://www.saucedemo.com/”. 
Enter the username into the username text field as ${validUsername}. 
Enter the secure string into the password text field as ${validPassword}. 
Click on the “Login” button. 
Verify that the page sub-label is ${Products}. 
Verify that the list of products is visible in grid format. 
Verify that the “filter” icon is enabled. 
 Verify the “Name (A to Z)” is already selected as a filter dropdown option. 
 Click on the “filter” icon. 
 Click on the “Price (low to high)” as a filter dropdown option. 
 Verify that the product prices are shown in ascending order. 
 Verify that the first product's price is less than the second product's price. 
 Verify that the second product's price is less than the third product's price.  

Verify that the user should filter the products by Name (A to Z) 

Navigate to the target URL “https://www.saucedemo.com/”. 
Enter the username into the username text field as ${validUsername}. 
Enter the secure string into the password text field as ${validPassword}. 
Click on the “Login” button. 
Verify that the page sub-label is ${Products}. 
Verify that the list of products is visible in grid format. 
Verify that the “filter” icon is enabled. 
Verify the “Name (A to Z)” is already selected as a filter dropdown option. 
Verify that the product names are shown in A-Z order. 

Verify that the user should filter the products by Name (Z to A)

Navigate to the target URL “https://www.saucedemo.com/”. 
Enter the username into the username text field as ${validUsername}. 
Enter the secure string into the password text field as ${validPassword}. 
Click on the “Login” button. 
Verify that the page sub-label is ${Products}. 
Verify that the list of products is visible in grid format. 
Verify that the “filter” icon is enabled. 
Verify the “Name (A to Z)” is already selected as a filter dropdown option. 
Store the first product name as ${productName1}.
Click on the “filter” icon. 
 Click on the “Name (Z to A)" as a filter dropdown option. 
 Verify that the first product name is not equal to ${productName1}. 
 Verify that the product names are sorted in Z to A order.
 
Verify that the user should be able to purchase a product using valid prospect information. 

Navigate to the target URL “https://www.saucedemo.com/”. 
Enter the username into the username text field as ${validUsername}. 
Enter the secure string into the password text field as ${validPassword}. 
Click on the “Login” button. 
Verify that the page sub-label is ${Products}. 
Verify that the list of products is visible in grid format.
Store the first product name in a variable ${firstProductName}. 
Store the first product price in a variable ${firstProductPrice}.
Click on the “Add to cart” button of the ${firstProductName}. 
 Verify that the item count over the “cart” icon is increased to 1. 
 Click on the cart icon. 
 Verify that the product name is equal to ${firstProductName}. 
 Verify that the product price is equal to ${firstProductPrice}. 
 Verify that the “Checkout” button is enabled. 
 Click on the “Checkout” button. 
 Verify that the page sub-header is equal to “Checkout: Your Information.”
 Enter into the “First Name” text field as ${validFirstName}. 
 Enter into the “Last Name” text field as ${validLastName}. 
 Enter into the “Zip/Postal Code” text field as ${validZipCode}. 
 Verify that the “Continue” button is enabled.
 Click on the “Continue” button. 
 Verify that the page sub-header is equal to “Checkout: Overview.“
 Verify that the product quantity is equal to 1 as the “QTY” column value. 
 Verify that the product name under the “Description” column value is ${firstProductName}. 
 Verify that the product price for ${firstProductName} is equal to ${firstProductPrice}. 
 Verify that the value of the “Payment Information” label is not empty. 
 Verify that the value of the “Shipping Information” label is not empty. 
 Verify that the value of the “Price Total” label contains ${firstProductPrice} as the value of “Item Total” sub-label. 
 Verify that the “Tax” sub-label value is not empty.
 Store the tax value in a variable ${tax}.
 Verify that the "Total" label value is ${firstProductPrice}+${tax}. 
 Click on the “Finish” button. 
 Verify that the page header is equal to “Checkout: Complete! ”.
 Verify that the order confirmation message header is equal to “Thank you for your order! ”. 
 Verify that the order confirmation message sub-header is equal to “Your order has been dispatched, and will arrive just as fast as the pony can get there!”
 Verify that the “Back Home” button is enabled. 

Verify that the user should not be able to purchase a product using an invalid zip code.

Navigate to the target URL “https://www.saucedemo.com/”. 
Enter the username into the username text field as ${validUsername}. 
Enter the secure string into the password text field as ${validPassword}. 
Click on the “Login” button. 
Verify that the page sub-label is ${Products}. 
Verify that the list of products is visible in grid format.
Click on the “Add to cart” button of the ${firstProductName}.
 Verify that the item count over the “cart” icon is increased to 1. 
 Click on the cart icon. 
 Verify that the “Checkout” button is enabled. 
 Click on the “Checkout” button. 
 Verify that the page sub-header is equal to “Checkout: Your Information.”
 Enter into the “First Name” text field as ${validFirstName}. 
 Enter into the “Last Name” text field as ${validLastName}.
 Enter into the “Zip/Postal Code” text field as ${invalidZipCode}. 
 Click on the “Continue” button. 
 Verify that the error message should contain “Invalid Zip/Postal Code.”

Verify that the user should not be able to purchase a product using a completely blank prospect form.

Navigate to the target URL “https://www.saucedemo.com/”. 
Enter the username into the username text field as ${validUsername}. 
Enter the secure string into the password text field as ${validPassword}. 
Click on the “Login” button. 
Verify that the page sub-label is ${Products}. 
Verify that the list of products is visible in grid format.
Click on the “Add to cart” button of the ${firstProductName}.
 Verify that the item count over the “cart” icon is increased to 1. 
 Click on the cart icon. 
 Verify that the “Checkout” button is enabled. 
 Click on the “Checkout” button. 
 Verify that the page sub-header is equal to “Checkout: Your Information.” 
 Verify that the “First Name” text field is enabled. 
 Verify that the “Last Name” text field is enabled. 
 Verify that the “Zip/Postal Code” text field is enabled.  
 Click on the “Continue” button. 
 Verify that the error message is equal to “Error: First Name is required." 

Verify that the user should not be able to purchase a product, keeping the first name and last name blank in the prospect form. 

Navigate to the target URL “https://www.saucedemo.com/”. 
Enter the username into the username text field as ${validUsername}. 
Enter the secure string into the password text field as ${validPassword}. 
Click on the “Login” button. 
Verify that the page sub-label is ${Products}. 
Verify that the list of products is visible in grid format.
Click on the “Add to cart” button of the ${firstProductName}.
 Verify that the item count over the “cart” icon is increased to 1. 
 Click on the cart icon. 
 Verify that the “Checkout” button is enabled. 
 Click on the “Checkout” button. 
 Verify that the page sub-header is equal to “Checkout: Your Information.” 
 Verify that the “First Name” text field is enabled. 
 Verify that the “Last Name” text field is enabled. 
 Verify that the “Zip/Postal Code” text field is enabled.  
 Enter into the “Zip/Postal Code” text field as ${validZipcode}. 
 Click on the “Continue” button. 
 Verify that the error message is equal to “Error: First Name is required."

Verify that the user should add the product to the cart from the respective product page. 

Navigate to the target URL “https://www.saucedemo.com/”. 
Enter the username into the username text field as ${validUsername}. 
Enter the secure string into the password text field as ${validPassword}. 
Click on the “Login” button. 
Verify that the page sub-label is ${Products}. 
Verify that the list of products is visible in grid format.
Store the first product name in a variable as ${firstProductName}. 
Store the first product price as ${firstProductPrice}. 
Hover on the ${firstProductName}
 Verify that the ${firstProductName} is highlighted with green color. 
 Click on the ${firstProductName}. 
 Verify that the “Back to products” link is enabled in the upper left corner. 
 Verify that the product name is equal to ${firstProductName}. 
 Verify that the product price is equal to ${firstProductPrice}.
 Store the cart count in a variable as ${initialCartCount}  
 Click on the “Add to cart” button. 
 Verify that the cart count is ${initialCartCount+1}. 
Verify that the “Remove” button is enabled for the ${firstProductName}.
 Click on the cart icon. 
 Verify that the page header is equal to “Your Cart”. 
 Verify that the product name is equal to ${firstProductName}. 
 Verify that the product price is equal to ${firstProductPrice}.
 Verify that the “Remove” button is enabled for the ${firstProductName}.

**AI-generated test cases:** 
TC ID
Scenario
Test Steps
Test Data
Expected Result
TC_001
Verify login with valid user
Open site, enter username and password, click Login
standard_user / secret_sauce
User should land on Products page
TC_002
Verify login with locked user
Enter locked user credentials, click Login
locked_out_user / secret_sauce
Error message should display
TC_003
Verify login with invalid username
Enter invalid username and valid password
invalid_user / secret_sauce
Login should fail with error message
TC_004
Verify login with invalid password
Enter valid username and invalid password
standard_user / wrong_pass
Login should fail with error message
TC_005
Verify login with blank fields
Click Login without entering credentials
Blank
Username required error should display
TC_006
Verify product list loads
Login with valid user
standard_user
Product page should show inventory items
TC_007
Verify product details page
Click any product name/image
Any product
Product details page should open with name, price, description, and image
TC_008
Verify Add to Cart button
Click Add to Cart for a product
Any product
Cart badge should increase by 1 and button changes to Remove
TC_009
Verify Remove button
Add product, then click Remove
Any product
Product should be removed and cart badge should update
TC_010
Verify cart page
Add product and click cart icon
Any product
Cart page should display selected product
TC_011
Verify checkout with valid details
Go to cart, checkout, enter details, continue
First name, last name, postal code
Checkout overview page should display
TC_012
Verify checkout with missing first name
Leave first name empty and continue
Blank first name
Error message should display
TC_013
Verify checkout with missing last name
Leave last name empty and continue
Blank last name
Error message should display
TC_014
Verify checkout with missing postal code
Leave postal code empty and continue
Blank postal code
Error message should display
TC_015
Verify order completion
Complete checkout flow and click Finish
Valid checkout data
Confirmation page should show successful order message
TC_016
Verify Cancel on checkout page
Start checkout and click Cancel
Valid cart item
User should return to cart/products page depending on checkout stage
TC_017
Verify product sorting A-Z
Select Name A to Z
Sort dropdown
Products should sort alphabetically ascending
TC_018
Verify product sorting Z-A
Select Name Z to A
Sort dropdown
Products should sort alphabetically descending
TC_019
Verify price sorting low-high
Select Price low to high
Sort dropdown
Products should sort by price ascending
TC_020
Verify price sorting high-low
Select Price high to low
Sort dropdown
Products should sort by price descending
TC_021
Verify hamburger menu opens
Click menu icon
Logged in user
Sidebar menu should open
TC_022
Verify logout
Open menu and click Logout
Logged in user
User should return to login page
TC_023
Verify reset app state
Add product, open menu, click Reset App State
Any product
Cart should reset and product buttons should return to Add to Cart
TC_024
Verify About link
Open menu and click About
Logged in user
User should navigate to Sauce Labs website
TC_025
Verify cart persists during navigation
Add item, open product page, return to products
Any product
Cart badge should still show selected item
TC_026
Verify Remove from cart page
Add product, open cart, click Remove
Any product
Product should be removed from cart
TC_027
Verify Continue Shopping button
Open cart and click Continue Shopping
Logged in user
User should return to Products page
TC_028
Verify social links
Click Twitter/X, Facebook, LinkedIn icons
Footer links
Correct external social pages should open
TC_029
Verify responsive layout
Open app on mobile/tablet/desktop sizes
Different viewports
UI should remain usable without overlap
TC_030
Verify session behavior after refresh
Login, refresh browser
standard_user
User should remain on or return appropriately to authenticated product page


Please refer to this document :[https://docs.google.com/document/d/1USQdOjR0CKYEnXt8xZX7ZYDW4yuxlsGdWeTAkKIO_to/edit?tab=t.0](url)





 

