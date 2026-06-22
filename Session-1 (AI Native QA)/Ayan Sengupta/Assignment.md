**QA AI Workshop \- Assignment Template**

*DemoBlaze E2E Purchase Flow*

| Member Name | Ayan Sengupta |
| :---- | :---- |
| **Assigned Website** | [https://www.demoblaze.com/](https://www.demoblaze.com/) |
| **Flow Type** | Complete Product Purchase E2E Flow |
| **Submission Type** | Manual \+ AI \+ Final Automation-Ready Test Case |

**QA Manual Test Cases:-**

Member 1:- Ayan Sengupta

Query/Test cases:- DemoBlaze \- Complete Product Purchase E2E Flow ([https://www.demoblaze.com/](https://www.demoblaze.com/))

*Human Thinking Test Cases*

***Sign Up Flow***

**TestCases\_001:- Verify successful sign up with valid username and password** 

1\. Go to [https://www.demoblaze.com/](https://www.demoblaze.com/)

2\. Click on the Sign up button from the Header.

3\. Verify that the Sign up modal is displayed.

4\. Enter a new valid username.

5\. Enter a valid password.

6\. Click on the Sign up button.

7\. Verify that the successful sign up confirmation alert is displayed.

  8\. Verify that the alert is closed successfully. 

**TestCases\_002:- Verify sign up validation with blank username and blank password**


1\. Go to [https://www.demoblaze.com/](https://www.demoblaze.com/)

2\. Click on the Sign up button from the Header.

3\. Verify that the Sign up modal is displayed.

  4\. Enter Blank Username with spaces

  5\. Enter Blank password with spaces

  6\. Click on the Sign up button

  7\. Error Toast should appear or inline error message should appear


**TestCases\_003:- Verify sign up validation with blank username and valid password**


1\. Go to [https://www.demoblaze.com/](https://www.demoblaze.com/)

2\. Click on the Sign up button from the Header.

3\. Verify that the Sign up modal is displayed.

  4\. Enter Blank Username with spaces

  5\. Enter valid password with spaces

  6\. Click on the Sign up button

  7\. Error Toast should appear or inline error message should appear

**TestCases\_004:- Verify sign up validation with valid username and blank password**


1\. Go to [https://www.demoblaze.com/](https://www.demoblaze.com/)

2\. Click on the Sign up button from the Header.

3\. Verify that the Sign up modal is displayed.

  4\. Enter a new valid username.

5\. Enter a blank password.

6\. Click on the Sign up button.

  7\. Error Toast should appear or inline error message should appear

**TestCases\_005:- Verify sign up with valid already registered user name and password**


1\. Go to [https://www.demoblaze.com/](https://www.demoblaze.com/)

2\. Click on the Sign up button from the Header.

3\. Verify that the Sign up modal is displayed.

  4\. Enter an already registered username.

5\. Enter an already registered password.

6\. Click on the Sign up button.

  7\. Error Toast should appear telling the user has already been registered

**TestCases\_006:- Verify sign up with valid already registered user name and password**


1\. Go to [https://www.demoblaze.com/](https://www.demoblaze.com/)

2\. Click on the Sign up button from the Header.

3\. Verify that the Sign up modal is displayed.

  4\. Enter an already registered username.

5\. Enter an already registered password.

6\. Click on the Sign up button.

  7\. Error Toast should appear telling the user has already been registered

***Log in Flow***

**TestCases\_007:- Verify successful Login with registered username and password** 

1\. Go to [https://www.demoblaze.com/](https://www.demoblaze.com/)

2\. Click on the Log in button from the Header.

3\. Verify that the Log in modal is displayed.

4\. Enter registered username.

5\. Enter a registered password.

6\. Click on the Log in button.

7\. Verify that the successful Log in confirmation message should be displayed

8\. Click on the OK button.

9\. Verify that the modal is closed successfully. 

10\. Registered mail id should appear in header

**TestCases\_008:- Verify Login validation with blank username and blank password**


1\. Go to [https://www.demoblaze.com/](https://www.demoblaze.com/)

2\. Click on the Login button from the Header.

3\. Verify that the Login modal is displayed.

  4\. Enter Blank Username with spaces

  5\. Enter Blank password with spaces

  6\. Click on the Login button

  7\. Error Toast should appear or inline error message should appear


**TestCases\_009:- Verify Login validation with blank username and valid password**


1\. Go to [https://www.demoblaze.com/](https://www.demoblaze.com/)

2\. Click on the Login button from the Header.

3\. Verify that the Login modal is displayed.

  4\. Enter Blank Username with spaces

  5\. Enter valid password with spaces

  6\. Click on the Login button

  7\. Error Toast should appear or inline error message should appear

**TestCases\_010:- Verify Login validation with valid username and blank password**


1\. Go to [https://www.demoblaze.com/](https://www.demoblaze.com/)

2\. Click on the Login button from the Header.

3\. Verify that the Login modal is displayed.

  4\. Enter a new valid username.

5\. Enter a blank password.

6\. Click on the Login button.

  7\. Error Toast should appear or inline error message should appear

**TestCases\_011:- Verify Login with valid registered user name and invalid non registered password**


1\. Go to [https://www.demoblaze.com/](https://www.demoblaze.com/)

2\. Click on the Login button from the Header.

3\. Verify that the Login modal is displayed.

  4\. Enter a registered username.

5\. Enter invalid non registered password.

6\. Click on the Login button.

  7\. Error Toast should appear telling credentials wrong

**TestCases\_012:- Verify Login with invalid non registered user name and valid registered password**


1\. Go to [https://www.demoblaze.com/](https://www.demoblaze.com/)

2\. Click on the Login  button from the Header.

3\. Verify that the Login  modal is displayed.

  4\. Enter an invalid non registered user name.

5\. Enter an valid registered password.

6\. Click on the Login  button.

  7\. Error Toast should appear telling credentials wrong.

**TestCases\_013:- Verify Login with invalid non registered user name and invalid non registered password**


1\. Go to [https://www.demoblaze.com/](https://www.demoblaze.com/)

2\. Click on the Login  button from the Header.

3\. Verify that the Login  modal is displayed.

  4\. Enter an invalid non registered user name.

5\. Enter invalid non registered password.

6\. Click on the Login  button.

  7\. Error Toast should appear telling credentials wrong.

**TestCases\_014:- Verify Login with invalid non registered user name and invalid non registered password**


1\. Go to [https://www.demoblaze.com/](https://www.demoblaze.com/)

2\. Click on the Login  button from the Header.

3\. Verify that the Login  modal is displayed.

  4\. Enter an invalid non registered user name.

5\. Enter invalid non registered password.

6\. Click on the Login  button.

  7\. Error Toast should appear telling credentials wrong.

**TestCases\_015:- Verify Login without entering user name and password**


1\. Go to [https://www.demoblaze.com/](https://www.demoblaze.com/)

2\. Click on the Login  button from the Header.

3\. Verify that the Login modal is displayed.

  4\. Click on the Login  button.

  5\. Error Toast should appear telling filling password and username.

**TestCases\_016:- Verify Login without entering user name and password**


1\. Go to [https://www.demoblaze.com/](https://www.demoblaze.com/)

2\. Click on the Login  button from the Header.

3\. Verify that the Login modal is displayed.

  4\. Click on the Login  button.

  5\. Error Toast should appear telling filling password and username.

**TestCases\_017:- Verify password field should have eye button** 


1\. Go to [https://www.demoblaze.com/](https://www.demoblaze.com/)

2\. Click on the Login button from the Header.

3\. Verify that the Login modal is displayed.

  4\. Check whether the Password field contains an eye button.

***Cross Browser Testing***

**TestCases\_018:- Verify whether the website opens and runs properly in different browsers**

1\. Open different browsers like Firefox, Chrome, Opera, Edge.

2\. Go to [https://www.demoblaze.com/](https://www.demoblaze.com/)

3\. Verify all the functionalities of the website by running it in different browsers

***Add to cart Flow***

**TestCases\_019:- Verify whether user can properly add the product to cart**

1\. Go to [https://www.demoblaze.com/](https://www.demoblaze.com/)

2\. Click on the product in the home page’s product list.

3\. Verify that the Add to cart button appears after redirection to the product details page.

4\. Click on Add to cart button.

5\. Check for a success message.

6\. Check whether product name , Product price , product quantity and the calculation breakdown are proper in cart

**TestCases\_020:- Verify system prevents user to add out of stock item to cart**

1\. Go to [https://www.demoblaze.com/](https://www.demoblaze.com/)

2\. Pickup an out of product from the product list.

3\. When the user tries to add the out of stock. Product to cart system should show an error message preventing the user to add the product to cart4. Click on Add to cart button.

**TestCases\_021- Verify system prevents user to add product quantity which is more than available in inventory stock item to cart**

1\. Go to [https://www.demoblaze.com/](https://www.demoblaze.com/)

2\. Click on the product in the home page’s product list.

3\. Verify that the Add to cart button appears after redirection to the product details page.

4\. Add the quantity that more than available in stock

5\. System should prevent user to add quantity of that product which is more than present in inventory stock

***Checkout flow*** 

**TestCases\_022:- Verify whether user properly checkout with product added to cart**

1\. Go to [https://www.demoblaze.com/](https://www.demoblaze.com/)

2\. Click on the product in the home page’s product list.

3\. Verify that the Add to cart button appears after redirection to the product details page.

4\. Click on Add to cart button.

5\. Check for a success message.

6\. Check whether product name , Product price , product quantity and the calculation breakdown are proper in cart

7\. Click on Place Order button 

8\. Fill the billing details form

9\. Provide payment card details

10\. Click on Purchase Button

**TestCases\_023:- Verify whether after proper checkout proper order confirmation details are fetched.**

1\. Go to [https://www.demoblaze.com/](https://www.demoblaze.com/)

2\. Click on the product in the home page’s product list.

3\. Verify that the Add to cart button appears after redirection to the product details page.

4\. Click on Add to cart button.

5\. Check for a success message.

6\. Check whether product name , Product price , product quantity and the calculation breakdown are proper in cart

7\. Click on Place Order button 

8\. Fill the billing details form

9\. Provide payment card details

10\. Click on Purchase Button

11\. Check for thank you message and the order details

 **TestCases\_024:- Verify whether System prevents user from checkout and purchase if without filling billing address**

 1\. Go to [https://www.demoblaze.com/](https://www.demoblaze.com/)

2\. Click on the product in the home page’s product list.

3\. Verify that the Add to cart button appears after redirection to the product details page.

4\. Click on Add to cart button.

5\. Check for a success message.

6\. Check whether product name , Product price , product quantity and the calculation breakdown are proper in cart

7\. Click on Place Order button 

8\. Without Filling the billing details form

9\. Click on Purchase Button

10\. System should prevent user from purchase

 **TestCases\_024:- Verify whether System prevents user from checkout and purchase if proper card details are not given.**

 1\. Go to [https://www.demoblaze.com/](https://www.demoblaze.com/)

2\. Click on the product in the home page’s product list.

3\. Verify that the Add to cart button appears after redirection to the product details page.

4\. Click on Add to cart button.

5\. Check for a success message.

6\. Check whether product name , Product price , product quantity and the calculation breakdown are proper in cart

7\. Click on Place Order button 

8\. Fill the billing details form

9\. Provide invalid card details ( expired cards , Wrong Card Number , Wrong CVV number )

10\. Click on Purchase Button

10\. System should prevent user from purchase

**TestCases\_025:- Verify whether in case of payment failure proper error message should appear and user should be instructed to retry without deducting any amount from user account.**

1\. Go to [https://www.demoblaze.com/](https://www.demoblaze.com/)

2\. Click on the product in the home page’s product list.

3\. Verify that the Add to cart button appears after redirection to the product details page.

4\. Click on Add to cart button.

5\. Check for a success message.

6\. Check whether product name , Product price , product quantity and the calculation breakdown are proper in cart

7\. Click on Place Order button 

8\. Fill the billing details form

9\. Provide payment card details of an account with zero balance

10\. Click on Purchase Button

11\. Check for error message with proper explanation of payment not process and instructing user to retry 

11\. **AI Manual Test Cases:-**

Member 1:- Ayan Sengupta

Prompt:- See the Screenshots analyze an understand the feature and flow of demo blaze write manual  functional test cases for DemoBlaze complete E2E purchase flow where a user logs in, selects a product, adds it to the cart, places an order, and verifies successful purchase confirmation. Out Put will be in Table format. Both Positive and Negative test cases should be included..

### **DemoBlaze Complete E2E Purchase Flow \- Manual Functional Test Cases**

| Test Case ID | Test Type | Test Scenario | Pre-Condition | Test Steps | Test Data | Expected Result |
| ----- | ----- | ----- | ----- | ----- | ----- | ----- |
| TestCases\_001 | Positive | Verify successful login with valid credentials | User should have a valid registered DemoBlaze account | 1\. Go to [https://www.demoblaze.com/](https://www.demoblaze.com/) 2\. Click on the Log in button from the navigation bar. 3\. Enter valid username. 4\. Enter valid password. 5\. Click on the Log in button. | Username: avbps202026@yopmail.com Password: Valid Password | User should be logged in successfully and the Welcome username should be displayed in the navigation bar. |
| TestCases\_002 | Negative | Verify login validation with blank username and blank password | User should be on the DemoBlaze homepage | 1\. Go to [https://www.demoblaze.com/](https://www.demoblaze.com/) 2\. Click on the Log in button. 3\. Keep the Username field blank. 4\. Keep the Password field blank. 5\. Click on the Log in button. | Username: Blank Password: Blank | Proper validation alert/message should be displayed and user should not be logged in. |
| TestCases\_003 | Negative | Verify login validation with invalid username and valid password | User should be on the Login modal | 1\. Click on the Log in button. 2\. Enter an invalid username. 3\. Enter a valid password. 4\. Click on the Log in button. | Username: invaliduser@yopmail.com Password: Valid Password | User should not be logged in and proper invalid user validation message should be displayed. |
| TestCases\_004 | Negative | Verify login validation with valid username and wrong password | User should have a valid registered username | 1\. Click on the Log in button. 2\. Enter valid username. 3\. Enter wrong password. 4\. Click on the Log in button. | Username: avbps202026@yopmail.com Password: Wrong Password | User should not be logged in and proper wrong password validation message should be displayed. |
| TestCases\_005 | Positive | Verify product category and product listing on homepage | User should be logged in successfully | 1\. Go to the DemoBlaze homepage. 2\. Verify product categories are displayed. 3\. Click on Phones category. 4\. Verify that phone products are displayed. | Category: Phones | Products related to the selected category should be displayed properly. |
| TestCases\_006 | Positive | Verify product details page opens after selecting a product | User should be logged in and products should be visible | 1\. Click on the Samsung galaxy s6 product from the product list. 2\. Verify that the product details page is opened. 3\. Verify product image, name, price, and description. | Product: Samsung galaxy s6 | Product details page should open successfully with product image, product name, price, and description. |
| TestCases\_007 | Positive | Verify product can be added to cart successfully | User should be on the product details page | 1\. Click on the Add to cart button. 2\. Verify that product added alert/message is displayed. 3\. Click on OK button from the alert. | Product: Samsung galaxy s6 | Product should be added to the cart successfully and alert/message should display “Product added.” |
| TestCases\_008 | Positive | Verify selected product is displayed on cart page | Product should be added to the cart | 1\. Click on the Cart button from the navigation bar. 2\. Verify that the cart page is opened. 3\. Verify product image, title, and price in the cart. | Product: Samsung galaxy s6 Price: 360 | Added product should be displayed in the cart with correct title and price. |
| TestCases\_009 | Positive | Verify total amount is calculated correctly on cart page | Product should be available in the cart | 1\. Open the Cart page. 2\. Check the product price. 3\. Check the Total amount displayed beside the cart. | Product Price: 360 | Total amount should match the added product price. |
| TestCases\_010 | Positive | Verify Place Order modal opens from cart page | Product should be available in the cart | 1\. Click on the Place Order button. 2\. Verify that Place Order modal is displayed. 3\. Verify Total, Name, Country, City, Credit card, Month, and Year fields are displayed. | Total: 360 | Place Order modal should open successfully with all required order fields. |
| TestCases\_011 | Positive | Verify successful purchase with valid order details | Product should be available in the cart and Place Order modal should be open | 1\. Enter valid customer name. 2\. Enter country. 3\. Enter city. 4\. Enter credit card number. 5\. Enter month. 6\. Enter year. 7\. Click on the Purchase button. | Name: Bikas Pal Country: India City: Kolkata Credit Card: 646444646 Month: 12 Year: 2026 | Purchase should be completed successfully and confirmation popup should be displayed. |
| TestCases\_012 | Positive | Verify purchase confirmation popup details after successful order | Purchase should be completed successfully | 1\. Complete the purchase flow with valid details. 2\. Verify confirmation popup is displayed. 3\. Verify confirmation message. 4\. Verify order ID, amount, card number, name, and date are displayed. | Product Amount: 360 USD Name: Bikas Pal | Confirmation popup should display “Thank you for your purchase\!” along with order ID, amount, card number, name, and date. |
| TestCases\_013 | Positive | Verify OK button functionality on purchase confirmation popup | Purchase confirmation popup should be displayed | 1\. Click on the OK button from the confirmation popup. 2\. Verify that the popup is closed. | Action: Click OK | Confirmation popup should close successfully after clicking OK. |
| TestCases\_014 | Negative | Verify purchase validation with blank Name field | Product should be available in cart and Place Order modal should be open | 1\. Keep the Name field blank. 2\. Enter valid country. 3\. Enter valid city. 4\. Enter valid credit card. 5\. Enter valid month and year. 6\. Click on Purchase. | Name: Blank Credit Card: 646444646 | Purchase should not be completed and proper validation message should be displayed for blank Name field. |
| TestCases\_015 | Negative | Verify purchase validation with blank Credit Card field | Product should be available in cart and Place Order modal should be open | 1\. Enter valid name. 2\. Enter valid country. 3\. Enter valid city. 4\. Keep Credit card field blank. 5\. Enter valid month and year. 6\. Click on Purchase. | Name: Bikas Pal Credit Card: Blank | Purchase should not be completed and proper validation message should be displayed for blank Credit card field. |
| TestCases\_016 | Negative | Verify purchase validation when all order fields are blank | Product should be available in cart and Place Order modal should be open | 1\. Keep all fields blank in the Place Order modal. 2\. Click on the Purchase button. | Name: Blank Country: Blank City: Blank Credit Card: Blank Month: Blank Year: Blank | Purchase should not be completed and proper validation message should be displayed. |
| TestCases\_017 | Negative | Verify purchase behavior with invalid credit card value | Product should be available in cart and Place Order modal should be open | 1\. Enter valid name. 2\. Enter valid country. 3\. Enter valid city. 4\. Enter invalid credit card value. 5\. Enter valid month and year. 6\. Click on Purchase. | Credit Card: abcd@123 | System should not accept invalid credit card value and proper validation should be displayed. |
| TestCases\_018 | Negative | Verify purchase behavior with blank Country field | Product should be available in cart and Place Order modal should be open | 1\. Enter valid name. 2\. Keep Country field blank. 3\. Enter valid city. 4\. Enter valid credit card. 5\. Enter valid month and year. 6\. Click on Purchase. | Country: Blank | System should not allow purchase without country and proper validation should be displayed. |
| TestCases\_019 | Negative | Verify purchase behavior with blank City field | Product should be available in cart and Place Order modal should be open | 1\. Enter valid name. 2\. Enter valid country. 3\. Keep City field blank. 4\. Enter valid credit card. 5\. Enter valid month and year. 6\. Click on Purchase. | City: Blank | System should not allow purchase without city and proper validation should be displayed. |
| TestCases\_020 | Negative | Verify purchase behavior with blank Month and Year fields | Product should be available in cart and Place Order modal should be open | 1\. Enter valid name. 2\. Enter valid country. 3\. Enter valid city. 4\. Enter valid credit card. 5\. Keep Month and Year fields blank. 6\. Click on Purchase. | Month: Blank Year: Blank | System should not allow purchase without month and year and proper validation should be displayed. |
| TestCases\_021 | Positive | Verify Close button functionality on Place Order modal | Place Order modal should be open | 1\. Open the cart page. 2\. Click on Place Order. 3\. Verify Place Order modal is displayed. 4\. Click on the Close button. | Action: Click Close | Place Order modal should be closed successfully and order should not be placed. |
| TestCases\_022 | Positive | Verify X icon functionality on Place Order modal | Place Order modal should be open | 1\. Open the Place Order modal. 2\. Click on the X icon from the top-right corner. | Action: Click X icon | Place Order modal should be closed successfully without placing an order. |
| TestCases\_023 | Positive | Verify product delete functionality from cart | Product should be available in the cart | 1\. Go to the Cart page. 2\. Click on the Delete link for the added product. 3\. Verify that the product is removed from the cart. 4\. Verify that total amount is updated. | Product: Samsung galaxy s6 | Product should be removed from the cart and total amount should be updated correctly. |
| TestCases\_024 | Negative | Verify Place Order functionality when cart is empty | Cart should not contain any product | 1\. Go to the Cart page. 2\. Make sure no product is available in the cart. 3\. Click on Place Order if available. | Cart: Empty | System should not allow the user to place an order with an empty cart. |
| TestCases\_025 | Positive | Verify Logout after completing purchase flow | User should be logged in and purchase should be completed | 1\. Complete the purchase flow successfully. 2\. Click on the Log out button from the navigation bar. 3\. Verify that the user is logged out. | Action: Click Log out | User should be logged out successfully and Login/Sign up options should be displayed again. |

**Your thoughts:-**

**● What you felt Suitable:-**

**The AI-generated test cases were suitable because they presented the DemoBlaze E2E purchase flow in a more structured and professional format. Compared to the human-written test cases, the AI output clearly separated the Test Case ID, Test Type, Test Scenario, Pre-Condition, Test Steps, Test Data, and Expected Result. This made the test cases easier to read, review, and convert into automation scripts.**

**The AI performed better in organizing the complete purchase journey step by step, starting from successful login, product category verification, product details validation, add to cart, cart page validation, place order modal verification, successful purchase, confirmation popup validation, product deletion from cart, empty cart scenario, and logout after purchase.**

**The AI also added better validation points for the order confirmation popup, such as verifying the thank you message, order ID, amount, card number, customer name, and date. These are important checkpoints for an E2E purchase flow and make the final test case more complete.**

**Another suitable point is that the AI included positive and negative test cases in a clean table format. It also added pre-conditions and test data, which were missing or less structured in the human-thinking section. This makes the AI-generated version more documentation-friendly and automation-ready.**

**● What you felt Not suitable:-**

**The AI-generated test cases were not fully suitable because they missed some areas that were covered in the human-thinking test cases. For example, the human-written section included Sign Up flow, Cross Browser Testing, out-of-stock product scenarios, inventory quantity validation, billing address validation, invalid card details, and payment failure scenarios. These are important QA areas, but the AI mostly focused on the main purchase flow and did not cover all wider functional possibilities.**

**The AI also assumed that all Place Order fields such as Country, City, Month, and Year must have strict validation. This may not always match the actual DemoBlaze behavior, so these validations need to be verified manually before keeping them as final expected results.**

**The AI missed some website-specific observations from the human-thinking side, such as checking whether the password field has an eye button, checking blank inputs with spaces, and testing the website behavior across multiple browsers. However, some of these points should also be refined because DemoBlaze may not actually provide some features like an eye icon or stock/quantity handling.**

**Another issue is that the AI did not include the Sign Up flow, even though sign up is important before login and purchase for a new user journey. It also did not deeply cover real payment failure scenarios, expired card, wrong CVV, or zero-balance card scenarios. Since DemoBlaze is a demo website, these payment-related cases may need to be written carefully as theoretical negative scenarios instead of confirmed system behavior.**

**Overall, the AI performed better in formatting, structure, clarity, pre-condition writing, test data usage, and expected result writing. The human-thinking test cases performed better in wider QA coverage, edge case imagination, and identifying additional functional areas beyond the main E2E flow. So, the final test case should combine the AI’s structured format with the human-written edge cases and website-specific observations.**

### **Automation Framework and Tech Stack**

**The final automation-ready test cases will be automated using a Java-based Selenium automation framework with TestNG and Cucumber BDD integration.**

**Framework / Tech Stack Used:**

| Area | Technology / Approach |
| ----- | ----- |
| **Programming Language** | **Java** |
| **Automation Tool** | **Selenium WebDriver** |
| **Test Runner** | **TestNG** |
| **BDD Framework** | **Cucumber** |
| **Cucumber-TestNG Integration** | **`AbstractTestNGCucumberTests`** |
| **Test Data Handling** | **TestNG `DataProvider` and `.properties` files** |
| **Configuration Handling** | **`.properties` files** |
| **Test Execution Style** | **Cucumber Feature Files \+ Step Definitions \+ TestNG Runner** |
| **Validation Approach** | **Assertions and UI verification through Selenium** |
| **Reporting** | **TestNG/Cucumber execution report** |

**Framework Approach:**

1. **Cucumber Feature Files will be used to define the DemoBlaze E2E purchase flow in a readable BDD format.**  
2. **Step Definition classes will contain the implementation of each Given, When, Then, and And step.**  
3. **The Test Runner class will extend `AbstractTestNGCucumberTests` to execute Cucumber scenarios with TestNG.**  
4. **Test data such as username, password, customer name, country, city, card number, month, year, product name, and expected messages will be handled using TestNG `DataProvider` and `.properties` files.**  
5. **Common configuration values such as browser name, application URL, timeout values, and environment details will be stored in `.properties` files.**  
6. **Selenium WebDriver will be used to interact with DemoBlaze UI elements such as Sign up modal, Login modal, product cards, Add to cart button, Cart page, Place Order modal, and Purchase confirmation popup.**  
7. **Assertions will be used to verify important checkpoints like successful login, product details visibility, cart product details, total amount, order confirmation message, order ID, amount, card number, customer name, and date.**  
8. **The automation flow will be designed in a reusable and maintainable way so that positive and negative test scenarios can be executed with different test data sets.**

### **Final Automation-Ready Test Cases**

| TC ID | Test Scenario | Preconditions | Test Steps | Test Data | Expected Result | Automation Priority |
| ----- | ----- | ----- | ----- | ----- | ----- | ----- |
| **TC\_001** | **User Sign Up with Valid Data** | **User is on DemoBlaze homepage** | **Click Sign Up → Enter username and password → Click Sign Up** | **Username, Password** | **User account is created successfully and success alert is displayed** | **Medium** |
| **TC\_002** | **Login with Valid Credentials** | **Registered user exists** | **Click Login → Enter username and password → Click Login** | **Username, Password** | **User is logged in successfully and username is displayed in header** | **High** |
| **TC\_003** | **Login with Blank Credentials** | **User is on Login modal** | **Click Login without entering data** | **Blank Username, Blank Password** | **Validation message or login failure is displayed** | **Medium** |
| **TC\_004** | **Verify Product Details Page** | **User is logged in** | **Select category → Click product** | **Product Name** | **Product image, name, price, and description are displayed correctly** | **High** |
| **TC\_005** | **Add Product to Cart** | **User is on Product Details page** | **Click Add to Cart** | **Product Name** | **Product added confirmation alert is displayed** | **High** |
| **TC\_006** | **Verify Product in Cart** | **Product added to cart** | **Navigate to Cart page** | **Product Name** | **Product name and price match selected product** | **High** |
| **TC\_007** | **Verify Cart Total Amount** | **Product exists in cart** | **Open Cart page** | **Product Price** | **Total amount equals product price** | **High** |
| **TC\_008** | **Delete Product from Cart** | **Product exists in cart** | **Click Delete against product** | **Product Name** | **Product is removed from cart successfully** | **Medium** |
| **TC\_009** | **Open Place Order Modal** | **Product exists in cart** | **Click Place Order** | **N/A** | **Place Order modal is displayed successfully** | **High** |
| **TC\_010** | **Verify Place Order Modal Close Functionality** | **Place Order modal is open** | **Click Close button and X icon** | **N/A** | **Modal closes successfully** | **Medium** |
| **TC\_011** | **Complete Purchase with Valid Data** | **Product exists in cart** | **Open Place Order → Enter customer details → Click Purchase** | **Name, Country, City, Card, Month, Year** | **Purchase confirmation popup is displayed successfully** | **High** |
| **TC\_012** | **Verify Purchase Confirmation Details** | **Purchase completed** | **Capture confirmation popup details** | **Order Details** | **Order ID, Amount, Card Number, Name, and Date are displayed correctly** | **High** |
| **TC\_013** | **Purchase with Mandatory Fields Blank** | **Place Order modal is open** | **Leave mandatory fields blank → Click Purchase** | **Blank Data** | **Appropriate validation or purchase failure behavior is displayed** | **Medium** |
| **TC\_014** | **Logout Successfully** | **User is logged in** | **Click Logout** | **N/A** | **User is logged out and Login option is displayed** | **High** |

### **Final E2E Automation Flow Summary**

1. **Launch browser using Selenium WebDriver.**  
2. **Read application URL and browser configuration from `.properties` file.**  
3. **Navigate to [https://www.demoblaze.com/](https://www.demoblaze.com/)**  
4. **Perform Sign up flow with unique test data if a new user is required.**  
5. **Perform Login flow using valid credentials from test data.**  
6. **Verify that the logged-in username is displayed in the header.**  
7. **Select a product category.**  
8. **Select a product from the product list.**  
9. **Verify product details page with product image, name, price, and description.**  
10. **Click on Add to cart.**  
11. **Accept the product added alert/message.**  
12. **Navigate to the Cart page.**  
13. **Verify product title and price in the cart.**  
14. **Verify total amount calculation.**  
15. **Click on Place Order.**  
16. **Fill order details using data from `DataProvider` / `.properties` file.**  
17. **Click on Purchase.**  
18. **Verify purchase confirmation popup.**  
19. **Verify order ID, amount, card number, customer name, and date.**  
20. **Click on OK.**  
21. **Log out from the application.**  
22. **Execute the scenarios using Cucumber with TestNG runner by extending `AbstractTestNGCucumberTests`.**

### **Automation Priority**

**High Priority**

* **Login with valid credentials**  
* **Product details verification**  
* **Add to cart**  
* **Cart validation**  
* **Place order**  
* **Purchase confirmation validation**  
* **Logout**

**Medium Priority**

* **Sign up validation**  
* **Blank login validation**  
* **Blank checkout field validation**  
* **Cart delete functionality**  
* **Place Order modal Close/X icon functionality**

**Low Priority**

* **Cross browser testing**  
* **Empty cart checkout behavior**  
* **Invalid credit card behavior (depending on actual DemoBlaze validation support)**

### **DemoBlaze Complete E2E Purchase Flow \- Final Automation Ready Test Cases**

| Test Case ID | Test Type | Module / Flow | Test Scenario | Pre-Condition | Test Steps | Test Data | Expected Result |
| ----- | ----- | ----- | ----- | ----- | ----- | ----- | ----- |
| **TestCases\_001** | **Positive** | **Sign Up Flow** | **Verify successful sign up with valid username and password** | **DemoBlaze website should be accessible and username should be new** | **1\. Go to [https://www.demoblaze.com/](https://www.demoblaze.com/) 2\. Click on the Sign up button from the header. 3\. Verify that the Sign up modal is displayed. 4\. Enter a new valid username. 5\. Enter a valid password. 6\. Click on the Sign up button. 7\. Verify that the success alert is displayed. 8\. Accept the alert.** | **Username: New unique username Password: Valid password** | **User should be registered successfully and success alert should be displayed.** |
| **TestCases\_002** | **Negative** | **Sign Up Flow** | **Verify sign up validation with blank username and blank password** | **DemoBlaze website should be accessible** | **1\. Go to [https://www.demoblaze.com/](https://www.demoblaze.com/) 2\. Click on the Sign up button from the header. 3\. Verify that the Sign up modal is displayed. 4\. Keep Username field blank. 5\. Keep Password field blank. 6\. Click on the Sign up button. 7\. Verify validation alert/message.** | **Username: Blank Password: Blank** | **User should not be registered and validation alert/message should be displayed.** |
| **TestCases\_003** | **Negative** | **Sign Up Flow** | **Verify sign up validation with already registered username** | **User should already be registered with the same username** | **1\. Go to [https://www.demoblaze.com/](https://www.demoblaze.com/) 2\. Click on the Sign up button from the header. 3\. Enter an already registered username. 4\. Enter a valid password. 5\. Click on the Sign up button. 6\. Verify duplicate user validation alert/message.** | **Username: Existing registered username Password: Valid password** | **System should prevent duplicate registration and display proper validation alert/message.** |
| **TestCases\_004** | **Positive** | **Login Flow** | **Verify successful login with valid registered username and password** | **User should have a valid registered account** | **1\. Go to [https://www.demoblaze.com/](https://www.demoblaze.com/) 2\. Click on the Log in button from the header. 3\. Verify that the Log in modal is displayed. 4\. Enter valid registered username. 5\. Enter valid registered password. 6\. Click on the Log in button. 7\. Verify that the user is logged in successfully.** | **Username: Valid registered username Password: Valid registered password** | **User should be logged in successfully and Welcome username should be displayed in the header.** |
| **TestCases\_005** | **Negative** | **Login Flow** | **Verify login validation with blank username and blank password** | **DemoBlaze website should be accessible** | **1\. Go to [https://www.demoblaze.com/](https://www.demoblaze.com/) 2\. Click on the Log in button from the header. 3\. Verify that the Log in modal is displayed. 4\. Keep Username field blank. 5\. Keep Password field blank. 6\. Click on the Log in button. 7\. Verify validation alert/message.** | **Username: Blank Password: Blank** | **User should not be logged in and validation alert/message should be displayed.** |
| **TestCases\_006** | **Negative** | **Login Flow** | **Verify login validation with valid username and invalid password** | **User should have a valid registered username** | **1\. Go to [https://www.demoblaze.com/](https://www.demoblaze.com/) 2\. Click on the Log in button from the header. 3\. Enter valid registered username. 4\. Enter invalid password. 5\. Click on the Log in button. 6\. Verify login error alert/message.** | **Username: Valid registered username Password: Invalid password** | **User should not be logged in and proper error alert/message should be displayed.** |
| **TestCases\_007** | **Negative** | **Login Flow** | **Verify login validation with invalid username and valid password** | **DemoBlaze website should be accessible** | **1\. Go to [https://www.demoblaze.com/](https://www.demoblaze.com/) 2\. Click on the Log in button from the header. 3\. Enter invalid/non-registered username. 4\. Enter valid password. 5\. Click on the Log in button. 6\. Verify login error alert/message.** | **Username: Invalid username Password: Valid password** | **User should not be logged in and proper error alert/message should be displayed.** |
| **TestCases\_008** | **Positive** | **Product Listing Flow** | **Verify product categories are displayed on homepage** | **User should be on DemoBlaze homepage** | **1\. Go to [https://www.demoblaze.com/](https://www.demoblaze.com/) 2\. Verify that product categories are displayed. 3\. Verify Phones category. 4\. Verify Laptops category. 5\. Verify Monitors category.** | **Categories: Phones, Laptops, Monitors** | **Product categories should be displayed properly on the homepage.** |
| **TestCases\_009** | **Positive** | **Product Listing Flow** | **Verify products are displayed after selecting category** | **User should be on DemoBlaze homepage** | **1\. Go to [https://www.demoblaze.com/](https://www.demoblaze.com/) 2\. Click on Phones category. 3\. Verify that phone products are displayed.** | **Category: Phones** | **Products related to the selected category should be displayed.** |
| **TestCases\_010** | **Positive** | **Product Details Flow** | **Verify product details page opens after selecting a product** | **Product should be visible on homepage/product listing** | **1\. Go to [https://www.demoblaze.com/](https://www.demoblaze.com/) 2\. Click on Samsung galaxy s6 product. 3\. Verify product details page is opened. 4\. Verify product image is displayed. 5\. Verify product name is displayed. 6\. Verify product price is displayed. 7\. Verify product description is displayed.** | **Product: Samsung galaxy s6** | **Product details page should open successfully with product image, name, price, and description.** |
| **TestCases\_011** | **Positive** | **Add to Cart Flow** | **Verify product can be added to cart successfully** | **User should be on product details page** | **1\. Click on the Add to cart button. 2\. Verify product added alert/message is displayed. 3\. Accept the alert/message.** | **Product: Samsung galaxy s6** | **Product should be added to cart successfully and “Product added.” alert/message should be displayed.** |
| **TestCases\_012** | **Positive** | **Cart Flow** | **Verify added product is displayed on cart page** | **Product should be added to cart** | **1\. Click on the Cart button from the header. 2\. Verify that the Cart page is opened. 3\. Verify product image is displayed. 4\. Verify product title is displayed. 5\. Verify product price is displayed.** | **Product: Samsung galaxy s6 Price: 360** | **Added product should be displayed in the cart with correct title and price.** |
| **TestCases\_013** | **Positive** | **Cart Flow** | **Verify total amount is displayed correctly on cart page** | **Product should be available in the cart** | **1\. Open the Cart page. 2\. Capture the product price. 3\. Capture the Total amount. 4\. Compare product price with Total amount.** | **Product Price: 360** | **Total amount should match the added product price.** |
| **TestCases\_014** | **Positive** | **Cart Flow** | **Verify product delete functionality from cart** | **Product should be available in the cart** | **1\. Open the Cart page. 2\. Click on the Delete link for the product. 3\. Verify that the product is removed from the cart. 4\. Verify that the total amount is updated/cleared.** | **Product: Samsung galaxy s6** | **Product should be removed from the cart successfully and total amount should be updated/cleared.** |
| **TestCases\_015** | **Positive** | **Checkout Flow** | **Verify Place Order modal opens from cart page** | **Product should be available in cart** | **1\. Open the Cart page. 2\. Click on the Place Order button. 3\. Verify that the Place Order modal is displayed. 4\. Verify Total value is displayed. 5\. Verify Name, Country, City, Credit card, Month, and Year fields are displayed. 6\. Verify Close and Purchase buttons are displayed.** | **Total: 360** | **Place Order modal should open successfully with all order fields and action buttons.** |
| **TestCases\_016** | **Positive** | **Checkout Flow** | **Verify successful purchase with valid order details** | **Product should be available in cart and Place Order modal should be open** | **1\. Enter valid customer name. 2\. Enter valid country. 3\. Enter valid city. 4\. Enter valid credit card number. 5\. Enter valid month. 6\. Enter valid year. 7\. Click on the Purchase button.** | **Name: Bikas Pal Country: India City: Kolkata Credit Card: 646444646 Month: 12 Year: 2026** | **Purchase should be completed successfully and confirmation popup should be displayed.** |
| **TestCases\_017** | **Positive** | **Purchase Confirmation Flow** | **Verify purchase confirmation popup details after successful order** | **Purchase should be completed successfully** | **1\. Complete purchase with valid order details. 2\. Verify confirmation popup is displayed. 3\. Verify “Thank you for your purchase\!” message is displayed. 4\. Verify Order ID is displayed. 5\. Verify Amount is displayed. 6\. Verify Card Number is displayed. 7\. Verify Name is displayed. 8\. Verify Date is displayed.** | **Name: Bikas Pal Amount: 360 USD** | **Confirmation popup should display successful purchase message along with order ID, amount, card number, customer name, and date.** |
| **TestCases\_018** | **Positive** | **Purchase Confirmation Flow** | **Verify OK button functionality on purchase confirmation popup** | **Purchase confirmation popup should be displayed** | **1\. Click on the OK button from the confirmation popup. 2\. Verify that the popup is closed successfully.** | **Action: Click OK** | **Confirmation popup should close successfully after clicking OK.** |
| **TestCases\_019** | **Negative** | **Checkout Flow** | **Verify purchase validation when all Place Order fields are blank** | **Product should be available in cart and Place Order modal should be open** | **1\. Open the Place Order modal. 2\. Keep all fields blank. 3\. Click on the Purchase button. 4\. Verify validation alert/message.** | **Name: Blank Country: Blank City: Blank Credit Card: Blank Month: Blank Year: Blank** | **Purchase should not be completed and proper validation alert/message should be displayed.** |
| **TestCases\_020** | **Negative** | **Checkout Flow** | **Verify purchase validation with blank Name field** | **Product should be available in cart and Place Order modal should be open** | **1\. Open the Place Order modal. 2\. Keep Name field blank. 3\. Enter valid country. 4\. Enter valid city. 5\. Enter valid credit card number. 6\. Enter valid month and year. 7\. Click on Purchase.** | **Name: Blank Country: India City: Kolkata Credit Card: 646444646 Month: 12 Year: 2026** | **Purchase should not be completed and validation alert/message should be displayed.** |
| **TestCases\_021** | **Negative** | **Checkout Flow** | **Verify purchase validation with blank Credit Card field** | **Product should be available in cart and Place Order modal should be open** | **1\. Open the Place Order modal. 2\. Enter valid name. 3\. Enter valid country. 4\. Enter valid city. 5\. Keep Credit card field blank. 6\. Enter valid month and year. 7\. Click on Purchase.** | **Name: Bikas Pal Credit Card: Blank** | **Purchase should not be completed and validation alert/message should be displayed.** |
| **TestCases\_022** | **Negative** | **Checkout Flow** | **Verify purchase behavior with invalid credit card value** | **Product should be available in cart and Place Order modal should be open** | **1\. Open the Place Order modal. 2\. Enter valid name. 3\. Enter valid country. 4\. Enter valid city. 5\. Enter invalid credit card value. 6\. Enter valid month and year. 7\. Click on Purchase.** | **Credit Card: abcd@123** | **System should not accept invalid credit card value and proper validation should be displayed if validation is implemented.** |
| **TestCases\_023** | **Negative** | **Checkout Flow** | **Verify purchase validation with blank Country field** | **Product should be available in cart and Place Order modal should be open** | **1\. Open the Place Order modal. 2\. Enter valid name. 3\. Keep Country field blank. 4\. Enter valid city. 5\. Enter valid credit card number. 6\. Enter valid month and year. 7\. Click on Purchase.** | **Country: Blank** | **Purchase should not be completed and validation alert/message should be displayed if country validation is implemented.** |
| **TestCases\_024** | **Negative** | **Checkout Flow** | **Verify purchase validation with blank City field** | **Product should be available in cart and Place Order modal should be open** | **1\. Open the Place Order modal. 2\. Enter valid name. 3\. Enter valid country. 4\. Keep City field blank. 5\. Enter valid credit card number. 6\. Enter valid month and year. 7\. Click on Purchase.** | **City: Blank** | **Purchase should not be completed and validation alert/message should be displayed if city validation is implemented.** |
| **TestCases\_025** | **Negative** | **Checkout Flow** | **Verify purchase validation with blank Month and Year fields** | **Product should be available in cart and Place Order modal should be open** | **1\. Open the Place Order modal. 2\. Enter valid name. 3\. Enter valid country. 4\. Enter valid city. 5\. Enter valid credit card number. 6\. Keep Month and Year fields blank. 7\. Click on Purchase.** | **Month: Blank Year: Blank** | **Purchase should not be completed and validation alert/message should be displayed if month/year validation is implemented.** |
| **TestCases\_026** | **Positive** | **Checkout Modal Flow** | **Verify Close button functionality on Place Order modal** | **Place Order modal should be open** | **1\. Open the Cart page. 2\. Click on Place Order. 3\. Verify that Place Order modal is displayed. 4\. Click on the Close button.** | **Action: Click Close** | **Place Order modal should close successfully and order should not be placed.** |
| **TestCases\_027** | **Positive** | **Checkout Modal Flow** | **Verify X icon functionality on Place Order modal** | **Place Order modal should be open** | **1\. Open the Place Order modal. 2\. Click on the X icon from the top-right corner.** | **Action: Click X icon** | **Place Order modal should close successfully without placing an order.** |
| **TestCases\_028** | **Negative** | **Cart / Checkout Flow** | **Verify Place Order behavior when cart is empty** | **Cart should not contain any product** | **1\. Go to the Cart page. 2\. Verify that no product is available in the cart. 3\. Check whether Place Order button is available. 4\. Click on Place Order if available. 5\. Verify system behavior.** | **Cart: Empty** | **System should not allow a valid purchase with an empty cart. If the modal opens, this should be treated as a validation gap/issue.** |
| **TestCases\_029** | **Positive** | **Logout Flow** | **Verify logout after completing purchase flow** | **User should be logged in** | **1\. Complete the purchase flow or stay logged in after product activity. 2\. Click on the Log out button from the header. 3\. Verify that the user is logged out successfully.** | **Action: Click Log out** | **User should be logged out successfully and Log in / Sign up buttons should be displayed again.** |
| **TestCases\_030** | **Compatibility** | **Cross Browser Testing** | **Verify DemoBlaze E2E purchase flow works across supported browsers** | **Browser should be installed and internet should be stable** | **1\. Open Chrome browser and execute the E2E purchase flow. 2\. Open Firefox browser and execute the E2E purchase flow. 3\. Open Edge browser and execute the E2E purchase flow. 4\. Verify UI and functionality behavior across browsers.** | **Browsers: Chrome, Firefox, Edge** | **DemoBlaze website and E2E purchase flow should work properly across supported browsers without major UI or functional breakage.** |

### **Final E2E Automation Flow Summary**

1. **Launch browser.**  
2. **Navigate to [https://www.demoblaze.com/](https://www.demoblaze.com/)**  
3. **Perform user sign up with unique data if a new user is required.**  
4. **Perform login with valid registered credentials.**  
5. **Verify logged-in username in the header.**  
6. **Select a product category.**  
7. **Select a product from the product list.**  
8. **Verify product details page.**  
9. **Click on Add to cart.**  
10. **Accept product added alert/message.**  
11. **Navigate to Cart page.**  
12. **Verify product title and price.**  
13. **Verify total amount.**  
14. **Click on Place Order.**  
15. **Fill valid order details.**  
16. **Click on Purchase.**  
17. **Verify purchase confirmation popup.**  
18. **Verify order ID, amount, card number, name, and date.**  
19. **Click on OK.**  
20. **Log out from the application.**

### **Automation Priority**

**High Priority:**

* **Login with valid credentials**  
* **Product details verification**  
* **Add to cart**  
* **Cart validation**  
* **Place order**  
* **Purchase confirmation validation**  
* **Logout**

**Medium Priority:**

* **Sign up validation**  
* **Blank login validation**  
* **Blank checkout field validation**  
* **Cart delete functionality**  
* **Place Order modal close/X icon functionality**

**Low Priority:**

* **Cross browser testing**  
* **Empty cart checkout behavior**  
* **Invalid credit card behavior, depending on actual DemoBlaze validation support**


