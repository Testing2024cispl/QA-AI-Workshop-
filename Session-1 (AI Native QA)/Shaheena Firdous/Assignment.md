Sauce Demo – Successful User Login Test Cases
Part 1: Human Thinking Test Cases
Test Case 1: Verify successful login with valid username and password
Steps:
Open the Sauce Demo application.
Enter a valid username.
Enter a valid password.
Click the Login button.
Expected Result:
The user should successfully log in and be redirected to the Products page.

Test Case 2: Verify user is redirected to the Inventory page after login
Steps:
Launch the application.
Enter valid login credentials.
Click Login.
Observe the URL.
Expected Result:
The URL should change to inventory.html.

Test Case 3: Verify the Products page is displayed after successful login
Steps:
Login using valid credentials.
Observe the landing page.
Expected Result:
The Products page should be displayed with the product list.

Test Case 4: Verify the shopping cart icon is visible after login
Steps:
Login successfully.
Check the top-right corner of the page.
Expected Result:
The shopping cart icon should be visible.

Test Case 5: Verify the navigation menu is displayed after login
Steps:
Login to the application.
Observe the top-left corner.
Click the hamburger menu.
Expected Result:
The navigation menu should open successfully.

Test Case 6: Verify all inventory items are displayed after successful login
Steps:
Login with valid credentials.
Scroll through the Products page.
Expected Result:
All available inventory items should be displayed.

Test Case 7: Verify the page title is displayed correctly after login
Steps:
Login successfully.
Observe the page title.
Expected Result:
The page title should display "Swag Labs."

Test Case 8: Verify the user session remains active while navigating
Steps:
Login successfully.
Navigate between different pages.
Return to the Products page.
Expected Result:
The user should remain logged in.

Test Case 9: Verify the user can successfully log out
Steps:
Login successfully.
Click the hamburger menu.
Click Logout.
Expected Result:
The user should be redirected to the Login page.

Test Case 10: Verify the user cannot access the Inventory page after logout
Steps:
Login successfully.
Logout from the application.
Press the browser Back button.
Expected Result:
The Inventory page should not be accessible without logging in again.

Part 2: AI-Generated Test Cases
Prompt - Generate 10 detailed manual test cases for the Successful User Login functionality of the Sauce Demo application.
Application: Sauce Demo (https://www.saucedemo.com/)
Scenario: Successful User Login using valid credentials.
Requirements:
Generate exactly 10 positive test cases.
Each test case should include:
Test Case Title
Test Steps
Expected Result
Use the valid credentials:
Username: standard_user
Password: secret_sauce
Cover different aspects of the login process, including:
Successful authentication
Redirection to the Inventory page
URL validation
UI element verification (shopping cart, navigation menu, products)
Session persistence after browser refresh
Product information display
Logout functionality
Access restriction after logout
Basic performance validation (login response time)
Write the test cases in a professional QA format suitable for manual testing.

Test Case 1: Verify successful login using valid credentials
Steps:
Navigate to the Sauce Demo login page.
Enter username standard_user.
Enter password secret_sauce.
Click Login.
Expected Result:
The application should authenticate the user and redirect them to the Inventory page.

Test Case 2: Verify the application redirects to inventory.html after successful login
Steps:
Login using valid credentials.
Observe the browser URL.
Expected Result:
The URL should end with inventory.html.

Test Case 3: Verify the Inventory page loads without UI errors
Steps:
Login successfully.
Observe the page layout.
Check for broken images or missing elements.
Expected Result:
The Inventory page should load completely without any UI issues.

Test Case 4: Verify all product details are displayed correctly
Steps:
Login successfully.
Review each product displayed.
Expected Result:
Each product should display its image, name, description, and price correctly.

Test Case 5: Verify the shopping cart icon and badge are displayed correctly
Steps:
Login successfully.
Observe the shopping cart section.
Expected Result:
The shopping cart icon should be visible and function correctly.

Test Case 6: Verify the hamburger menu displays all navigation options
Steps:
Login successfully.
Click the hamburger menu.
Expected Result:
The menu should display options such as All Items, About, Logout, and Reset App State.

Test Case 7: Verify the user session persists after refreshing the browser
Steps:
Login successfully.
Refresh the browser.
Expected Result:
The user should remain logged in and continue on the Inventory page.

Test Case 8: Verify login response time is within acceptable limits
Steps:
Enter valid credentials.
Click Login.
Measure the time taken to load the Inventory page.
Expected Result:
The Inventory page should load within the expected response time (e.g., under 3 seconds).

Test Case 9: Verify the logout functionality
Steps:
Login successfully.
Open the hamburger menu.
Click Logout.
Expected Result:
The user should be logged out and redirected to the Login page.

Test Case 10: Verify direct access to the Inventory page is restricted after logout
Steps:
Login successfully.
Logout from the application.
Enter the Inventory page URL directly in the browser.
Expected Result:
The application should redirect the user to the Login page instead of allowing access to the Inventory page.

Login successfully.
Observe the page title.
Expected Result:
The page title should display "Swag Labs."

Test Case 8: Verify the user session remains active while navigating
Steps:
Login successfully.
Navigate between different pages.
Return to the Products page.
Expected Result:
The user should remain logged in.

Test Case 9: Verify the user can successfully log out
Steps:
Login successfully.
Click the hamburger menu.
Click Logout.
Expected Result:
The user should be redirected to the Login page.

Test Case 10: Verify the user cannot access the Inventory page after logout
Steps:
Login successfully.
Logout from the application.
Press the browser Back button.
Expected Result:
The Inventory page should not be accessible without logging in again.

# Final Test Cases – Successful User Login (Sauce Demo)

### Test Case 1: Verify successful login with valid credentials

**Steps:**

1. Open the Sauce Demo application.
2. Enter username **standard_user**.
3. Enter password **secret_sauce**.
4. Click the **Login** button.

**Expected Result:**
The user should successfully log in and be redirected to the Inventory page.

---

### Test Case 2: Verify the application redirects to the Inventory page after successful login

**Steps:**

1. Login using valid credentials.
2. Observe the browser URL.

**Expected Result:**
The URL should end with **inventory.html**.

---

### Test Case 3: Verify the Inventory page loads correctly

**Steps:**

1. Login successfully.
2. Observe the page after login.

**Expected Result:**
The Inventory page should load completely without any UI errors.

---

### Test Case 4: Verify all inventory products are displayed

**Steps:**

1. Login successfully.
2. Scroll through the Products page.

**Expected Result:**
All available inventory items should be displayed.

---

### Test Case 5: Verify product details are displayed correctly

**Steps:**

1. Login successfully.
2. Review each product listed.

**Expected Result:**
Each product should display its image, product name, description, and price correctly.

---

### Test Case 6: Verify the shopping cart icon is displayed

**Steps:**

1. Login successfully.
2. Observe the top-right corner of the page.

**Expected Result:**
The shopping cart icon should be visible and clickable.

---

### Test Case 7: Verify the navigation menu options

**Steps:**

1. Login successfully.
2. Click the hamburger menu.

**Expected Result:**
The menu should display the options: **All Items, About, Logout,** and **Reset App State**.

---

### Test Case 8: Verify the page title after successful login

**Steps:**

1. Login successfully.
2. Observe the application title displayed at the top.

**Expected Result:**
The page title should display **Swag Labs**.

---

### Test Case 9: Verify user session persistence after browser refresh

**Steps:**

1. Login successfully.
2. Refresh the browser page.

**Expected Result:**
The user should remain logged in and stay on the Inventory page.

---

### Test Case 10: Verify successful logout

**Steps:**

1. Login successfully.
2. Click the hamburger menu.
3. Select **Logout**.

**Expected Result:**
The user should be logged out and redirected to the Login page.

---

### Test Case 11: Verify Inventory page cannot be accessed after logout

**Steps:**

1. Login successfully.
2. Logout from the application.
3. Enter the Inventory page URL (**inventory.html**) directly in the browser.

**Expected Result:**
The application should redirect the user to the Login page and prevent unauthorized access.

---

### Test Case 12: Verify login response time

**Steps:**

1. Enter valid login credentials.
2. Click the **Login** button.
3. Observe the time taken for the Inventory page to load.

**Expected Result:**
The Inventory page should load within the acceptable response time (e.g., less than 3 seconds under normal network conditions).

SESSIO 2
# Skill: Generate Manual Test Cases for Successful User Login (Sauce Demo)

## Objective
Create comprehensive manual test cases for the Successful User Login functionality of the Sauce Demo application.

## Application
- **Application Name:** Sauce Demo
- **URL:** https://www.saucedemo.com/
- **Module:** Login
- **Scenario:** Successful User Login

## Test Data
- Username: `standard_user`
- Password: `secret_sauce`

---

# Test Case 1: Verify successful login with valid credentials
## Steps
1. Open the Sauce Demo application.
2. Enter username `standard_user`.
3. Enter password `secret_sauce`.
4. Click **Login**.

**Expected Result:** User is redirected to the Inventory page.

---

# Test Case 2: Verify redirection to Inventory page
## Steps
1. Login with valid credentials.
2. Observe the URL.

**Expected Result:** URL ends with `inventory.html`.

---

# Test Case 3: Verify Inventory page loads correctly
## Steps
1. Login successfully.
2. Observe the page.

**Expected Result:** Inventory page loads without UI errors.

---

# Test Case 4: Verify all inventory products are displayed
## Steps
1. Login successfully.
2. Scroll through the page.

**Expected Result:** All products are displayed.

---

# Test Case 5: Verify product details are displayed correctly
## Steps
1. Login successfully.
2. Review product details.

**Expected Result:** Image, name, description, and price are displayed.

---

# Test Case 6: Verify shopping cart icon is displayed
## Steps
1. Login successfully.
2. Observe the top-right corner.

**Expected Result:** Shopping cart icon is visible.

---

# Test Case 7: Verify navigation menu options
## Steps
1. Login successfully.
2. Click the hamburger menu.

**Expected Result:** All Items, About, Logout, and Reset App State are displayed.

---

# Test Case 8: Verify page title
## Steps
1. Login successfully.
2. Observe the page title.

**Expected Result:** Title displays **Swag Labs**.

---

# Test Case 9: Verify session persistence after refresh
## Steps
1. Login successfully.
2. Refresh the browser.

**Expected Result:** User remains logged in.

---

# Test Case 10: Verify successful logout
## Steps
1. Login successfully.
2. Open the menu.
3. Click Logout.

**Expected Result:** User is redirected to the Login page.

---

# Test Case 11: Verify Inventory page cannot be accessed after logout
## Steps
1. Logout.
2. Enter `inventory.html` in the browser.

**Expected Result:** User is redirected to the Login page.

---

# Test Case 12: Verify login response time
## Steps
1. Login with valid credentials.
2. Observe loading time.

**Expected Result:** Inventory page loads within approximately 3 seconds.

---

## Coverage Summary
- Authentication
- URL validation
- Inventory page validation
- Product verification
- Shopping cart verification
- Navigation menu verification
- Session persistence
- Logout
- Access restriction
- Performance validation


