QA Manual Test Cases:-

Member: Akash Jaiswal

# _Human Thinking Test Cases_

# TestCases

## 001:-

\_

- Go to <https://www.saucedemo.com/>
- Enter valid username "standard_user"
- Enter valid password "secret_sauce"
- Click on the Login button
- Verify that the user is logged in successfully and redirected to the Inventory page ("/inventory.html")
- Verify that the header title "Swag Labs" and the shopping cart icon are visible

## 002:-

\_

- Go to <https://www.saucedemo.com/>
- Enter an invalid username "invalid_user"
- Enter a valid password "secret_sauce"
- Click on the Login button
- Verify that an error message is displayed: "Username and password do not match any user in this service"

## 003:-

\_

- Go to <https://www.saucedemo.com/>
- Enter valid username "standard_user"
- Enter an invalid password "wrong_password"
- Click on the Login button
- Verify that an error message is displayed: "Username and password do not match any user in this service"

## 004:-

\_

- Go to <https://www.saucedemo.com/>
- Leave the username field empty
- Enter a valid password "secret_sauce"
- Click on the Login button
- Verify that an error message is displayed: "Username is required"

## 005:-

\_

- Go to <https://www.saucedemo.com/>
- Enter valid username "standard_user"
- Leave the password field empty
- Click on the Login button
- Verify that an error message is displayed: "Password is required"

## 006:-

\_

- Go to <https://www.saucedemo.com/>
- Enter the locked-out username "locked_out_user"
- Enter valid password "secret_sauce"
- Click on the Login button
- Verify that an error message is displayed: "Sorry, this user has been locked out."

#

007:-

\_

- Go to <https://www.saucedemo.com/>
- Enter valid username "standard_user"
- Enter valid password "secret_sauce"
- Click on the Login button
- Click on the "Add to cart" button for "Sauce Labs Backpack"
- Verify that the button text changes to "Remove"
- Verify that the shopping cart badge shows a count of "1"
- Click on the "Remove" button for the same item from the Inventory page
- Verify that the button text changes back to "Add to cart"
- Verify that the shopping cart badge is cleared or decremented

## 008:-

\_

- Go to <https://www.saucedemo.com/>
- Enter valid username "standard_user"
- Enter valid password "secret_sauce"
- Click on the Login button
- Click on the sorting dropdown menu
- Select "Name (A to Z)"
- Verify that the product listing sorts in ascending alphabetical order
- Click on the sorting dropdown menu
- Select "Name (Z to A)"
- Verify that the product listing sorts in descending alphabetical order
- Click on the sorting dropdown menu
- Select "Price (low to high)"
- Verify that the product listing sorts based on price from the cheapest item to the most expensive item
- Click on the sorting dropdown menu
- Select "Price (high to low)"
- Verify that the product listing sorts based on price from the most expensive item to the cheapest item

## 009:-

\_

- Go to <https://www.saucedemo.com/>
- Enter valid username "error_user"
- Enter valid password "secret_sauce"
- Click on the Login button
- Click on the sorting dropdown menu
- Select "Name (A to Z)"
- Verify that an error message is displayed: "Sorting is broken! This error has been reported to Backtrace."

## 010:-

\_

- Go to <https://www.saucedemo.com/>
- Enter valid username "standard_user"
- Enter valid password "secret_sauce"
- Click on the Login button
- Navigate directly to the Cart page and click "Checkout"
- Leave "First Name", "Last Name", and "Zip/Postal Code" empty
- Click on the "Continue" button
- Verify that an error message is displayed: "Error: First Name is required"
- Enter a valid First Name
- Leave "Last Name" and "Zip/Postal Code" empty
- Click on the "Continue" button
- Verify that an error message is displayed: "Error: Last Name is required"
- Enter a valid Last Name
- Leave "Zip/Postal Code" empty
- Click on the "Continue" button
- Verify that an error message is displayed: "Error: Postal Code is required"

## 011:-

\_

- Go to <https://www.saucedemo.com/>
- Enter valid username "standard_user"
- Enter valid password "secret_sauce"
- Click on the Login button
- Navigate to the Checkout Information page
- Click on the "Cancel" button
- Verify that the user is taken back to the Cart page ("/cart.html")

## 012:-

\_

- Go to <https://www.saucedemo.com/>
- Enter valid username "standard_user"
- Enter valid password "secret_sauce"
- Click on the Login button
- Click on the "Add to cart" button for "Sauce Labs Backpack"
- Navigate directly to the Cart page and click "Checkout"
- Enter a valid First Name
- Enter a valid Last Name
- Enter a valid Zip Code
- Click on the Continue button
- Verify that the user is navigated to the Checkout: Overview page ("/checkout-step-two.html")
- Verify that the "Payment Information", "Shipping Information", "Item total", "Tax", and "Total" fields are accurately calculated and displayed

## 013:-

\_

- Go to <https://www.saucedemo.com/>
- Enter valid username "standard_user"
- Enter valid password "secret_sauce"
- Click on the Login button
- Click on the "Add to cart" button for "Sauce Labs Backpack"
- Navigate directly to the Cart page and click "Checkout"
- Enter a valid First Name
- Enter a valid Last Name
- Enter a valid Zip Code
- Click on the Continue button
- Verify that the user is navigated to the Checkout: Overview page ("/checkout-step-two.html")
- Click on the Cancel button
- Verify that the user is taken back to the Cart page ("/cart.html")

## 014:-

\_

- Go to <https://www.saucedemo.com/>
- Enter valid username "standard_user"
- Enter valid password "secret_sauce"
- Click on the Login button
- Click on the "Add to cart" button for "Sauce Labs Backpack"
- Navigate directly to the Cart page and click "Checkout"
- Enter a valid First Name
- Enter a valid Last Name
- Enter a valid Zip Code
- Click on the Continue button
- Verify that the user is navigated to the Checkout: Overview page ("/checkout-step-two.html")
- Click on the Finish button
- Verify that the user is taken back to the Checkout Complete page ("/checkout-complete.html")
- Verify that a success message "Thank you for your order!" is visible

## 015:-

\_

- Go to <https://www.saucedemo.com/>
- Enter valid username "standard_user"
- Enter valid password "secret_sauce"
- Click on the Login button
- Click on the hamburger menu icon (three lines) in the top-left corner
- Verify that the sidebar navigation panel slides open smoothly
- Verify that four links are visible: "All Items", "About", "Logout", and "Reset App State"

## 016:-

\_

- Go to <https://www.saucedemo.com/>
- Enter valid username "standard_user"
- Enter valid password "secret_sauce"
- Click on the Login button
- Click on the hamburger menu icon
- Click on the "About" link
- Verify that the user is redirected to the official Sauce Labs company website landing page ("<https://saucelabs.com/>")

## 017:-

\_

- Go to <https://www.saucedemo.com/>
- Enter valid username "standard_user"
- Enter valid password "secret_sauce"
- Click on the Login button
- Click on the "Add to cart" button for any item
- Click on the hamburger menu icon
- Click on the "Reset App State" link
- Verify that the shopping cart badge count disappears and the item button changes back to "Add to cart"

## 018:-

\_

- Go to <https://www.saucedemo.com/>
- Enter valid username "standard_user"
- Enter valid password "secret_sauce"
- Click on the Login button
- Click on the hamburger menu icon
- Click on the "Logout" link
- Verify that the user is safely logged out and redirected back to the root Login page ("<https://www.saucedemo.com/>")

## 019:-

\_

- Go to <https://www.saucedemo.com/>
- Enter valid username "standard_user"
- Enter valid password "secret_sauce"
- Click on the Login button
- Verify that the user is logged in successfully and redirected to the Inventory page ("/inventory.html")
- Verify that the header title "Swag Labs" and the shopping cart icon are visible
- Click on the "Add to cart" button for "Sauce Labs Backpack"
- Verify that the button text changes to "Remove"
- Verify that the shopping cart badge shows a count of "1"
- Click on the hamburger icon
- Verify Logout Option is displayed
- Click on Logout
- Verify that page redirects to Logout page
- Enter valid username "standard_user"
- Enter valid password "secret_sauce"
- Click on the Login button
- Verify that the user is logged in successfully and redirected to the Inventory page ("/inventory.html")
- Verify that the header title "Swag Labs" and the shopping cart icon are visible
- Verify that the shopping cart badge shows a count of "1"

## 020:-

\_

- Go to <https://www.saucedemo.com/>
- Enter valid username "standard_user"
- Enter valid password "secret_sauce"
- Click on the Login button
- Verify that the user is logged in successfully and redirected to the Inventory page ("/inventory.html")
- Verify that the header title "Swag Labs" and the shopping cart icon are visible
- Click on the "Add to cart" button for "Sauce Labs Backpack"
- Verify that the button text changes to "Remove"
- Verify that the shopping cart badge shows a count of "1"
- Click on the hamburger icon
- Verify Logout Option is displayed
- Click on Logout
- Verify that page redirects to Logout page
- Enter valid username "error_user"
- Enter valid password "secret_sauce"
- Click on the Login button
- Verify that the user is logged in successfully and redirected to the Inventory page ("/inventory.html")
- Verify that the header title "Swag Labs" and the shopping cart icon are visible
- Verify that the shopping cart badge is clear

#

_AI Manual Test Cases_

## Model: Gimini 3 Flash

## Prompt

Create a list of all the functional test cases for this URL "<https://www.saucedemo.com/>" explore all the possible routes and provide the response in this format

TestCases

001:-

\_

1\. Go to Amazon.com

2\. Click on Sign In

3\. Enter a valid registered email/mobile number

4\. Click on Continue

5\. Enter a valid password

6\. Click on Sign In

7\. Verify that the user is logged in successfully

8\. Verify that the Account & Lists section displays the logged-in

user name

##

TestCases

## 001:-

\_

- Go to <https://www.saucedemo.com/>
- Enter valid username "standard_user"
- Enter valid password "secret_sauce"
- Click on the Login button
- Verify that the user is logged in successfully and redirected to the Inventory page ("/inventory.html")
- Verify that the header title "Swag Labs" and the shopping cart icon are visible

## 002:-

\_

- Go to <https://www.saucedemo.com/>
- Enter an invalid username "invalid_user"
- Enter a valid password "secret_sauce"
- Click on the Login button
- Verify that an error message is displayed: "Epic sadface: Username and password do not match any user in this service"

## 003:-

\_

- Go to <https://www.saucedemo.com/>
- Enter valid username "standard_user"
- Enter an invalid password "wrong_password"
- Click on the Login button
- Verify that an error message is displayed: "Epic sadface: Username and password do not match any user in this service"

## 004:-

\_

- Go to <https://www.saucedemo.com/>
- Leave the username field empty
- Enter a valid password "secret_sauce"
- Click on the Login button
- Verify that an error message is displayed: "Epic sadface: Username is required"

## 005:-

\_

- Go to <https://www.saucedemo.com/>
- Enter valid username "standard_user"
- Leave the password field empty
- Click on the Login button
- Verify that an error message is displayed: "Epic sadface: Password is required"

## 006:-

\_

- Go to <https://www.saucedemo.com/>
- Enter the locked-out username "locked_out_user"
- Enter valid password "secret_sauce"
- Click on the Login button
- Verify that an error message is displayed: "Epic sadface: Sorry, this user has been locked out."

## 007:-

\_

- Go to <https://www.saucedemo.com/>
- Enter valid username "standard_user"
- Enter valid password "secret_sauce"
- Click on the Login button
- Click on the "Add to cart" button for "Sauce Labs Backpack"
- Verify that the button text changes to "Remove"
- Verify that the shopping cart badge shows a count of "1"

## 008:-

\_

- Go to <https://www.saucedemo.com/>
- Enter valid username "standard_user"
- Enter valid password "secret_sauce"
- Click on the Login button
- Click on the "Add to cart" button for multiple items (e.g., Backpack and Bike Light)
- Verify that the shopping cart badge increments correctly to "2"

## 009:-

\_

- Go to <https://www.saucedemo.com/>
- Enter valid username "standard_user"
- Enter valid password "secret_sauce"
- Click on the Login button
- Click on the "Add to cart" button for "Sauce Labs Backpack"
- Click on the "Remove" button for the same item from the Inventory page
- Verify that the button text changes back to "Add to cart"
- Verify that the shopping cart badge is cleared or decremented

## 010:-

\_

- Go to <https://www.saucedemo.com/>
- Enter valid username "standard_user"
- Enter valid password "secret_sauce"
- Click on the Login button
- Click on the "Name (A to Z)" sorting dropdown menu
- Select "Name (Z to A)"
- Verify that the product listing sorts in descending alphabetical order

## 011:-

\_

- Go to <https://www.saucedemo.com/>
- Enter valid username "standard_user"
- Enter valid password "secret_sauce"
- Click on the Login button
- Click on the sorting dropdown menu
- Select "Price (low to high)"
- Verify that the product listing sorts based on price from the cheapest item to the most expensive item

## 012:-

\_

- Go to <https://www.saucedemo.com/>
- Enter valid username "standard_user"
- Enter valid password "secret_sauce"
- Click on the Login button
- Click on the item name link "Sauce Labs Backpack"
- Verify that the user is navigated to the Product Details page ("/inventory-item.html")
- Verify that the product image, description, and correct price are displayed

## 013:-

\_

- Go to <https://www.saucedemo.com/>
- Enter valid username "standard_user"
- Enter valid password "secret_sauce"
- Click on the Login button
- Click on the item name link "Sauce Labs Backpack"
- Click on the "Add to cart" button on the Product Details page
- Verify that the shopping cart badge updates to "1"
- Click on the "Back to products" button and verify redirection to the main Inventory page

## 014:-

\_

- Go to <https://www.saucedemo.com/>
- Enter valid username "standard_user"
- Enter valid password "secret_sauce"
- Click on the Login button
- Click on the shopping cart icon link
- Verify that the user is navigated to the Your Cart page ("/cart.html")
- Verify that the cart displays the title "Your Cart"

## 015:-

\_

- Go to <https://www.saucedemo.com/>
- Enter valid username "standard_user"
- Enter valid password "secret_sauce"
- Click on the Login button
- Click on the "Add to cart" button for "Sauce Labs Backpack"
- Click on the shopping cart icon link
- Verify that the "Sauce Labs Backpack" is displayed in the list on the Cart page with a quantity of 1

## 016:-

\_

- Go to <https://www.saucedemo.com/>
- Enter valid username "standard_user"
- Enter valid password "secret_sauce"
- Click on the Login button
- Click on the "Add to cart" button for "Sauce Labs Backpack"
- Click on the shopping cart icon link
- Click on the "Remove" button next to the item on the Cart page
- Verify that the item is removed from the cart list and the cart badge updates

## 017:-

\_

- Go to <https://www.saucedemo.com/>
- Enter valid username "standard_user"
- Enter valid password "secret_sauce"
- Click on the Login button
- Click on the shopping cart icon link
- Click on the "Continue Shopping" button
- Verify that the user is redirected back to the main Inventory page

## 018:-

\_

- Go to <https://www.saucedemo.com/>
- Enter valid username "standard_user"
- Enter valid password "secret_sauce"
- Click on the Login button
- Click on the "Add to cart" button for "Sauce Labs Backpack"
- Click on the shopping cart icon link
- Click on the "Checkout" button
- Verify that the user is navigated to the Checkout: Your Information page ("/checkout-step-one.html")

## 019:-

\_

- Go to <https://www.saucedemo.com/>
- Enter valid username "standard_user"
- Enter valid password "secret_sauce"
- Click on the Login button
- Navigate directly to the Cart page and click "Checkout"
- Leave "First Name", "Last Name", and "Zip/Postal Code" empty
- Click on the "Continue" button
- Verify that an error message is displayed: "Error: First Name is required"

## 020:-

\_

- Go to <https://www.saucedemo.com/>
- Enter valid username "standard_user"
- Enter valid password "secret_sauce"
- Click on the Login button
- Navigate to the Checkout Information page
- Enter a valid First Name
- Leave "Last Name" and "Zip/Postal Code" empty
- Click on the "Continue" button
- Verify that an error message is displayed: "Error: Last Name is required"

## 021:-

\_

- Go to <https://www.saucedemo.com/>
- Enter valid username "standard_user"
- Enter valid password "secret_sauce"
- Click on the Login button
- Navigate to the Checkout Information page
- Enter a valid First Name and Last Name
- Leave "Zip/Postal Code" empty
- Click on the "Continue" button
- Verify that an error message is displayed: "Error: Postal Code is required"

## 022:-

\_

- Go to <https://www.saucedemo.com/>
- Enter valid username "standard_user"
- Enter valid password "secret_sauce"
- Click on the Login button
- Navigate to the Checkout Information page
- Enter a valid First Name, Last Name, and Postal Code
- Click on the "Cancel" button
- Verify that the user is taken back to the Cart page ("/cart.html")

## 023:-

\_

- Go to <https://www.saucedemo.com/>
- Enter valid username "standard_user"
- Enter valid password "secret_sauce"
- Click on the Login button
- Click on the "Add to cart" button for "Sauce Labs Backpack"
- Navigate to the Checkout Information page, enter all valid info, and click "Continue"
- Verify that the user is navigated to the Checkout: Overview page ("/checkout-step-two.html")
- Verify that the "Payment Information", "Shipping Information", "Item total", "Tax", and "Total" fields are accurately calculated and displayed

## 024:-

\_

- Go to <https://www.saucedemo.com/>
- Enter valid username "standard_user"
- Enter valid password "secret_sauce"
- Click on the Login button
- Progress through the cart and enter checkout details until reaching Checkout: Overview
- Click on the "Cancel" button
- Verify that the transaction is cancelled and the user is redirected to the main Inventory page

## 025:-

\_

- Go to <https://www.saucedemo.com/>
- Enter valid username "standard_user"
- Enter valid password "secret_sauce"
- Click on the Login button
- Progress through to the Checkout: Overview page
- Click on the "Finish" button
- Verify that the user is navigated to the Checkout: Complete page ("/checkout-complete.html")
- Verify that a success message "Thank you for your order!" is visible

## 026:-

\_

- Go to <https://www.saucedemo.com/>
- Enter valid username "standard_user"
- Enter valid password "secret_sauce"
- Click on the Login button
- Complete an order to reach the Checkout: Complete page
- Click on the "Back Home" button
- Verify that the user is redirected to the main Inventory page and the shopping cart badge is completely empty

## 027:-

\_

- Go to <https://www.saucedemo.com/>
- Enter valid username "standard_user"
- Enter valid password "secret_sauce"
- Click on the Login button
- Click on the hamburger menu icon (three lines) in the top-left corner
- Verify that the sidebar navigation panel slides open smoothly
- Verify that four links are visible: "All Items", "About", "Logout", and "Reset App State"

## 028:-

\_

- Go to <https://www.saucedemo.com/>
- Enter valid username "standard_user"
- Enter valid password "secret_sauce"
- Click on the Login button
- Click on the hamburger menu icon
- Click on the "About" link
- Verify that the user is redirected to the official Sauce Labs company website landing page ("<https://saucelabs.com/>")

## 029:-

\_

- Go to <https://www.saucedemo.com/>
- Enter valid username "standard_user"
- Enter valid password "secret_sauce"
- Click on the Login button
- Click on the "Add to cart" button for any item
- Click on the hamburger menu icon
- Click on the "Reset App State" link
- Verify that the shopping cart badge count disappears and the item button changes back to "Add to cart"

## 030:-

\_

- Go to <https://www.saucedemo.com/>
- Enter valid username "standard_user"
- Enter valid password "secret_sauce"
- Click on the Login button
- Click on the hamburger menu icon
- Click on the "Logout" link
- Verify that the user is safely logged out and redirected back to the root Login page ("<https://www.saucedemo.com/>")

## 031:-

\_

- Without logging in, attempt to navigate directly via browser address bar to "[https://www.saucedemo.com/inventory.html](https://www.google.com/search?q=https://www.saucedemo.com/inventory.html)"
- Verify that the access is blocked, and the user is redirected back to the Login page
- Verify that an error message is displayed: "Epic sadface: You can only access '/inventory.html' when you are logged in."

# Your thoughts:-

## What you felt Suitable:-

- **Atomic, single-purpose cases.** The AI split one behaviour per test instead of bundling many
- **Exact, real expected results.** The AI used SauceDemo's actual error strings, including the "Epic sadface:" prefix (e.g. "Epic sadface: Username is required")
- **Consistent, predictable structure.** Every case follows the same "navigate → act → verify" shape with the same login preamble.

## What you felt Not Suitable:-

- **A few imprecise steps.** Case 010 says _"Click on the 'Name (A to Z)' sorting dropdown menu"_, which confuses the dropdown's default value with the dropdown control itself
- **Missed sharp human scenarios.** The AI did not cover the error*user sorting bug (which surfaces *"Sorting is broken! This error has been reported to Backtrace."\_) or the session/cart-persistence behaviour across logout → re-login, and the different-user cart-state case.
- **Overly Literal Step Generation:** It sometimes produces excessively redundant test steps across separate cases rather than building a smart, modularized end-to-end framework layout.

**3\. Final Combined Test Suite - Automation Ready**

The suite below merges both sources: it keeps the AI's atomic structure and exact strings, removes duplicates and the stray Amazon block, and adds back the human-only scenarios. Login is defined once as a reusable precondition instead of being repeated in every case.

**Reusable building blocks (define once in code, e.g. as fixtures / Page Objects):**

- **PRECOND-A - On Login page:** Browser is open at <https://www.saucedemo.com/>.
- **PRECOND-B - Logged in:** PRECOND-A done, then login as standard_user / secret_sauce so the Inventory page (/inventory.html) is shown.
- **Standard test data:** valid user standard_user, password secret_sauce; sample item Sauce Labs Backpack; second item Sauce Labs Bike Light; valid checkout info First=Test, Last=User, Zip=12345.

Notation: each case lists ID · Module · Priority · Precondition · Steps · Expected Result.

**Module 1 - Authentication**

**TC_AUTH_01 · Login · High** Precondition: PRECOND-A Steps: Enter standard_user; enter secret_sauce; click Login. Expected: Redirected to /inventory.html; header title "Swag Labs" and the shopping-cart icon are visible.

**TC_AUTH_02 · Login · High** Precondition: PRECOND-A Steps: Enter invalid_user; enter secret_sauce; click Login. Expected: Error shown: Epic sadface: Username and password do not match any user in this service.

**TC_AUTH_03 · Login · High** Precondition: PRECOND-A Steps: Enter standard_user; enter wrong_password; click Login. Expected: Error shown: Epic sadface: Username and password do not match any user in this service.

**TC_AUTH_04 · Login · Medium** Precondition: PRECOND-A Steps: Leave username empty; enter secret_sauce; click Login. Expected: Error shown: Epic sadface: Username is required.

**TC_AUTH_05 · Login · Medium** Precondition: PRECOND-A Steps: Enter standard_user; leave password empty; click Login. Expected: Error shown: Epic sadface: Password is required.

**TC_AUTH_06 · Login · Medium** Precondition: PRECOND-A Steps: Enter locked_out_user; enter secret_sauce; click Login. Expected: Error shown: Epic sadface: Sorry, this user has been locked out..

**TC_AUTH_07 · Login · Low** Precondition: PRECOND-B Steps: Open hamburger menu; click Logout. Expected: User is logged out and returned to the Login page (<https://www.saucedemo.com/>).

**Module 2 - Inventory / Products**

**TC_INV_01 · Inventory · Medium** Precondition: PRECOND-B Steps: Open the sort dropdown; select "Name (A to Z)". Expected: Products are listed in ascending alphabetical order.

**TC_INV_02 · Inventory · Medium** Precondition: PRECOND-B Steps: Open the sort dropdown; select "Name (Z to A)". Expected: Products are listed in descending alphabetical order.

**TC_INV_03 · Inventory · Medium** Precondition: PRECOND-B Steps: Open the sort dropdown; select "Price (low to high)". Expected: Products are listed cheapest → most expensive.

**TC_INV_04 · Inventory · Medium** Precondition: PRECOND-B Steps: Open the sort dropdown; select "Price (high to low)". Expected: Products are listed most expensive → cheapest.

**TC_INV_05 · Inventory · High (known-bug / negative)** Precondition: PRECOND-A Steps: Login as error*user / secret_sauce; open the sort dropdown; select "Name (A to Z)". Expected: Error surfaces: Sorting is broken! This error has been reported to Backtrace. *(use as a guard test to confirm the broken behaviour is detected.)\_

**TC_INV_06 · Inventory · High** Precondition: PRECOND-B Steps: Click "Add to cart" for Sauce Labs Backpack. Expected: Button changes to "Remove"; cart badge shows 1.

**TC_INV_07 · Inventory · Medium** Precondition: PRECOND-B Steps: Add Sauce Labs Backpack and Sauce Labs Bike Light to cart. Expected: Cart badge increments to 2.

**TC_INV_08 · Inventory · Medium** Precondition: PRECOND-B; backpack already added Steps: Click "Remove" for Sauce Labs Backpack on the Inventory page. Expected: Button reverts to "Add to cart"; cart badge is cleared/decremented.

**TC_INV_09 · Product Detail · Medium** Precondition: PRECOND-B Steps: Click the item name link Sauce Labs Backpack. Expected: Navigated to Product Details (/inventory-item.html); image, description, and correct price are displayed.

**TC_INV_10 · Product Detail · Medium** Precondition: PRECOND-B; on Product Details for backpack Steps: Click "Add to cart"; then click "Back to products". Expected: Cart badge shows 1; user returns to the Inventory page.

**Module 3 - Cart**

**TC_CART_01 · Cart · Medium** Precondition: PRECOND-B Steps: Click the shopping-cart icon. Expected: Navigated to /cart.html; page title "Your Cart" is shown.

**TC_CART_02 · Cart · Medium** Precondition: PRECOND-B; backpack added Steps: Click the shopping-cart icon. Expected: Sauce Labs Backpack is listed on the Cart page with quantity 1.

**TC_CART_03 · Cart · Medium** Precondition: PRECOND-B; backpack added; on Cart page Steps: Click "Remove" next to the item. Expected: Item is removed from the cart list and the cart badge updates.

**TC_CART_04 · Cart · Low** Precondition: PRECOND-B; on Cart page Steps: Click "Continue Shopping". Expected: User is returned to the Inventory page.

**Module 4 - Checkout**

**TC_CHK_01 · Checkout · Medium** Precondition: PRECOND-B; backpack added; on Cart page Steps: Click "Checkout". Expected: Navigated to Checkout: Your Information (/checkout-step-one.html).

**TC_CHK_02 · Checkout · High** Precondition: On Checkout: Your Information page Steps: Leave all three fields empty; click Continue. Expected: Error shown: Error: First Name is required.

**TC_CHK_03 · Checkout · High** Precondition: On Checkout: Your Information page Steps: Enter First Name only; leave Last Name and Zip empty; click Continue. Expected: Error shown: Error: Last Name is required.

**TC_CHK_04 · Checkout · High** Precondition: On Checkout: Your Information page Steps: Enter First and Last Name; leave Zip empty; click Continue. Expected: Error shown: Error: Postal Code is required.

**TC_CHK_05 · Checkout · Low** Precondition: On Checkout: Your Information page Steps: Click Cancel. Expected: User is taken back to the Cart page (/cart.html).

**TC_CHK_06 · Checkout · High** Precondition: PRECOND-B; backpack added; on Checkout: Your Information page Steps: Enter First=Test, Last=User, Zip=12345; click Continue. Expected: Navigated to Checkout: Overview (/checkout-step-two.html); Payment Information, Shipping Information, Item total, Tax, and Total are displayed and correctly calculated.

**TC_CHK_07 · Checkout · Low** Precondition: On Checkout: Overview page Steps: Click Cancel. Expected: User is returned to the Inventory page.

**TC_CHK_08 · Checkout · High** Precondition: On Checkout: Overview page Steps: Click Finish. Expected: Navigated to Checkout: Complete (/checkout-complete.html); success message "Thank you for your order!" is visible.

**TC_CHK_09 · Checkout · Medium** Precondition: On Checkout: Complete page Steps: Click "Back Home". Expected: User is returned to the Inventory page; cart badge is empty.

**Module 5 - Navigation / Side Menu**

**TC_NAV_01 · Menu · Medium** Precondition: PRECOND-B Steps: Click the hamburger menu icon. Expected: Side panel opens; four links are visible - "All Items", "About", "Logout", "Reset App State".

**TC_NAV_02 · Menu · Low** Precondition: PRECOND-B; menu open Steps: Click "About". Expected: User is redirected to <https://saucelabs.com/>.

**TC_NAV_03 · Menu · Medium** Precondition: PRECOND-B; at least one item added Steps: Open hamburger menu; click "Reset App State". Expected: Cart badge count disappears and item buttons revert to "Add to cart".

**Module 6 - Security / Session**

**TC_SEC_01 · Security · High (negative)** Precondition: PRECOND-A (not logged in) Steps: In the address bar, navigate directly to <https://www.saucedemo.com/inventory.html>. Expected: Access is blocked and the user is sent back to Login with: Epic sadface: You can only access '/inventory.html' when you are logged in..

**TC_SEC_02 · Session · Medium** Precondition: PRECOND-B Steps: Add Sauce Labs Backpack; logout via hamburger menu; log back in as standard_user / secret_sauce. Expected: Cart state persists - cart badge still shows 1 after re-login.

**TC_SEC_03 · Session · Medium** Precondition: PRECOND-A Steps: Login as standard_user; add Sauce Labs Backpack; logout; login as error_user / secret_sauce. Expected: Cart badge is clear for the new user (cart state is not carried across different users).
