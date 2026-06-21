QA Manual Test Cases:-  
For URL [https://advantageonlineshopping.com](https://advantageonlineshopping.com/#/) 

**Member:- Md Imran**

# **Query/Test cases:- OpenCart (Login \+ Registration \+ Store \+ Cart Flow)**

---

# **Human Thinking Test Cases**

## **TestCases\_001:-**

**Verify that a new user can successfully register an account, log in using the registered credentials, and access the application without errors.** 

1. Go to the OpenCart website.  
2. Click on “My Account” → Register  
3. Ena ter valid First Name  
4. Ena ter valid Last Name  
5. Ena ter valid Email ID  
6. Enter a valid Password  
7. Click on Continue  
8. Verify account creation success message  
9. Logout  
10. Gothe login page  
11. Enter the same Email ID  
12. Enter Password  
13. Click Login  
14. Verify user is logged in successfully

---

## TestCases\_002:-

**Verify that the system displays appropriate validation messages for invalid email formats, duplicate email registrations, and incorrect login credentials.** 

1. Go to OpenCart website  
2. Click on Register  
3. Ean nter invalid Email ID format (abc.com)  
4. Find the other mandatory fields  
5. Click Continue  
6. The eck validation message  
7. Enter the already registered Email ID  
8. Click Continue  
9. Verify duplicate email error  
10. Go to the login page  
11. Enter the wrong password  
12. Click Login  
13. Verify that the error message is shown

---

## TestCases\_003:- 

**Verify that products can be added to the cart successfully and that product name, price, quantity, and total price calculations are displayed accurately.** 

1. Go to the OpenCart Store page  
2. Select a product  
3. Click Add to Cart  
4. Go to Cart page  
5. Verify product name  
6. Verify product price  
7. Verify quantity \= 1  
8. Verify total price calculation  
9. Increase quantity to 2  
10. Click Update  
11. Verify total price updates correctly

---

## **TestCases\_004:-**

| Verify that users can remove products from the cart, that checkout is prevented when the cart is empty, and that out-of-stock products cannot be added to the cart. |
| :---- |

1. Go to the OpenCart Store page  
2. Add product to cart  
3. Open Cart  
4. Remove product from cart  
5. Verify the cart becomes empty  
6. Try checking out with an empty cart  
7. Verify error/validation message  
8. Go to the store again  
9. Add out-of-stock product (if available)  
10. Verify the system blocks addition

---

# **AI Manual Test Cases:-**

Prompt:- Write test cases for OpenCart end-to-end flow (Register → Login → Add to Cart → Verify Price)

---

### **TestCases\_001:-**

**Verify that a registered user can successfully search for a product, view the product details page, and verify product information.**

1. Go to the OpenCart website.  
2. Enter a valid product name in the Search box.  
3. Click the Search button.  
4. Verify search results are displayed.  
5. Select a product from the search results.  
6. Verify navigation to the Product Details page.  
7. Verify the product name is displayed correctly.  
8. Verify the product price is displayed.  
9. Verify the product description is displayed.  
10. Verify the product image is displayed.  
11. Verify the Add to Cart button is available.

    ---

    ### **TestCases\_006:-**

**Verify that a registered user can successfully update account information and view the updated details.**

1. Go to the OpenCart website.  
2. Click on “My Account” → Login.  
3. Enter valid Email ID.  
4. Enter valid Password.  
5. Click Login.  
6. Verify successful login.  
7. Click on “My Account” → Edit Account.  
8. Update First Name or Last Name.  
9. Click Continue.  
10. Verify account update success message.  
11. Open Account Information page.  
12. Verify updated details are displayed correctly.
     
    ---

    ### **TestCases\_002:-**

**Verify that a logged-in user can add multiple different products to the cart and that the cart displays all selected items correctly.**

1. Go to the OpenCart Store page.  
2. Select the first product.  
3. Click Add to Cart.  
4. Return to the Store page.  
5. Select a second product.  
6. Click Add to Cart.  
7. Open the Cart page.  
8. Verify both products are displayed.  
9. Verify the correct quantity for each product.  
10. Verify individual product prices.  
11. Verify the cart subtotal is calculated correctly.  
12. Verify the total amount is displayed correctly.
    
    ---

    ### **TestCases\_003:-**

**Verify that a user can successfully add a product to the Wish List and view it in the Wish List page.**

1. Go to the OpenCart website.  
2. Login with valid credentials.  
3. Search for a product.  
4. Open the Product Details page.  
5. Click Add to Wish List.  
6. Verify success message is displayed.  
7. Navigate to the Wish List page.  
8. Verify the selected product appears in the Wish List.  
9. Verify the product name is displayed correctly.  
10. Verify the product price is displayed correctly.
    
    ---

    ### **TestCases\_004:-**

**Verify that a logged-in user can successfully complete the checkout process and place an order.**

1. Go to the OpenCart website.  
2. Login with valid credentials.  
3. Select a product.  
4. Click Add to Cart.  
5. Open the Cart page.  
6. Verify the product is added successfully.  
7. Click Proceed to Checkout.  
8. Enter or verify Billing Details.  
9. Select Shipping Method.  
10. Select Payment Method.  
11. Accept Terms and Conditions.  
12. Click Confirm Order.  
13. Verify order confirmation message is displayed.  
14. Verify an Order ID is generated.  
15. Verify the order appears in Order History.

---

# **Your Thoughts:-**

● What you felt Suitable:-

* Covers complete end-to-end user journey (Register → Login → Search → Cart → Checkout)  
* Strong core functional coverage for OpenCart (most critical business flows included)  
* Good balance of positive \+ negative scenarios (TC001, TC002)  
* Proper cart validation and calculation testing (TC003, TC007)  
* Checkout flow is fully covered including order confirmation and Order ID validation (TC006)  
* Includes product discovery \+ product details validation (TC005)  
* Covers important error handling scenarios (invalid email, duplicate email, empty cart checkout)


---

● What you felt Not suitable:-

* Slight overlap between TC003 and TC007 (both heavily focus on cart behavior and calculations)  
* TC004 is useful but partially overlaps with TC003 (cart add/remove \+ edge cases)  
* No coverage for session persistence / refresh behavior during checkout flow  
* Missing non-functional testing (performance, usability, accessibility)  
* No explicit coverage for payment failure scenarios or gateway errors  
* Out-of-stock handling is included but dependent on availability (may not always be testable)

---

# **Final Test Case:- (AI \+ Manual Combined, Automation Ready)**

## **TestCases\_001:-**

Verify that a new user can successfully register an account, log in using the registered credentials, and access the application without errors.

1. Go to the OpenCart website  
2. Click on “My Account” → Register  
3. Enter valid First Name  
4. Enter valid Last Name  
5. Enter valid Email ID  
6. Enter a valid Password  
7. Click on Continue  
8. Verify account creation success message  
9. Logout from the application  
10. Go to login page and enter same Email ID and Password  
11. Click Login  
12. Verify user is logged in successfully

    ---

    ## **TestCases\_002:-**

Verify that the system displays appropriate validation messages for invalid email formats, duplicate email registrations, and incorrect login credentials.

1. Go to OpenCart website  
2. Click on Register  
3. Enter invalid Email ID format (abc.com)  
4. Fill other mandatory fields  
5. Click Continue  
6. Verify email validation message is displayed  
7. Enter already registered Email ID  
8. Click Continue  
9. Verify duplicate email error is shown  
10. Go to login page  
11. Enter wrong password  
12. Click Login  
13. Verify error message is displayed

    ---

    ## **TestCases\_003:-**

Verify that products can be added to the cart successfully and that product name, price, quantity, and total price calculations are displayed accurately.

1. Go to OpenCart Store page  
2. Select a product  
3. Click Add to Cart  
4. Open Cart page  
5. Verify product name is displayed correctly  
6. Verify product price is correct  
7. Verify quantity is 1  
8. Verify total price calculation is correct  
9. Increase quantity to 2  
10. Click Update  
11. Verify total price updates correctly

    ---

    ## **TestCases\_004:-**

Verify that users can remove products from the cart, that checkout is prevented when the cart is empty, and that out-of-stock products cannot be added.

1. Go to OpenCart Store page  
2. Add product to cart  
3. Open Cart page  
4. Remove product from cart  
5. Verify cart becomes empty  
6. Try proceeding to checkout with empty cart  
7. Verify error/validation message is displayed  
8. Navigate back to store page  
9. Attempt to add out-of-stock product (if available)  
10. Verify system blocks addition of out-of-stock item

    ---

    ## **TestCases\_005:-**

Verify that a registered user can search for a product, view product details, and validate product information correctly.

1. Go to OpenCart website  
2. Enter product name in search box  
3. Click Search  
4. Verify search results are displayed  
5. Select a product  
6. Verify Product Details page opens  
7. Verify product name is displayed correctly  
8. Verify product price is displayed  
9. Verify product description is visible  
10. Verify Add to Cart button is available

    ---

    ## **TestCases\_006:-**

Verify that a logged-in user can successfully complete checkout and place an order.

1. Go to OpenCart website  
2. Login with valid credentials  
3. Select a product  
4. Click Add to Cart  
5. Open Cart page  
6. Verify product is added correctly  
7. Click Proceed to Checkout  
8. Enter billing details  
9. Select shipping method  
10. Select payment method  
11. Accept terms and conditions  
12. Click Confirm Order  
13. Verify order confirmation message is displayed  
14. Verify Order ID is generated  
15. Verify order appears in Order History

    ---

    ## **TestCases\_007:-**

Verify that a logged-in user can add multiple products to the cart and verify cart calculations.

1. Go to OpenCart Store page  
2. Select first product  
3. Click Add to Cart  
4. Return to store page  
5. Select second product  
6. Click Add to Cart  
7. Open Cart page  
8. Verify both products are listed  
9. Verify correct quantity for each product  
10. Verify subtotal and total calculation is correct

## **TestCase001: Automation Ready E2E Flow (OpenCart – Register → Login → Search → Add to Cart → Checkout)**

Verify that a user can successfully complete the full end-to-end flow from account creation to order placement without errors.

1. Go to the OpenCart website  
2. Click on “My Account” → Register  
3. Enter valid First Name  
4. Enter valid Last Name  
5. Enter valid Email ID  
6. Enter valid Password  
7. Click Continue  
8. Verify account creation success message is displayed  
9. Logout from the application  
10. Go to “My Account” → Login  
11. Enter the same registered Email ID  
12. Enter Password  
13. Click Login  
14. Verify user is logged in successfully  
15. Enter a product name in the Search box  
16. Click Search  
17. Select a product from results  
18. Verify Product Details page is displayed  
19. Click Add to Cart  
20. Open Cart page  
21. Verify product name is correct  
22. Verify product price is correct  
23. Verify quantity is correct  
24. Click Proceed to Checkout  
25. Enter billing details  
26. Select shipping method  
27. Select payment method  
28. Accept terms and conditions  
29. Click Confirm Order  
30. Verify order confirmation message is displayed  
31. Verify Order ID is generated  
32. Verify order appears in Order History

# **Query/Test cases:- Sign In Page (Functional Test Cases)**

---

## Human Thinking Test Cases

---

### TestCases\_001:-

| Verify that users can successfully log in with valid credentials and are redirected to the dashboard or home page. |
| :---- |

1. Open Sign In page  
2. Enter a valid Username  
3. Enter a valid Password  
4. Click the Sign In button  
5. Verify user is logged in successfully  
6. Verify user is redirected to dashboard/home page  
7. Logout  
8. Again, open the Sign In page  
9. Enter the same credentials  
10. Click Sign In  
11. Verify login works consistently

---

### TestCases\_002:-

**Verify that the system displays validation messages when the username field is empty or contains invalid values.** 

1. Open Sign In page  
2. Leave Username blank  
3. Enter a valid Password  
4. Click Sign In  
5. Check the validation message  
6. Enter an invalid Username  
7. Enter a valid Password  
8. Click Sign In  
9. Verify the error message displayed  
10. Try logging in again with the correct credentials  
11. Verify the system allows login

---

### TestCases\_003:-

**Verify that the system displays appropriate validation messages for empty or incorrect passwords and allows login with valid credentials.** 

1. Open Sign In page  
2. Enter a valid Username  
3. Leave Password blank  
4. Click Sign In  
5. Verify the password required message  
6. Enter the wrong Password  
7. Click Sign In  
8. Verify the authentication failure message  
9. Enter the correct Password  
10. Click Sign In  
11. Verify successful login

---

### TestCases\_004:-

**Verify that mandatory field validations are displayed when both the username and password fields are left blank.** 

1. Open Sign In page  
2. Leave both Username and Password blank  
3. Click Sign In  
4. Verify both field validation messages  
5. Enter a valid Username  
6. Enter the wrong Password  
7. Click Sign In  
8. Verify login fails  
9. Retry with correct credentials  
10. Verify login success

---

### TestCases\_005:-

**Verify that the "Remember Me" functionality correctly retains or removes user sessions based on the selected option.** 

1. Open Sign In page  
2. Enter a valid Username and Password  
3. Check the “Remember Me” option  
4. Click Sign In  
5. Logout  
6. Reopen application  
7. Check whether the session is retained or not  
8. Log in again without Remember Me  
9. Logout again  
10. Verify the session is not retained

---

### TestCases\_006:-

**Verify that the Forgot Password feature allows registered users to initiate password recovery and displays appropriate messages for invalid requests.** 

1. Open Sign In page  
2. Click “Forgot Password”  
3. Verify navigation to the recovery page  
4. Enter registered email  
5. Submit request  
6. Verify that the reset email has been sent  
7. Try with an unregistered email  
8. Verify the error message displayed  
9. Navigate back to the login page  
10. Verify the login page loads correctly

---

### TestCases\_007:-

**Verify that social login functionality redirects users to the external authentication provider and handles success or cancellation correctly.** 

1. Open Sign In page  
2. Click “Sign in with Facebook”  
3. Verify the Facebook authentication page opens  
4. Enter valid Facebook credentials  
5. Approve permissions  
6. Verify user is logged in  
7. Logout from application  
8. Try Facebook login again  
9. Cancel login process  
10. Verify user remains on login page

---

### TestCases\_008:-

**Verify that the authentication system correctly handles both successful and failed login attempts.** 

1. Open Sign In page  
2. Enter valid Username  
3. Enter valid Password  
4. Click Sign In  
5. Verify login success  
6. Enter invalid Username  
7. Click Sign In  
8. Verify error message  
9. Enter invalid Password  
10. Click Sign In  
11. Verify authentication failure

---

### TestCases\_009:-

**Verify that username input validation correctly handles leading/trailing spaces, special characters, and invalid formats.**

1. Open Sign In page  
2. Enter Username with leading/trailing spaces  
3. Enter valid Password  
4. Click Sign In  
5. Verify system trims input or rejects it  
6. Enter special characters in Username  
7. Click Sign In  
8. Verify validation message  
9. Retry with valid input  
10. Verify successful login

---

### TestCases\_010:-

**Verify that all login page UI elements, navigation links, and account creation links function correctly.** 

1. Open Sign In page  
2. Verify all UI elements are loaded  
3. Click “Create New Account” link  
4. Verify navigation to registration page  
5. Come back to login page  
6. Verify page loads correctly  
7. Enter valid credentials  
8. Click Sign In  
9. Verify login success  
10. Logout and confirm session ends

---

# **AI Manual Test Cases:-**

Prompt:- Write automation-ready functional test cases for the Sign In page

---

## **TestCases\_001**

**Title:** Successful login with valid credentials and session consistency

**Steps:**

1. Open URL (Sign In page)  
2. Enter a valid Username  
3. Enter a valid Password  
4. Click the Sign In button  
5. Verify user is logged in successfully  
6. Verify user is redirected to dashboard/home page  
7. Click Logout  
8. Again open URL (Sign In page)  
9. Enter the same valid credentials  
10. Click Sign In button  
11. Verify login works consistently

**Expected Result:**  
 User should successfully log in, be redirected to dashboard/home page, and login should work consistently after logout.

---

## **TestCases\_002**

**Title:** Username field validation (empty and invalid values)

**Steps:**

1. Open URL (Sign In page)  
2. Leave Username blank  
3. Enter a valid Password  
4. Click Sign In button  
5. Verify validation message for username  
6. Enter an invalid Username  
7. Enter a valid Password  
8. Click Sign In button  
9. Verify error message is displayed  
10. Enter valid credentials  
11. Click Sign In button  
12. Verify user is logged in successfully

**Expected Result:**  
 System should show validation errors for empty/invalid username and allow login only with valid credentials.

---

## **TestCases\_003**

**Title:** Password field validation (empty, incorrect, valid)

**Steps:**

1. Open URL (Sign In page)  
2. Enter a valid Username  
3. Leave Password blank  
4. Click Sign In button  
5. Verify password required message  
6. Enter wrong Password  
7. Click Sign In button  
8. Verify authentication failure message  
9. Enter correct Password  
10. Click Sign In button  
11. Verify successful login

**Expected Result:**  
 System should validate empty/incorrect password and allow login only with correct password.

---

## **TestCases\_004**

**Title:** Mandatory field validation for both username and password

**Steps:**

1. Open URL (Sign In page)  
2. Leave Username blank  
3. Leave Password blank  
4. Click Sign In button  
5. Verify validation messages for both fields  
6. Enter a valid Username  
7. Enter wrong Password  
8. Click Sign In button  
9. Verify login fails  
10. Enter correct credentials  
11. Click Sign In button  
12. Verify login success

**Expected Result:**  
 System should show required field validation when both fields are empty and allow login only with valid credentials.

---

## **TestCases\_005**

**Title:** Remember Me functionality validation

**Steps:**

1. Open URL (Sign In page)  
2. Enter valid Username and Password  
3. Check “Remember Me” checkbox  
4. Click Sign In button  
5. Click Logout  
6. Reopen application URL  
7. Verify whether session is retained  
8. Login again without selecting “Remember Me”  
9. Click Logout  
10. Reopen application  
11. Verify session is not retained

**Expected Result:**  
 Session should persist only when “Remember Me” is selected.

---

## **TestCases\_006**

**Title:** Forgot Password functionality validation

**Steps:**

1. Open URL (Sign In page)  
2. Click “Forgot Password”  
3. Verify navigation to recovery page  
4. Enter registered email  
5. Click Submit  
6. Verify reset email sent message  
7. Enter unregistered email  
8. Click Submit  
9. Verify error message  
10. Navigate back to Sign In page  
11. Verify login page loads correctly

**Expected Result:**  
 Password reset should work for registered users and show error for invalid emails.

---

## **TestCases\_007**

**Title:** Social login (Facebook) authentication flow

**Steps:**

1. Open URL (Sign In page)  
2. Click “Sign in with Facebook”  
3. Verify Facebook login page opens  
4. Enter valid Facebook credentials  
5. Approve permissions  
6. Verify user is logged in  
7. Click Logout  
8. Again click “Sign in with Facebook”  
9. Cancel authentication  
10. Verify user remains on login page

**Expected Result:**  
 User should be able to log in via Facebook and handle cancel flow correctly.

---

## **TestCases\_008**

**Title:** Login authentication success and failure handling

**Steps:**

1. Open URL (Sign In page)  
2. Enter valid Username  
3. Enter valid Password  
4. Click Sign In button  
5. Verify login success  
6. Enter invalid Username  
7. Click Sign In button  
8. Verify error message  
9. Enter invalid Password  
10. Click Sign In button  
11. Verify authentication failure

**Expected Result:**  
 System should correctly handle both successful and failed login attempts.

---

## **TestCases\_009**

**Title:** Username input validation (spaces and special characters)

**Steps:**

1. Open URL (Sign In page)  
2. Enter Username with leading/trailing spaces  
3. Enter valid Password  
4. Click Sign In button  
5. Verify input is trimmed or rejected  
6. Enter special characters in Username  
7. Click Sign In button  
8. Verify validation message  
9. Enter valid Username  
10. Enter valid Password  
11. Click Sign In button  
12. Verify successful login

**Expected Result:**  
 System should handle spaces and special characters properly and allow only valid usernames.

---

## **TestCases\_010**

**Title:** Login page UI elements and navigation validation

**Steps:**

1. Open URL (Sign In page)  
2. Verify all UI elements are visible  
3. Click “Create New Account” link  
4. Verify navigation to registration page  
5. Navigate back to login page  
6. Verify login page loads correctly  
7. Enter valid credentials  
8. Click Sign In button  
9. Verify login success  
10. Click Logout  
11. Verify session ends properly

**Expected Result:**  
 All UI elements and navigation links should work correctly, and login/logout flow should function properly.

---

# **Your Thoughts:-**

● What you felt Suitable:-

* Good coverage of login functionality (positive \+ negative cases)  
* Includes important features like Remember Me, Forgot Password, Social Login  
* Covers real user flows (login → logout → re-login)  
* Good mix of validation and authentication scenarios  
* Basic UI \+ navigation checks are included

---

● What you felt Not suitable:-

* Repeated login/logout and authentication checks (redundant cases)  
* Multiple scenarios combined in single test case (not atomic)  
* Overlapping validation cases (username/password repeated in different tests)  
* UI and functional flows mixed together in some test cases  
* Some steps are too detailed and unnecessary for automation readiness

---

# **Final Test Case:-** 

---

## 

### **TC\_001 — Valid Login (Happy Path \+ Session Check)**

**Steps:**

1. Open Sign In page  
2. Enter valid Username  
3. Enter valid Password  
4. Click Sign In  
5. Verify user is redirected to dashboard/home page  
6. Click Logout  
7. Reopen Sign In page  
8. Login again with same credentials

**Expected Result:**  
 User should successfully log in, be redirected to dashboard, and login should work consistently after logout.

---

### **TC\_002 — Username Field Validation**

**Steps:**

1. Open Sign In page  
2. Leave Username blank  
3. Enter valid Password  
4. Click Sign In  
5. Verify validation message  
6. Enter invalid Username (special characters / wrong format)  
7. Click Sign In  
8. Verify error message

**Expected Result:**  
 System should not allow login with empty or invalid username.

---

### **TC\_003 — Password Field Validation**

**Steps:**

1. Open Sign In page  
2. Enter valid Username  
3. Leave Password blank  
4. Click Sign In  
5. Verify required password message  
6. Enter incorrect Password  
7. Click Sign In  
8. Verify authentication failure message

**Expected Result:**  
 System should block login for empty or incorrect password.

---

### **TC\_004 — Mandatory Field Validation (Both Empty)**

**Steps:**

1. Open Sign In page  
2. Leave Username blank  
3. Leave Password blank  
4. Click Sign In  
5. Verify validation messages for both fields

**Expected Result:**  
 System should show required field validations for both username and password.

---

### **TC\_005 — Remember Me Functionality**

**Steps:**

1. Open Sign In page  
2. Enter valid Username and Password  
3. Select “Remember Me”  
4. Click Sign In  
5. Click Logout  
6. Reopen application  
7. Verify session is retained  
8. Login again without selecting “Remember Me”  
9. Logout  
10. Reopen application  
11. Verify session is not retained

**Expected Result:**  
 Session should persist only when “Remember Me” is selected.

---

### **TC\_006 — Forgot Password Flow**

**Steps:**

1. Open Sign In page  
2. Click “Forgot Password”  
3. Enter registered email  
4. Click Submit  
5. Verify reset email confirmation message  
6. Enter unregistered email  
7. Click Submit  
8. Verify error message  
9. Navigate back to login page

**Expected Result:**  
 Registered users should receive reset flow, invalid users should see error message.

---

### **TC\_007 — Social Login (Facebook)**

**Steps:**

1. Open Sign In page  
2. Click “Sign in with Facebook”  
3. Login using valid Facebook credentials  
4. Approve permissions  
5. Verify successful login  
6. Logout  
7. Click Facebook login again  
8. Cancel authentication

**Expected Result:**  
 User should be able to login via Facebook and cancellation should return to login page safely.

---

### **TC\_008 — Authentication Handling (Positive \+ Negative)**

**Steps:**

1. Open Sign In page  
2. Enter valid Username and Password → Click Sign In  
3. Verify successful login  
4. Enter invalid Username → Click Sign In  
5. Verify error message  
6. Enter invalid Password → Click Sign In  
7. Verify authentication failure

**Expected Result:**  
 System should correctly handle both successful and failed login attempts.

---

### **TC\_009 — Username Format Validation**

**Steps:**

1. Open Sign In page  
2. Enter Username with leading/trailing spaces  
3. Enter valid Password  
4. Click Sign In  
5. Verify input is trimmed or rejected  
6. Enter special characters in Username  
7. Click Sign In  
8. Verify validation message

**Expected Result:**  
 System should handle invalid username formats correctly.

---

### **TC\_010 — UI Elements & Navigation Check**

**Steps:**

1. Open Sign In page  
2. Verify all UI elements are visible (fields, buttons, links)  
3. Click “Create New Account”  
4. Verify navigation to registration page  
5. Navigate back to Sign In page  
6. Enter valid credentials  
7. Click Sign In  
8. Verify successful login  
9. Click Logout

**Expected Result:**  
 All UI elements and navigation links should work correctly.

# **End-to-End Sign In Flow (Automation Ready)**

Validate complete Sign In functionality from login to logout and re-login stability.

---

## 

1. Open Sign In page URL  
2. Verify Username field is visible  
3. Verify Password field is visible  
4. Verify Sign In button is visible  
5. Click Sign In button without entering any data  
6. Verify validation messages for Username and Password fields  
7. Enter invalid Username  
8. Enter invalid Password  
9. Click Sign In button  
10. Verify authentication error message is displayed  
11. Enter valid Username  
12. Enter valid Password  
13. Click Sign In button  
14. Verify user is redirected to Dashboard/Home page  
15. Verify user session is active (profile/logout visible)  
16. Click Logout button  
17. Verify user is redirected to Sign In page  
18. Enter valid Username and Password again  
19. Click Sign In button  
20. Verify login is successful again  
21. (Optional) Enable “Remember Me”, login, logout, and reopen application  
22. Verify session behavior based on Remember Me setting

---

Expected Result:

* Login page should load correctly with all UI elements visible  
* System should show validation messages for empty inputs  
* Invalid credentials should be rejected with error message  
* Valid credentials should allow login and redirect to dashboard  
* Logout should end session properly  
* Re-login should work consistently without issues  
* “Remember Me” should persist session when enabled

# **Query/Test cases:- Product Page (BOSE SOUNDLINK BLUETOOTH SPEAKER III)**

---

# **Human Thinking Test Cases**

---

## **TestCases\_001:-**

**Verify that all product information, including name, price, description, and page content, loads correctly and remains consistent after refresh.** 

1. Open product page  
2. Verify product name is displayed  
3. Verify product price is shown  
4. Verify product description is visible  
5. Check all product information loads correctly  
6. Scroll product page  
7. Confirm no missing UI elements  
8. Refresh page  
9. Verify data consistency after reload  
10. Validate no layout distortion

---

## **TestCases\_002:-**

**Verify that the colour selection functionality allows only one active selection and updates correctly when switching between available colours.** 

1. Open product page  
2. Select Black color  
3. Verify Black is selected  
4. Switch to Grey color  
5. Verify only Grey is selected  
6. Confirm previous selection is unselected  
7. Reload page  
8. Check default color behavior  
9. Try switching colors multiple times  
10. Verify selection always updates correctly

---

## **TestCases\_003:-**

**Verify that quantity controls correctly increase, decrease, and restrict invalid quantity values and non-numeric input.**

1. Open product page  
2. Click “+” button to increase quantity  
3. Verify quantity increases  
4. Click “–” button to decrease quantity  
5. Verify quantity decreases  
6. Try decreasing below 1  
7. Verify system prevents invalid quantity  
8. Enter quantity manually  
9. Enter invalid input (abc/@\#)  
10. Verify system rejects invalid input  
11. Set quantity to 0  
12. Verify system resets to minimum value

---

## **TestCases\_004:-**

**Verify that a product can be added to the cart successfully and that cart details accurately reflect the selected configuration.** 

1. Open product page  
2. Select color  
3. Set quantity  
4. Click Add to Cart  
5. Verify product is added  
6. Open cart  
7. Verify product name  
8. Verify product price  
9. Verify quantity  
10. Verify total calculation

---

## **TestCases\_005:-**

**Verify that required product options and quantity validations are enforced before allowing Add to Cart actions.** 

1. Open product page  
2. Click Add to Cart without selecting color  
3. Verify validation message  
4. Select color only  
5. Click Add to Cart  
6. Verify behavior  
7. Set invalid quantity  
8. Click Add to Cart  
9. Verify system handles default or error  
10. Confirm product not added incorrectly

---

## **TestCases\_006:-**

**Verify that product specification details such as manufacturer, compatibility, weight, and wireless technology are displayed correctly.** 

1. Open product page  
2. Verify product specifications section  
3. Check compatibility information  
4. Check connector type  
5. Check manufacturer name  
6. Check weight  
7. Check wireless technology  
8. Scroll section  
9. Refresh page  
10. Verify data remains correct

---

## **TestCases\_007:-**

**Verify that product option selection impacts Add to Cart behavior correctly and validation messages are displayed when required selections are missing.** 

1. Open product page  
2. Select color option  
3. Switch between colors multiple times  
4. Verify only one color selected  
5. Click Add to Cart button state  
6. Verify button behavior changes correctly  
7. Try adding product without selection  
8. Check validation message  
9. Re-select valid options  
10. Verify Add to Cart works

---

## **TestCases\_008:-**

**Verify that the product page loads successfully, displays all UI components correctly, and remains functional during navigation and refresh actions.** 

1. Open product page URL  
2. Verify page loads successfully  
3. Check product image visibility  
4. Check UI alignment  
5. Scroll page completely  
6. Refresh page  
7. Verify content reloads properly  
8. Verify no broken elements  
9. Check responsiveness  
10. Confirm no functional errors

---

## **TestCases\_009:-**

**Verify that product selections and cart updates behave consistently during page refreshes and repeated cart operations.** 

1. Open product page  
2. Select color and quantity  
3. Add product to cart  
4. Refresh page  
5. Check if selection persists or resets  
6. Navigate away and return  
7. Verify product state  
8. Add again to cart  
9. Verify cart update  
10. Validate no duplicate errors

---

## **TestCases\_010:-**

**Verify that valid and invalid Add to Cart scenarios are handled correctly and cart information remains accurate throughout the workflow.** 

1. Open product page  
2. Perform valid Add to Cart flow  
3. Perform invalid Add to Cart flow  
4. Verify validation messages  
5. Check cart update  
6. Check quantity update  
7. Check price consistency  
8. Re-check product selection  
9. Remove product from cart  
10. Verify cart updates correctly

---

# **AI Manual Test Cases:-**

Prompt:- Write automation-ready functional test cases for Product Page (BOSE Speaker)

---

## **TestCases\_001:-**

## **TestCase001:-**

Verify that the product page loads correctly with all essential sections (images, price, title, CTA buttons) rendered properly.

1. open product listing page  
2.  click on a product  
3.  verify product detail page opens  
4.  check product title is visible  
5.  check product price is displayed  
6.  verify add to cart button is visible  
7.  verify product images section is loaded  
8.  scroll down the page  
9.  verify description section is visible  
10.  refresh page and confirm all elements load correctly


## **TestCase002:-**

 Verify that product quantity selector increases and decreases quantity correctly within allowed limits.

1. open product page  
2. locate quantity selector  
3. click increase quantity button  
4. verify quantity increases by 1  
5. click increase again  
6. verify quantity updates correctly  
7. click decrease quantity button  
8. verify quantity decreases by 1  
9. try setting quantity below minimum  
10. verify system prevents invalid quantity

---

## TestCase003:-

 Verify that product description section expands and collapses correctly without UI glitches.

1. open product page  
2. scroll to product description  
3. click "read more" button  
4. verify full description expands  
5. scroll through expanded content  
6. click "read less" button  
7. verify description collapses  
8. repeat expand action  
9. verify no layout break occurs  
10. refresh page and confirm default state

---

## **TestCase004:-**

 Verify that related products section displays relevant items and navigation works correctly.

1. open product page  
2. scroll to related products section  
3. verify related products are displayed  
4. click on a related product  
5. verify navigation to new product page  
6. return back to original product page  
7. verify related section loads again  
8. scroll horizontally through related items  
9. verify all items are accessible  
10. refresh page and confirm section reloads

---

## **TestCase005:-**

 Verify that product review section displays ratings and allows users to view all reviews.

1. open product page  
2. scroll to reviews section  
3. verify average rating is visible  
4. check number of reviews displayed  
5. click on "view all reviews"  
6. verify full review list opens  
7. scroll through reviews  
8. verify star ratings are shown correctly  
9. close review modal or section  
10. refresh page and confirm review summary remains

---

## TestCase006:-

 Verify that product filter options (if available) update product results correctly on selection.

1. open product listing page  
2. locate filter panel  
3. select first filter option  
4. verify results update accordingly  
5. select additional filter option  
6. verify filtered results refine further  
7. remove one filter  
8. verify results update again  
9. reset all filters  
10. verify default product list is restored

---

## **TestCase007:-**

 Verify that product page handles browser refresh without losing critical session behavior.

1. open product page  
2. select product variant  
3. add product to cart  
4. verify cart update is successful  
5. refresh the page  
6. verify selected variant is retained  
7. verify cart icon still shows updated item count  
8. scroll down the page  
9. verify previously selected options are still visible  
10. navigate away and return to confirm session consistency

---

# **Your Thoughts:-**

● What you felt Suitable:-

* Covers complete end-to-end product flow (browse → select → add to cart → verify cart)  
* Good mix of positive and negative test scenarios  
* Strong focus on cart functionality and validations  
* Includes state persistence and refresh handling  
* Quantity and validation logic is well covered  
* Reduces major functional risk areas

---

● What you felt Not suitable:-

* Some duplication in UI and variant selection tests (TC002 vs TC007, TC001 vs TC008)  
* Includes a few low-priority informational checks (TC006, TC008) in regression scope  
* Missing some non-functional coverage (performance, accessibility, API failure handling)  
* Slight overlap in page load and UI validation scenarios  
* Could be optimized further to reduce redundancy in execution time


---

# **Final Test Case:- (AI \+ Manual Combined, Automation Ready)**

---

##   **TestCases\_001:-**

Verify that all product information, including name, price, description, and page content, loads correctly and remains consistent after refresh.

1. Open product page  
2. Verify product name is displayed  
3. Verify product price is shown  
4. Verify product description is visible  
5. Check all product information loads correctly  
6. Scroll product page  
7. Confirm no missing UI elements  
8. Refresh page  
9. Verify data consistency after reload  
10. Validate no layout distortion

## ---

## **TestCases\_003:-**

Verify that quantity controls correctly increase, decrease, and restrict invalid quantity values and non-numeric input.

1. Open product page  
2. Click “+” button to increase quantity  
3. Verify quantity increases  
4. Click “–” button to decrease quantity  
5. Verify quantity decreases  
6. Try decreasing below 1  
7. Verify system prevents invalid quantity  
8. Enter invalid input (abc/@\#)  
9. Verify system rejects invalid input

10. ## **Set quantity to 0 and verify reset to minimum value**

## ---

## **TestCases\_004:-**

Verify that a product can be added to the cart successfully and that cart details accurately reflect the selected configuration.

1. Open product page  
2. Select product color  
3. Set quantity  
4. Click Add to Cart  
5. Verify product is added successfully  
6. Open cart page  
7. Verify product name is correct  
8. Verify product price is correct  
9. Verify quantity is correct  
10. Verify total calculation is accurate

## ---

## **TestCases\_005:-**

Verify that required product options and quantity validations are enforced before allowing Add to Cart actions.

1. Open product page  
2. Click Add to Cart without selecting color  
3. Verify validation message is displayed  
4. Select color only  
5. Click Add to Cart  
6. Verify system behavior is handled correctly  
7. Set invalid quantity  
8. Click Add to Cart  
9. Verify system prevents incorrect addition  
10. Confirm product is not added incorrectly

## ---

## **TestCases\_007:-**

Verify that product option selection impacts Add to Cart behavior correctly and validation messages are displayed when required selections are missing.

1. Open product page  
2. Select color option  
3. Switch between colors multiple times  
4. Verify only one color is selected  
5. Observe Add to Cart button state  
6. Verify button behavior updates correctly  
7. Try adding product without valid selection  
8. Verify validation message is shown  
9. Re-select valid options  
10. Verify Add to Cart works successfully

## ---

## **TestCases\_009:-**

Verify that product selections and cart updates behave consistently during page refreshes and repeated cart operations.

1. Open product page  
2. Select color and quantity  
3. Add product to cart  
4. Refresh page  
5. Check if selection persists or resets  
6. Navigate away and return  
7. Verify product state consistency  
8. Add product again to cart  
9. Verify cart updates correctly  
10. Confirm no duplicate or inconsistent entries

## ---

## **TestCases\_010:-**

Verify that valid and invalid Add to Cart scenarios are handled correctly and cart information remains accurate throughout the workflow.

1. Open product page  
2. Perform valid Add to Cart flow  
3. Verify product is added correctly  
4. Perform invalid Add to Cart flow  
5. Verify validation messages are shown  
6. Check cart update accuracy  
7. Verify quantity correctness  
8. Verify price consistency  
9. Remove product from cart  
10. Verify cart updates correctly

## **TestCase\_001 (Automation Ready – Product Page End-to-End Flow)**

## 

Verify complete end-to-end Product Page flow including UI load, variant selection, quantity handling, Add to Cart, cart validation, and state consistency.

1. Open product listing page  
2. Click on a product  
3. Verify product detail page loads successfully  
4. Verify product title, price, images, and Add to Cart button are visible  
5. Select a product color option  
6. Verify only one color is selected at a time  
7. Change color selection and verify update is reflected correctly  
8. Increase quantity using “+” button and verify increment works  
9. Decrease quantity using “–” button and verify decrement works  
10. Try entering invalid quantity (text/0/negative) and verify validation prevents it  
11. Click Add to Cart button  
12. Verify product is added to cart successfully  
13. Open cart page  
14. Verify correct product name, selected color, quantity, and price are displayed  
15. Verify cart total is calculated correctly  
16. Refresh product page  
17. Verify selected state behavior (reset or retained as per system design)  
18. Navigate away and return back to product page  
19. Verify product page loads correctly without data mismatch  
20. Confirm no duplicate or incorrect cart entries exist

