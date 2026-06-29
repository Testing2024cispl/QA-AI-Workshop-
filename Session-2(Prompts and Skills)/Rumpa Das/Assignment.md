QA Manual test cases--------------------
https://grocerystoredemo.pcubeweb.com/
https://grocerystoredemo.pcubeweb.com/


Member :-Rumpa Das 
Query/Test cases:- 
Human Thinking Test Cases 
TestCases_001:- 
Navigate to https://grocerystoredemo.pcubeweb.com/ 
Click on categories banner
Verify that the page is getting redirected to the categories page & all available categories are displayed


TestCases_002:- 
Open the categories page
Click on any category (health-care,grocery-staples,drinking-water,beverages,pet-food-accessories,breakfast-packaged-food,personal-care,dairy-products,baby products,spices)
Verify that the page is getting redirected to the selected category page

TestCases_003:- 
Open the categories page
Verify that all required product name & images are displayed
TestCases_004:- 
Open the categories page
Click on any category (health-care,grocery-staples,drinking-water,beverages,pet-food-accessories,breakfast-packaged-food,personal-care,dairy-products,baby products,spices)
Verify that all required product name & images are displayed along with add button
TestCases_005:- 
Open the categories page
Refresh the page
Verify that all required product name & images are displayed properly
TestCases_006:- 
Navigate to https://grocerystoredemo.pcubeweb.com/ 
Click on view all for all categories
Verify that all required product name & images are displayed properly

AI  driven test cases for category module -

TC ID
Test Scenario
Steps
Expected Result


CAT_E2E_001
Verify Categories page loads
Click Categories from menu
Categories page opens successfully


CAT_E2E_002
Verify all categories are displayed
Navigate to Categories page
All categories are visible


CAT_E2E_003
Verify category navigation
Click each category one by one
User navigates to correct category page


CAT_E2E_004
Verify category URL accessibility
Open category URL directly
Category page loads correctly


CAT_E2E_005
Verify products display under category
Open Biscuits & Snacks category
Products are displayed with image, name, price and Add button


CAT_E2E_006
Verify "View All" functionality
Click View All for any category
Complete product list is displayed


CAT_E2E_007
Verify Add to Cart from category
Click ADD on product
Product added to cart


CAT_E2E_008
Verify cart count update
Add product from category
Cart badge count updates


CAT_E2E_009
Verify multiple products addition
Add products from different categories
All products appear in cart


CAT_E2E_010
Verify same product quantity increment
Add same product multiple times
Quantity increases appropriately


CAT_E2E_011
Verify product price display
Open multiple categories
Correct price displayed for all products


CAT_E2E_012
Verify product image loading
Open category page
Product images load without broken image


CAT_E2E_013
Verify search within categories
Search product name
Matching products appear


CAT_E2E_014
Verify invalid search
Search random string
No products found message appears


CAT_E2E_015
Verify category refresh behavior
Refresh category page
Data persists correctly


CAT_E2E_016
Verify navigation back to Home
Navigate category → Home
Home page opens successfully


CAT_E2E_017
Verify cart persistence
Add product → navigate categories
Product remains in cart


CAT_E2E_018
Verify responsive category view
Open in mobile viewport
Categories display correctly


CAT_E2E_019
Verify empty cart after logout
Logout and login again
Cart behavior as per business rule


CAT_E2E_020
Verify category page performance
Open categories repeatedly
Page loads within acceptable time



My Account:-
Human Thinking Test Cases 
TestCases_007:-
Navigate to https://grocerystoredemo.pcubeweb.com/ 
Click on account icon
Verify that the sign in pop up is displayed along with mobile number text field & send OTP button & terms & condition & privacy policy link & close icon.

TestCases_008:-
Navigate to https://grocerystoredemo.pcubeweb.com/ 
Click on account icon
Enter the valid data in mobile number textfield
Check that mobile number textfield accepts only numeric data
TestCases_009:-
Navigate to https://grocerystoredemo.pcubeweb.com/ 
Click on account icon
Enter the valid data in mobile number textfield
Check that mobile number textfield accepts only numeric data

TestCases_010:-
Navigate to https://grocerystoredemo.pcubeweb.com/ 
Click on account icon
Click on the close icon
Check that the sign in pop up is being closed.
TestCases_011:-
Navigate to https://grocerystoredemo.pcubeweb.com/ 
Click on account icon
Enter the valid data in mobile number textfield &click on send OTP button
Check that user should receive the OTP for the given mobile number
TestCases_012:-
Navigate to https://grocerystoredemo.pcubeweb.com/ 
Click on account icon
Enter the valid data in mobile number textfield &click on send OTP button
Use the received OTP in the OTP verification pop up within given time
Verify that the page is getting redirected to the user account page
TestCases_013:-
Navigate to https://grocerystoredemo.pcubeweb.com/ 
Click on account icon
Enter the valid data in mobile number textfield &click on send OTP button
Do not put the received OTP in the OTP verification pop up until the timer is being stopped
Verify that the OTP verification pop up should be vanished

TestCases_014:- 

Click on account icon 
Verify that the sign in pop up is displayed along with the mobile number textfield & send OTP button
Enter the phone number & click on send OTP button
Enter the OTP in OTP verification pop up & click on submit button
Go to my addresses tab 
Click on my address tab
Click on the add address icon
Verify that add new address pop up is displayed
Enter the data in all required fields (Name,Mobile Number,Address,Pincode,City,State)
Click on add address button
 Verify that address is added in the my address section
AI  driven test cases for my account module -

TC ID
Test Scenario
Steps
Expected Result
ACC_E2E_001
Verify Account page opens
Click Account
Account page opens successfully
ACC_E2E_002
Verify Registration page
Click Register
Registration form displayed
ACC_E2E_003
Verify successful registration
Enter valid data and submit
Account created successfully
ACC_E2E_004
Verify registration with empty fields
Leave mandatory fields blank
Validation messages displayed
ACC_E2E_005
Verify registration with invalid email
Enter invalid email format
Error message displayed
ACC_E2E_006
Verify duplicate email registration
Register with existing email
Appropriate error displayed
ACC_E2E_007
Verify successful login
Login with valid credentials
User logged in successfully
ACC_E2E_008
Verify invalid login
Login with wrong credentials
Error message displayed
ACC_E2E_009
Verify login with empty fields
Submit blank form
Validation displayed
ACC_E2E_010
Verify logout functionality
Click Logout
User logged out
ACC_E2E_011
Verify Forgot Password page
Click Forgot Password
Reset page displayed
ACC_E2E_012
Verify password reset request
Submit registered email
Reset link/email sent
ACC_E2E_013
Verify profile information display
Open profile section
Correct user information displayed
ACC_E2E_014
Verify profile update
Modify account details
Changes saved successfully
ACC_E2E_015
Verify password change
Update password
New password accepted
ACC_E2E_016
Verify login using new password
Login with updated password
Login successful
ACC_E2E_017
Verify order history page
Open Order History
Previous orders displayed
ACC_E2E_018
Verify order details
Open specific order
Order information displayed correctly
ACC_E2E_019
Verify unauthorized access
Open account URL without login
Redirect to login page
ACC_E2E_020
Verify session persistence
Refresh browser after login
User remains logged in
ACC_E2E_021
Verify session timeout
Keep session idle
Proper session handling occurs
ACC_E2E_022
Verify account page responsiveness
Open on mobile/tablet
Layout remains usable
ACC_E2E_023
Verify account data security
Access another user's account URL
Access denied
ACC_E2E_024
Verify special characters validation
Enter special chars in profile fields
Validation handled correctly
ACC_E2E_025
Verify maximum field length validation
Enter maximum length values
Proper validation displayed

-------------------------------Session 2---------------------------------------------------------------------

# Category & My Account Test Cases Skill

Member: Rumpa Das

## Overview
This skill file contains manual and AI-driven test cases for the Category and My Account modules of the Grocery Store Demo: https://grocerystoredemo.pcubeweb.com/

---

## Category Module — Human Thinking Test Cases

- **TestCases_001**: Navigate to https://grocerystoredemo.pcubeweb.com/ → Click on categories banner → Verify redirect to categories page and that all available categories are displayed.

- **TestCases_002**: Open the categories page → Click any category (health-care, grocery-staples, drinking-water, beverages, pet-food-accessories, breakfast-packaged-food, personal-care, dairy-products, baby products, spices) → Verify redirect to the selected category page.

- **TestCases_003**: Open the categories page → Verify that all required product names & images are displayed.

- **TestCases_004**: Open the categories page → Click any category (list above) → Verify that products show name, image and Add button.

- **TestCases_005**: Open the categories page → Refresh the page → Verify that all required product names & images are displayed properly.

- **TestCases_006**: Navigate to https://grocerystoredemo.pcubeweb.com/ → Click "View All" for all categories → Verify that all required product names & images are displayed properly.

## Category Module — AI-driven Test Cases (E2E)

TC ID | Test Scenario | Steps | Expected Result
---|---:|---|---
CAT_E2E_001 | Verify Categories page loads | Click Categories from menu | Categories page opens successfully
CAT_E2E_002 | Verify all categories are displayed | Navigate to Categories page | All categories are visible
CAT_E2E_003 | Verify category navigation | Click each category one by one | User navigates to correct category page
CAT_E2E_004 | Verify category URL accessibility | Open category URL directly | Category page loads correctly
CAT_E2E_005 | Verify products display under category | Open Biscuits & Snacks category | Products are displayed with image, name, price and Add button
CAT_E2E_006 | Verify "View All" functionality | Click View All for any category | Complete product list is displayed
CAT_E2E_007 | Verify Add to Cart from category | Click ADD on product | Product added to cart
CAT_E2E_008 | Verify cart count update | Add product from category | Cart badge count updates
CAT_E2E_009 | Verify multiple products addition | Add products from different categories | All products appear in cart
CAT_E2E_010 | Verify same product quantity increment | Add same product multiple times | Quantity increases appropriately
CAT_E2E_011 | Verify product price display | Open multiple categories | Correct price displayed for all products
CAT_E2E_012 | Verify product image loading | Open category page | Product images load without broken image
CAT_E2E_013 | Verify search within categories | Search product name | Matching products appear
CAT_E2E_014 | Verify invalid search | Search random string | No products found message appears
CAT_E2E_015 | Verify category refresh behavior | Refresh category page | Data persists correctly
CAT_E2E_016 | Verify navigation back to Home | Navigate category → Home | Home page opens successfully
CAT_E2E_017 | Verify cart persistence | Add product → navigate categories | Product remains in cart
CAT_E2E_018 | Verify responsive category view | Open in mobile viewport | Categories display correctly
CAT_E2E_019 | Verify empty cart after logout | Logout and login again | Cart behavior as per business rule
CAT_E2E_020 | Verify category page performance | Open categories repeatedly | Page loads within acceptable time

---

## My Account — Human Thinking Test Cases

- **TestCases_007**: Navigate to https://grocerystoredemo.pcubeweb.com/ → Click on account icon → Verify sign-in popup is displayed with mobile number field, Send OTP button, Terms & Conditions & Privacy Policy links, and close icon.

- **TestCases_008**: Open account popup → Enter mobile number → Verify mobile field accepts only numeric data.

- **TestCases_009**: (Duplicate of 008) Ensure mobile number input restricts to numeric data.

- **TestCases_010**: Open account popup → Click close icon → Verify pop-up closes.

- **TestCases_011**: Open account popup → Enter valid mobile number → Click Send OTP → Verify OTP is sent to given mobile number.

- **TestCases_012**: Open account popup → Send OTP → Enter received OTP within timer → Verify redirect to user account page.

- **TestCases_013**: Open account popup → Send OTP → Do not enter OTP until timer expires → Verify OTP verification popup vanishes.

- **TestCases_014**: End-to-end address add flow: Open account popup → Sign in → Go to My Addresses → Click Add Address → Verify add address popup appears → Fill Name, Mobile, Address, Pincode, City, State → Click Add Address → Verify address is added to My Addresses.

## My Account — AI-driven Test Cases (E2E)

TC ID | Test Scenario | Steps | Expected Result
---|---:|---|---
ACC_E2E_001 | Verify Account page opens | Click Account | Account page opens successfully
ACC_E2E_002 | Verify Registration page | Click Register | Registration form displayed
ACC_E2E_003 | Verify successful registration | Enter valid data and submit | Account created successfully
ACC_E2E_004 | Verify registration with empty fields | Leave mandatory fields blank | Validation messages displayed
ACC_E2E_005 | Verify registration with invalid email | Enter invalid email format | Error message displayed
ACC_E2E_006 | Verify duplicate email registration | Register with existing email | Appropriate error displayed
ACC_E2E_007 | Verify successful login | Login with valid credentials | User logged in successfully
ACC_E2E_008 | Verify invalid login | Login with wrong credentials | Error message displayed
ACC_E2E_009 | Verify login with empty fields | Submit blank form | Validation displayed
ACC_E2E_010 | Verify logout functionality | Click Logout | User logged out
ACC_E2E_011 | Verify Forgot Password page | Click Forgot Password | Reset page displayed
ACC_E2E_012 | Verify password reset request | Submit registered email | Reset link/email sent
ACC_E2E_013 | Verify profile information display | Open profile section | Correct user information displayed
ACC_E2E_014 | Verify profile update | Modify account details | Changes saved successfully
ACC_E2E_015 | Verify password change | Update password | New password accepted
ACC_E2E_016 | Verify login using new password | Login with updated password | Login successful
ACC_E2E_017 | Verify order history page | Open Order History | Previous orders displayed
ACC_E2E_018 | Verify order details | Open specific order | Order information displayed correctly
ACC_E2E_019 | Verify unauthorized access | Open account URL without login | Redirect to login page
ACC_E2E_020 | Verify session persistence | Refresh browser after login | User remains logged in
ACC_E2E_021 | Verify session timeout | Keep session idle | Proper session handling occurs
ACC_E2E_022 | Verify account page responsiveness | Open on mobile/tablet | Layout remains usable
ACC_E2E_023 | Verify account data security | Access another user's account URL | Access denied
ACC_E2E_024 | Verify special characters validation | Enter special chars in profile fields | Validation handled correctly
ACC_E2E_025 | Verify maximum field length validation | Enter maximum length values | Proper validation displayed

---

## Notes
- URLs used: https://grocerystoredemo.pcubeweb.com/
- Member: Rumpa Das







