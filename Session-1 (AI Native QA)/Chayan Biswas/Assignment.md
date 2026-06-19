Member: Chayan Biswas
URL: https://demowebshop.tricentis.com/ 

Manual Test Cases:

TC001: Successful Opening of the Website 
Open Browser ( Chrome \ Safari \ Firefox \ Opera..)
Enter the URL: https://demowebshop.tricentis.com/ 
Expected Result : Website should launch successfully.

TC002: Registration of the Website 
Open any Browser , Enter the link 
Click on “Register” link from top 
Registration Page should open - Demo Web Shop. Register 
Fill up the personal details with valid data.
Gender : Radio button : Male\Female - Male
First Name : Textbox : Enter Users First Name - John
Last Name : Textbox : Enter Users Last Name  - Doe
Email : Textbox : Enter New Users Registration Mail Address - johndoe26@yopmail.com 
Password : Textbox : Enter a valid alpha-numeric  ,  case sensitive and length verified password - cc@Test26
Confirm Password : Textbox : Enter Same data as entered in password field - cc@Test26
Click on Register Button
Expected Result : Users Registration should be done successfully.


TC003: Login of the Website 
Open any Browser , Enter the link 
Click on “Log in" link from top 
Log in  Page should open - Demo Web Shop. Login 
Enter the credentials 
Email : Textbox: Enter previously registered email address - johndoe26@yopmail.com 
Password : Textbox : Enter user’s password associated with the id. - cc@Test26
Remember Me : Checkbox : Stores users session
Click on the Login button
Expected Result : User’Should be Logged In into the system .

TC004: If User Don’t Remember his\her Password 
Go to the Login Page. 
Click on Forgot password? Link  
Forgot Password page should open - Demo Web Shop. Password Recovery 
Email : Textbox : Enter users previously registered password of the website - johndoe26@yopmail.com 
Click on recover button 
Now Open users email address , click on reset password link 
Enter Valid and Desired  and also same data in Password and Confirm Password field - ai@Test26

Expected Result : User  should recover his\er account. 



TC005: Opening of Category
Open the website 
Click on any category form header link Books \ Computers \ Electronics \ Apparel & Shoes \ Digital downloads \Jewelry \ Gift Cards
Check for any sub-category is there or not , then click on it
Expected Result : Desired Page should be opened.


TC006: Filter and Sorting of the Product 
Open the website.
Choose any Category \ Sub-Category 
Choose Available  Filter Options
Choose Available  Sorting Options
Expected Result : Desired Product should be displayed in an orderly manner. 


TC007: Go to the Product Details Page 
Open the website.
Choose any Category \ Sub-Category 
Choose Available  Filter \ Sorting  Options
Click on the particular product from the list
Expected Result : Desired Product’s details page should be displayed. 

TC008: Search Any Product 
Open the website. 
Click on the search icon 
Enter desired keyword in the textbox - camera 
Click on search button 
Expected Result : Desired  search result  should be displayed. 


TC009: Add a Product into Cart 
Open the website.
Search for a product 
From the list click on add to cart 
Go to the PDP 
Click on add to cart 

Expected Result : Desired  Product should be added in to cart 


TC010: E -2- E flow of the website 
Open the website. In any browser 
Successfully registered 
Logged in into system 
Look for a particular product on the website. 
Add it into cart 
Go to the cart page 
Accept T&C checkbox and click on checkout button
Fill out all the required information
Choose payment option 
Enter Valid Credit Card data
Click on confirm after enter all the section with valid data 

Expected Result : Order should be successfully placed 

—------------------------------------------------------------------------------
AI Generated Test Cases 

Application: Demo Web Shop
 URL: https://demowebshop.tricentis.com/

Test Suite: Demo Web Shop Website
Module 1: Website Launch / Accessibility
TC ID
Test Scenario
Test Steps
Test Data
Expected Result
Type
TC001-P01
Verify website opens successfully
Open browser → Enter URL
https://demowebshop.tricentis.com
Website should load successfully
Positive
TC001-P02
Verify website works on multiple browsers
Open Chrome, Firefox, Edge, Safari
Different browsers
Website should display correctly
Positive
TC001-N01
Open invalid URL
Enter wrong URL
demowebshop.tricentis.co
Error page should display
Negative
TC001-N02
Verify website during server issue
Access when server unavailable
N/A
Proper error message should display
Negative
TC001-N03
Verify page load performance
Open website
N/A
Page should load within acceptable time
Performance


Module 2: User Registration
Positive Test Cases
TC ID
Scenario
Test Data
Expected Result
TC002-P01
Register user with valid data
John Doe / johndoe26@yopmail.com / cc@Test26
User registration successful
TC002-P02
Register with Male gender
Male selected
Male radio button selected
TC002-P03
Register with Female gender
Female selected
Female radio button selected
TC002-P04
Verify confirmation password
Password=cc@Test26 Confirm=cc@Test26
Registration successful
TC002-P05
Verify registered user login
Registered email/password
User logged in


Negative Test Cases
TC ID
Scenario
Test Data
Expected Result
TC002-N01
Register without selecting gender
Blank gender
Validation message displayed
TC002-N02
First name empty
Blank
"First name required" message
TC002-N03
Last name empty
Blank
"Last name required" message
TC002-N04
Invalid email format
abc@test
Email validation message
TC002-N05
Existing email registration
Existing user email
Duplicate email error
TC002-N06
Password less than minimum length
abc
Password validation message
TC002-N07
Password without uppercase
test123
Password policy error
TC002-N08
Password without number
Testabc
Password policy error
TC002-N09
Password mismatch
Test123 / Test456
Password mismatch message
TC002-N10
Enter special characters in name
@@@
Validation should appear


Module 3: Login
Positive Test Cases
TC ID
Scenario
Expected Result
TC003-P01
Login with valid credentials
User successfully logged in
TC003-P02
Login with Remember Me checked
Session should persist
TC003-P03
Login after registration
Dashboard/home page displayed


Negative Test Cases
TC ID
Scenario
Expected Result
TC003-N01
Login with invalid email
Error message displayed
TC003-N02
Login with wrong password
Invalid credentials message
TC003-N03
Login with blank email
Required field validation
TC003-N04
Login with blank password
Required field validation
TC003-N05
Login using unregistered email
Account not found message
TC003-N06
Enter SQL injection in email
Input should be rejected

Example:
' OR '1'='1

Module 4: Forgot Password
Positive Test Cases
TC ID
Scenario
Expected Result
TC004-P01
Forgot password with registered email
Reset link generated
TC004-P02
Reset password successfully
New password saved
TC004-P03
Login with new password
Login successful


Negative Test Cases
TC ID
Scenario
Expected Result
TC004-N01
Forgot password with invalid email
Error displayed
TC004-N02
Blank email submission
Validation displayed
TC004-N03
Reset password mismatch
Password mismatch error
TC004-N04
Old password login after reset
Login should fail


Module 5: Category Navigation
Positive Test Cases
TC ID
Scenario
Expected Result
TC005-P01
Click Books category
Books page opens
TC005-P02
Click Computers category
Computers page opens
TC005-P03
Click Electronics category
Electronics page opens
TC005-P04
Open sub-category
Correct product list displayed


Negative Test Cases
TC ID
Scenario
Expected Result
TC005-N01
Click unavailable category URL
Proper error page
TC005-N02
Broken category link
Page should not break


Module 6: Product Filter & Sorting
Positive Test Cases
TC ID
Scenario
Expected Result
TC006-P01
Filter by category
Correct products displayed
TC006-P02
Filter by price
Products within price range
TC006-P03
Sort by Price Low-High
Ascending order
TC006-P04
Sort by Price High-Low
Descending order
TC006-P05
Sort Alphabetically A-Z
Products sorted correctly


Negative Test Cases
TC ID
Scenario
Expected Result
TC006-N01
Apply unavailable filter
No result message
TC006-N02
Multiple conflicting filters
Correct handling
TC006-N03
Invalid price range
Validation message


Module 7: Product Details Page
Positive Test Cases
TC ID
Scenario
Expected Result
TC007-P01
Open product page
Product details displayed
TC007-P02
Verify product image
Image visible
TC007-P03
Verify price
Correct price displayed
TC007-P04
Verify description
Description available


Negative Test Cases
TC ID
Scenario
Expected Result
TC007-N01
Open deleted product URL
Product unavailable message
TC007-N02
Broken product image
Placeholder displayed


Module 8: Search Functionality
Positive Test Cases
TC ID
Scenario
Expected Result
TC008-P01
Search valid product
Matching product displayed
TC008-P02
Search partial keyword
Related results displayed
TC008-P03
Search multiple words
Relevant products displayed


Negative Test Cases
TC ID
Scenario
Expected Result
TC008-N01
Search blank keyword
Validation/message displayed
TC008-N02
Search invalid product
No result found
TC008-N03
Search special characters
System should handle safely


Module 9: Add To Cart
Positive Test Cases
TC ID
Scenario
Expected Result
TC009-P01
Add product from listing page
Product added
TC009-P02
Add product from PDP
Product added
TC009-P03
Increase quantity
Quantity updated
TC009-P04
Remove product from cart
Product removed


Negative Test Cases
TC ID
Scenario
Expected Result
TC009-N01
Add without selecting required option
Validation displayed
TC009-N02
Add quantity 0
Error displayed
TC009-N03
Add negative quantity
System rejects
TC009-N04
Add unavailable product
Cannot add


Module 10: Checkout / E2E Flow
Complete Positive E2E Test Case
TC010-P01: Successful Purchase Journey
Steps:
Open website
Register new user
Login
Search product
Open Product Details Page
Add product to cart
Open cart
Accept Terms & Conditions
Click Checkout
Enter billing details
Select shipping method
Select payment method
Enter card details
Confirm order
Test Data:
Name:
John Doe

Email:
johndoe26@yopmail.com

Password:
cc@Test26

Card:
Valid Credit Card
Expected Result:
Order should be successfully placed.
Order confirmation number should generate.
Email confirmation should be sent.

Negative E2E Test Cases
TC ID
Scenario
Expected Result
TC010-N01
Checkout without login
User redirected to login
TC010-N02
Checkout without cart item
Checkout unavailable
TC010-N03
Checkout without accepting T&C
User cannot proceed
TC010-N04
Invalid billing information
Validation message
TC010-N05
Invalid credit card
Payment failed message
TC010-N06
Expired card details
Transaction rejected
TC010-N07
Network failure during payment
Proper error handling
TC010-N08
Refresh payment page
Order duplication prevented


Security Test Cases
TC ID
Scenario
Expected Result
SEC001
SQL Injection attempt
Input blocked
SEC002
XSS Script input
Script should not execute
SEC003
Password masking
Password hidden
SEC004
Session timeout
User logged out
SEC005
Unauthorized cart access
Access denied


Final E2E Business Flow
Launch Website
       |
Registration
       |
Login
       |
Browse Category
       |
Search Product
       |
Apply Filter/Sorting
       |
View Product Details
       |
Add To Cart
       |
Checkout
       |
Payment
       |
Order Confirmation


