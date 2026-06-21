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
 Click 






 


