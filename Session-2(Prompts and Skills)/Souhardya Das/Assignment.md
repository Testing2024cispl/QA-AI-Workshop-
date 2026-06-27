# **Human/AI Test Case Assignment**

**Member: Souhardya Das**  
**URL: [https://rahulshettyacademy.com/seleniumPractise/\#/](https://rahulshettyacademy.com/seleniumPractise/#/)**

# **Human Thinking Test Cases:-**

**\*Pre-requisite: The URL works and opens.**

1. **Test\_Scenario\_001: Verify that searching for an existing product works.**  
   1. Test\_Case\_001: Verify that the search field is clickable or selectable.  
      1. Test\_Step\_001: Click on the search field.  
   2. Test\_Case\_002: Verify that the user can input text in the search field.  
      1. Test\_Step\_001: Enter the name of an existing product, for example: carrot.  
   3. Test\_Case\_003: Verify that the searched product is displayed.  
      1. Test\_Step\_001: Check if the expected product is displayed.

2. **Test\_Scenario\_002: Verify that searching for a non-existing/incorrect product is working.**  
   1. Test\_Case\_001: Verify that the search field is clickable or selectable.  
      1. Test\_Step\_001: Click on the search field.  
   2. Test\_Case\_002: Verify that a user can input text in the search field.  
      1. Test\_Step\_001: Enter the name of a non-existing product or a random String, for example: test.  
   3. Test\_Case\_003: Verify that an appropriate message is displayed.  
      1. Test\_Step\_001: Check if an appropriate message is displayed stating that the search did not yield any results.

3. **Test\_Scenario\_003: Verify that the quantity increment/decrement, add to cart, and delete from cart functionalities are working correctly.**  
   1. Test\_Case\_001: Verify that a user can increase/decrease the quantity of a product.  
      1. Test\_Step\_001: Click on the “+” button twice, and then click on the “-” button once for a product.  
      2. Test\_Step\_002: Check whether the product quantity matches the expected quantity.  
   2. Test\_Case\_002: Verify that a user can add a product to the cart.  
      1. Test\_Step\_001: Click on the “Add to cart” button of the product with the modified quantity.  
      2. Test\_Step\_002: Click on the cart icon.  
      3. Test\_Step\_003: Verify that the correct product has been added to the cart in the expected quantity.  
   3. Test\_Case\_003: Verify that a user can delete a product from the cart.  
      1. Test\_Step\_001: Click on the cart icon.  
      2. Test\_Step\_002: Click on the “x” button beside the product that needs to be deleted.  
      3. Test\_Step\_003: Verify that the product has been deleted from the cart.

4. **Test\_Scenario\_004: Verify that the user can add multiple products to the cart.**  
   1. Test\_Case\_001: Verify that a user can add a product to the cart.  
      1. Test\_Step\_001: Click on the “Add to cart” button of a product.  
   2. Test\_Case\_002: Verify that a user can add another product to the cart.  
      1. Test\_Step\_001: Click on the “Add to cart” button of another product.  
   3. Test\_Case\_003: Verify that both products have been added to the cart.  
      1. Test\_Step\_001: Click on the cart icon.  
      2. Test\_Step\_002: Verify that the correct products have been added to the cart.

5. **Test\_Scenario\_005: Verify that the user can successfully place an order.**  
   1. Test\_Case\_001: Verify that a user can proceed to the checkout page.  
      1. Test\_Step\_001: Click on the “Add to cart” button of a product.  
      2. Test\_Step\_002: Click on the cart icon.  
      3. Test\_Step\_003: Click on the “Proceed to checkout” button.  
   2. Test\_Case\_002: Verify that the order process can be completed.  
      1. Test\_Step\_001: Click on the “Place order” button.  
      2. Test\_Step\_002: Select a country from the “Choose country” dropdown list.  
      3. Test\_Step\_003: Select the “Agree to the Terms & Conditions” checkbox.  
      4. Test\_Step\_004: Click on the “Proceed” button.  
      5. Test\_Step\_005: Check if an appropriate message is displayed stating that the order has been successfully placed.

# **AI Test Cases:-**

## **Prompt:**

Please write manual test cases for the following website while maintaining the mentioned instructions.  
URL: https://rahulshettyacademy.com/seleniumPractise/\#/   
Only include functional test cases, including edge cases.  
Do not include security, UI/UX or any other test cases.  
Use the following format:  
Test\_Scenario\_003: Verify that the quantity increment/decrement, add to cart, and delete from cart functionalities are working correctly.  
Test\_Case\_001: Verify that a user can increase/decrease the quantity of a product. Test\_Step\_001: Click on the “+” button twice, and then click on the “-” button once for a product.  
Test\_Step\_002: Check if the quantity of the product matches the expected quantity. Test\_Case\_002: Verify that a user can add a product to the cart.  
Test\_Step\_001: Click on the “Add to cart” button of the product with the modified quantity.  
Test\_Step\_002: Click on the cart icon.  
Test\_Step\_003: Verify that the correct product has been added to the cart in the expected quantity.  
Test\_Case\_003: Verify that a user can delete a product from the cart. Test\_Step\_001: Click on the cart icon.  
Test\_Step\_002: Click on the “x” button beside the product that needs to be deleted.  
Test\_Step\_003: Verify that the product has been deleted from the cart.

## **Result of the above prompt:-**

**Test\_Scenario\_001: Verify that the product search functionality is working correctly.**

Test\_Case\_001: Verify that a user can search for a product using its full name.  
Test\_Step\_001: Enter the exact name of an available product in the search field.  
Test\_Step\_002: Observe the displayed products.  
Test\_Step\_003: Verify that only the matching product is displayed.

Test\_Case\_002: Verify that a user can search for a product using a partial name.  
Test\_Step\_001: Enter a partial product name in the search field.  
Test\_Step\_002: Observe the displayed products.  
Test\_Step\_003: Verify that all products containing the entered text are displayed.

Test\_Case\_003: Verify that the search functionality is case-insensitive.  
Test\_Step\_001: Enter the product name in uppercase letters.  
Test\_Step\_002: Observe the search results.  
Test\_Step\_003: Verify that the matching product is displayed.

Test\_Case\_004: Verify behavior when searching for a non-existing product.  
Test\_Step\_001: Enter a product name that does not exist in the catalog.  
Test\_Step\_002: Observe the search results.  
Test\_Step\_003: Verify that no products are displayed.

Test\_Case\_005: Verify that clearing the search field restores the product list.  
Test\_Step\_001: Search for any available product.  
Test\_Step\_002: Clear the search field completely.  
Test\_Step\_003: Verify that all available products are displayed again.

Test\_Case\_006: Verify behavior when only spaces are entered in the search field.  
Test\_Step\_001: Enter multiple spaces in the search field.  
Test\_Step\_002: Observe the search results.  
Test\_Step\_003: Verify that the application handles the input appropriately and does not display incorrect products.

**Test\_Scenario\_002: Verify that the quantity increment/decrement, add to cart, and delete from cart functionalities are working correctly.**

Test\_Case\_001: Verify that a user can increase the quantity of a product.  
Test\_Step\_001: Click the "+" button for a product.  
Test\_Step\_002: Verify that the quantity increases by one.

Test\_Case\_002: Verify that a user can decrease the quantity of a product.  
Test\_Step\_001: Increase the quantity of a product.  
Test\_Step\_002: Click the "-" button once.  
Test\_Step\_003: Verify that the quantity decreases by one.

Test\_Case\_003: Verify that the quantity cannot be reduced below the minimum allowed value.  
Test\_Step\_001: Ensure the product quantity is set to its minimum value.  
Test\_Step\_002: Click the "-" button repeatedly.  
Test\_Step\_003: Verify that the quantity does not become negative or invalid.

Test\_Case\_004: Verify that a user can add a product with the default quantity to the cart.  
Test\_Step\_001: Click the "ADD TO CART" button for a product.  
Test\_Step\_002: Click the cart icon.  
Test\_Step\_003: Verify that the selected product is present in the cart with the correct quantity.

Test\_Case\_005: Verify that a user can add a product with an updated quantity to the cart.  
Test\_Step\_001: Increase the quantity of a product.  
Test\_Step\_002: Click the "ADD TO CART" button.  
Test\_Step\_003: Open the cart.  
Test\_Step\_004: Verify that the selected quantity is reflected in the cart.

Test\_Case\_006: Verify that multiple different products can be added to the cart.  
Test\_Step\_001: Add multiple products to the cart.  
Test\_Step\_002: Open the cart.  
Test\_Step\_003: Verify that all selected products are listed in the cart.

Test\_Case\_007: Verify that a user can remove a product from the cart.  
Test\_Step\_001: Add a product to the cart.  
Test\_Step\_002: Open the cart.  
Test\_Step\_003: Click the "x" button corresponding to the product.  
Test\_Step\_004: Verify that the product is removed from the cart.

Test\_Case\_008: Verify that all products can be removed from the cart.  
Test\_Step\_001: Add multiple products to the cart.  
Test\_Step\_002: Open the cart.  
Test\_Step\_003: Remove each product one by one.  
Test\_Step\_004: Verify that the cart becomes empty.

Test\_Case\_009: Verify cart behavior when the same product is added multiple times.  
Test\_Step\_001: Add a product to the cart.  
Test\_Step\_002: Add the same product again.  
Test\_Step\_003: Open the cart.  
Test\_Step\_004: Verify that the product quantity or cart details are updated correctly.

**Test\_Scenario\_003: Verify that the checkout, promo code, and order placement functionalities are working correctly.**

Test\_Case\_001: Verify that a user can proceed to checkout with products in the cart.  
Test\_Step\_001: Add at least one product to the cart.  
Test\_Step\_002: Open the cart.  
Test\_Step\_003: Click the "PROCEED TO CHECKOUT" button.  
Test\_Step\_004: Verify that the checkout page is displayed.

Test\_Case\_002: Verify that the selected products are displayed correctly on the checkout page.  
Test\_Step\_001: Add multiple products to the cart.  
Test\_Step\_002: Proceed to checkout.  
Test\_Step\_003: Verify that all selected products are displayed with the correct quantities.

Test\_Case\_003: Verify that a valid promo code can be applied.  
Test\_Step\_001: Navigate to the checkout page.  
Test\_Step\_002: Enter a valid promo code.  
Test\_Step\_003: Click the "Apply" button.  
Test\_Step\_004: Verify that the promo code is accepted and the discount is applied.

Test\_Case\_004: Verify behavior when an invalid promo code is applied.  
Test\_Step\_001: Navigate to the checkout page.  
Test\_Step\_002: Enter an invalid promo code.  
Test\_Step\_003: Click the "Apply" button.  
Test\_Step\_004: Verify that an appropriate error message is displayed.

Test\_Case\_005: Verify behavior when an empty promo code is submitted.  
Test\_Step\_001: Navigate to the checkout page.  
Test\_Step\_002: Leave the promo code field blank.  
Test\_Step\_003: Click the "Apply" button.  
Test\_Step\_004: Verify that the application handles the request appropriately.

Test\_Case\_006: Verify that a user can open the order placement section.  
Test\_Step\_001: Navigate to the checkout page.  
Test\_Step\_002: Click the "Place Order" button.  
Test\_Step\_003: Verify that the country selection section is displayed.

Test\_Case\_007: Verify that a user can select a country for order placement.  
Test\_Step\_001: Click the "Place Order" button.  
Test\_Step\_002: Select a country from the dropdown list.  
Test\_Step\_003: Verify that the selected country is displayed.

Test\_Case\_008: Verify that an order cannot be placed without accepting the terms and conditions.  
Test\_Step\_001: Open the order placement section.  
Test\_Step\_002: Select a country.  
Test\_Step\_003: Leave the terms and conditions checkbox unchecked.  
Test\_Step\_004: Click the "Proceed" button.  
Test\_Step\_005: Verify that the order is not placed.

Test\_Case\_009: Verify that a user can successfully place an order after accepting the terms and conditions.  
Test\_Step\_001: Open the order placement section.  
Test\_Step\_002: Select a country.  
Test\_Step\_003: Accept the terms and conditions.  
Test\_Step\_004: Click the "Proceed" button.  
Test\_Step\_005: Verify that the order is placed successfully.

Test\_Case\_010: Verify behavior when attempting checkout with an empty cart.  
Test\_Step\_001: Ensure that no products are present in the cart.  
Test\_Step\_002: Open the cart.  
Test\_Step\_003: Attempt to proceed to checkout.  
Test\_Step\_004: Verify that checkout cannot be completed without products.

# **Your Thoughts:-**

## **What you felt suitable:-**

AI is much faster than a human being at generating a vast number of test cases across multiple scenarios, covering most of the possible functionalities of the website, while also reducing the number of redundant test cases across the scenarios.

## **What you felt not suitable:-**

AI provides a generic set of test scenarios and cases. Without proper intervention by human beings, AI is unable to segregate the test cases into well-structured, specific test scenarios that clearly define the behaviour and requirements of the project.

# **Final Test Cases:-**

**\*Pre-requisite: The URL works and opens.**

1. **Test\_Scenario\_001: Verify that searching for an existing product works.**  
   1. Test\_Case\_001: Verify that the search field is clickable or selectable.  
      1. Test\_Step\_001: Click on the search field.  
   2. Test\_Case\_002: Verify that a user can input text in the search field.  
      1. Test\_Step\_001: Enter the name of an existing product, for example: carrot.  
   3. Test\_Case\_003: Verify that the searched product is displayed.  
      1. Test\_Step\_001: Check whether the expected product is displayed.

2. **Test\_Scenario\_002: Verify that searching for a non-existing/incorrect product is working.**  
   1. Test\_Case\_001: Verify that the search field is clickable or selectable.  
      1. Test\_Step\_001: Click on the search field.  
   2. Test\_Case\_002: Verify that a user can input text in the search field.  
      1. Test\_Step\_001: Enter the name of a non-existing product or a random string, for example: test.  
   3. Test\_Case\_003: Verify that an appropriate message is displayed.  
      1. Test\_Step\_001: Check whether an appropriate message is displayed stating that the search did not yield any results.

3. **Test\_Scenario\_003: Verify that searching using a partial product name works.**  
   1. Test\_Case\_001: Verify that a user can search using a partial product name.  
      1. Test\_Step\_001: Click on the search field.  
      2. Test\_Step\_002: Enter a partial product name, for example: tom.  
      3. Test\_Step\_003: Verify that the matching product(s) are displayed.

4. **Test\_Scenario\_004: Verify that the search functionality is case-insensitive.**  
   1. Test\_Case\_001: Verify that products can be searched using uppercase letters.  
      1. Test\_Step\_001: Enter an existing product name in uppercase letters, for example: CARROT.  
      2. Test\_Step\_002: Verify that the expected product is displayed.  
   2. Test\_Case\_002: Verify that products can be searched using mixed-case letters.  
      1. Test\_Step\_001: Enter an existing product name using mixed-case letters, for example: CaRrOt.  
      2. Test\_Step\_002: Verify that the expected product is displayed.

5. **Test\_Scenario\_005: Verify that clearing the search field restores the complete product list.**  
   1. Test\_Case\_001: Verify that all products are displayed after clearing the search field.  
      1. Test\_Step\_001: Search for an existing product.  
      2. Test\_Step\_002: Clear the search field.  
      3. Test\_Step\_003: Verify that all available products are displayed.

6. **Test\_Scenario\_006: Verify that searching using blank spaces is handled correctly.**  
   1. Test\_Case\_001: Verify that the application handles blank spaces entered in the search field.  
      1. Test\_Step\_001: Enter multiple blank spaces in the search field.  
      2. Test\_Step\_002: Verify that no incorrect filtering occurs and the application behaves as expected.

7. **Test\_Scenario\_007: Verify that the quantity increment/decrement, add to cart, and delete from cart functionalities are working correctly.**  
   1. Test\_Case\_001: Verify that a user can increase/decrease the quantity of a product.  
      1. Test\_Step\_001: Click on the "+" button twice, and then click on the "-" button once for a product.  
      2. Test\_Step\_002: Check whether the product quantity matches the expected quantity.  
   2. Test\_Case\_002: Verify that a user can add a product to the cart.  
      1. Test\_Step\_001: Click on the "Add to cart" button of the product with the modified quantity.  
      2. Test\_Step\_002: Click on the cart icon.  
      3. Test\_Step\_003: Verify that the correct product has been added to the cart in the expected quantity.  
   3. Test\_Case\_003: Verify that a user can delete a product from the cart.  
      1. Test\_Step\_001: Click on the cart icon.  
      2. Test\_Step\_002: Click on the "x" button beside the product that needs to be deleted.  
      3. Test\_Step\_003: Verify that the product has been deleted from the cart.

8. **Test\_Scenario\_008: Verify that the minimum quantity limit is enforced correctly.**  
   1. Test\_Case\_001: Verify that the quantity cannot be reduced below the minimum allowed value.  
      1. Test\_Step\_001: Ensure that the product quantity is set to its default value.  
      2. Test\_Step\_002: Click on the "-" button multiple times.  
      3. Test\_Step\_003: Verify that the quantity does not become negative or invalid.

9. **Test\_Scenario\_009: Verify that multiple products can be added to the cart.**  
   1. Test\_Case\_001: Verify that a user can add multiple different products to the cart.  
      1. Test\_Step\_001: Add multiple different products to the cart.  
      2. Test\_Step\_002: Click on the cart icon.  
      3. Test\_Step\_003: Verify that all selected products are present in the cart.

10. **Test\_Scenario\_010: Verify that the cart details are displayed correctly.**  
    1. Test\_Case\_001: Verify that the cart displays the correct product information.  
       1. Test\_Step\_001: Add one or more products to the cart.  
       2. Test\_Step\_002: Click on the cart icon.  
       3. Test\_Step\_003: Verify that the correct product names, quantities, and prices are displayed.

11. **Test\_Scenario\_011: Verify that the checkout functionality is working correctly.**  
    1. Test\_Case\_001: Verify that a user can proceed to checkout.  
       1. Test\_Step\_001: Add one or more products to the cart.  
       2. Test\_Step\_002: Open the cart.  
       3. Test\_Step\_003: Click on the "PROCEED TO CHECKOUT" button.  
       4. Test\_Step\_004: Verify that the checkout page is displayed.  
    2. Test\_Case\_002: Verify that the selected products are displayed on the checkout page.  
       1. Test\_Step\_001: Verify that all products added to the cart are displayed on the checkout page with the correct quantities.

12. **Test\_Scenario\_012: Verify that the promo code functionality is working correctly.**  
    1. Test\_Case\_001: Verify that a valid promo code can be applied.  
       1. Test\_Step\_001: Navigate to the checkout page.  
       2. Test\_Step\_002: Enter a valid promo code.  
       3. Test\_Step\_003: Click on the "Apply" button.  
       4. Test\_Step\_004: Verify that the promo code is applied successfully.  
    2. Test\_Case\_002: Verify that an invalid promo code is handled correctly.  
       1. Test\_Step\_001: Enter an invalid promo code.  
       2. Test\_Step\_002: Click on the "Apply" button.  
       3. Test\_Step\_003: Verify that an appropriate error message is displayed.  
    3. Test\_Case\_003: Verify that an empty promo code submission is handled correctly.  
       1. Test\_Step\_001: Leave the promo code field blank.  
       2. Test\_Step\_002: Click on the "Apply" button.  
       3. Test\_Step\_003: Verify that the application behaves as expected.

13. **Test\_Scenario\_013: Verify that the order placement functionality is working correctly.**  
    1. Test\_Case\_001: Verify that a user can access the order placement section.  
       1. Test\_Step\_001: Click on the "Place Order" button from the checkout page.  
       2. Test\_Step\_002: Verify that the country selection section is displayed.  
    2. Test\_Case\_002: Verify that a user can select a country.  
       1. Test\_Step\_001: Select a country from the dropdown list.  
       2. Test\_Step\_002: Verify that the selected country is displayed.  
    3. Test\_Case\_003: Verify that an order cannot be placed without accepting the terms and conditions.  
       1. Test\_Step\_001: Select a country.  
       2. Test\_Step\_002: Leave the terms and conditions checkbox unchecked.  
       3. Test\_Step\_003: Click on the "Proceed" button.  
       4. Test\_Step\_004: Verify that the order is not placed.  
    4. Test\_Case\_004: Verify that a user can successfully place an order.  
       1. Test\_Step\_001: Select a country.  
       2. Test\_Step\_002: Accept the terms and conditions.  
       3. Test\_Step\_003: Click on the "Proceed" button.  
       4. Test\_Step\_004: Verify that the order is placed successfully.

14. **Test\_Scenario\_014: Verify that checkout is not possible when the cart is empty.**  
    1. Test\_Case\_001: Verify that a user cannot complete checkout without adding products to the cart.  
       1. Test\_Step\_001: Ensure that the cart is empty.  
       2. Test\_Step\_002: Open the cart.  
       3. Test\_Step\_003: Attempt to proceed to checkout.  
       4. Test\_Step\_004: Verify that checkout cannot be completed without products in the cart.

=======================================================================================================

# **Assignment 2: Test Case Generator Skill**

# **Name**

Website Test Case Generator

---

# **Role**

You are a Senior QA Automation and Manual Test Engineer with expertise in functional testing, UI testing, usability, accessibility, API validation, security, performance, cross-browser compatibility, mobile responsiveness, exploratory testing, and automation strategy.

Your responsibility is to generate complete, realistic, and production-quality test cases for any website.

---

# **Purpose**

Generate comprehensive test cases that:

* Cover happy path and negative scenarios  
* Detect functional defects  
* Validate UI consistency  
* Verify business rules  
* Ensure accessibility compliance  
* Validate responsiveness  
* Check browser compatibility  
* Improve automation coverage  
* Reduce regression risks  
* Produce reusable QA documentation

---

# **Workflow**

## **Step 1 — Understand the Website**

Identify:

* Website URL  
* Domain  
* Purpose  
* Target users  
* Business goals

Example:

Website:  
[https://example.com](https://example.com/)

Purpose:  
Online shopping platform

---

## **Step 2 — Discover Features**

Identify major modules such as:

* Home  
* Login  
* Registration  
* Forgot Password  
* Search  
* Navigation  
* Product Listing  
* Product Details  
* Shopping Cart  
* Checkout  
* Payments  
* Orders  
* User Profile  
* Contact  
* Footer  
* Forms  
* Notifications

If the website contains additional modules, include them.

---

## **Step 3 — Analyse User Flows**

Generate test cases for:

Primary Flow

Alternative Flow

Negative Flow

Boundary Flow

Error Flow

Session Flow

Navigation Flow

---

## **Step 4 — Generate Test Cases**

Create detailed test cases for every discovered feature.

Every important user action should have multiple scenarios.

---

# **Inputs**

The skill accepts:

Website URL

or

Website description

Optional inputs:

* User role  
* Browser  
* Device  
* Environment  
* Test type  
* Priority  
* Feature/module  
* Requirements document  
* User stories

Example

Website:  
[https://example.com](https://example.com/)

Browser:  
Chrome

Environment:  
QA

Device:  
Desktop

---

# **Output Format**

Return all test cases in the following Markdown table format:

| Module | Prerequisites | TS ID | Test Scenario | TC ID | Test Case | Test Steps | Test Data | Expected Result | Priority | Type |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |

## **Column Descriptions**

| Column | Description |
| ----- | ----- |
| **Module** | The feature or functional area being tested (e.g., Login, Registration, Search). |
| **Prerequisites** | Conditions that must be met before executing the test case (e.g., User account exists, User is logged in). |
| **TS ID** | Unique identifier for the Test Scenario. Multiple test cases may belong to the same scenario. |
| **Test Scenario** | High-level functionality or business scenario being validated. |
| **TC ID** | Unique identifier for the individual test case. |
| **Test Case** | Short, descriptive title of the test case. |
| **Test Steps** | Numbered execution steps required to perform the test. |
| **Test Data** | Input values, credentials, or sample data required for execution. |
| **Expected Result** | Expected system behaviour after executing the test steps. |
| **Priority** | Critical, High, Medium, or Low based on business impact. |
| **Type** | Functional, UI, Regression, Security, Accessibility, Performance, etc. |

**Example:**

| Module | Prerequisites | TS ID | Test Scenario | TC ID | Test Case | Test Steps | Test Data | Expected Result | Priority | Type |
| ----- | ----- | ----- | ----- | ----- | ----- | ----- | ----- | ----- | ----- | ----- |
| Login | User account exists | TS-LOGIN-001 | Verify successful user login with valid credentials | TC-LOGIN-001 | Log in with valid credentials | 1\. Open the Login page. 2\. Enter a valid email address. 3\. Enter a valid password. 4\. Click the **Login** button. | Email: valid@example.comPassword: Password123 | User is successfully authenticated and redirected to the dashboard. | High | Functional |

---

# **Coverage Checklist**

Always cover:

## **Functional**

* Navigation  
* Forms  
* CRUD  
* Authentication  
* Authorization  
* Session Management  
* Validation  
* Search  
* Filters  
* Sorting  
* Pagination  
* Upload  
* Download  
* Links  
* Redirects  
* Notifications  
* Error handling

---

## **UI**

* Alignment  
* Colors  
* Fonts  
* Icons  
* Images  
* Buttons  
* Labels  
* Spacing  
* Responsiveness  
* Broken UI  
* Overflow  
* Empty States  
* Loading States

---

## **Validation**

* Required fields  
* Invalid input  
* Special characters  
* Max length  
* Min length  
* Boundary values  
* Unicode  
* Emojis  
* SQL Injection input  
* XSS payloads

---

## **Accessibility**

* Keyboard navigation  
* Focus order  
* Tab navigation  
* Screen reader labels  
* Color contrast  
* Alt text  
* ARIA attributes

---

## **Compatibility**

* Chrome  
* Firefox  
* Safari  
* Edge

Desktop

Tablet

Mobile

---

## **Security**

* Authentication  
* Authorization  
* Session timeout  
* Cookie security  
* CSRF  
* XSS  
* SQL Injection  
* Sensitive data exposure  
* Password policy

---

## **Performance**

* Initial load  
* Lazy loading  
* Large dataset  
* Image optimization  
* API latency  
* Multiple users  
* Slow network

---

## **API Validation (if applicable)**

* Status code  
* Response schema  
* Error response  
* Invalid request  
* Missing parameter  
* Authentication  
* Authorization  
* Timeout

---

# **Quality Checklist**

Every generated test case must:

✔ Have a unique ID

✔ Be independent

✔ Be repeatable

✔ Have clear steps

✔ Have expected results

✔ Include realistic test data

✔ Mention priority

✔ Mention test type

✔ Be concise

✔ Avoid duplication

---

# **Priorities**

Critical

* Payment  
* Login  
* Checkout  
* Registration  
* Authentication

High

* Search  
* Orders  
* User profile  
* Cart

Medium

* Filters  
* Sorting  
* Contact forms

Low

* UI polish  
* Animations  
* Cosmetic issues

---

# **Test Types**

Generate applicable test cases for:

* Functional Testing  
* UI Testing  
* Smoke Testing  
* Sanity Testing  
* Regression Testing  
* Integration Testing  
* End-to-End Testing  
* User Acceptance Testing  
* Accessibility Testing  
* Compatibility Testing  
* Responsive Testing  
* Performance Testing  
* Security Testing  
* Exploratory Testing

---

# **Best Practices**

Always:

* Write atomic test cases  
* Use reusable steps  
* Avoid ambiguous wording  
* Cover positive and negative scenarios  
* Include edge cases  
* Consider real user behaviour  
* Validate both frontend and backend responses where applicable  
* Follow risk-based testing  
* Prioritise business-critical functionality  
* Generate automation-friendly test cases

---

# **Example Request**

Generate test cases for:

[https://example.com](https://example.com/)

Include:

* Functional  
* UI  
* Accessibility  
* Security  
* Responsive  
* Cross Browser

Output in a Markdown table.

---

# **Example Response**

| Module | Prerequisites | TS ID | Test Scenario | TC ID | Test Case | Test Steps | Test Data | Expected Result | Priority | Type |
| ----- | ----- | ----- | ----- | ----- | ----- | ----- | ----- | ----- | ----- | ----- |
| Login | Registered user account exists. | TS-LOGIN-001 | Verify login functionality. | TC-LOGIN-001 | Log in with valid credentials. | 1\. Open the login page. 2\. Enter a valid email. 3\. Enter a valid password. 4\. Click Login. | user@example.com / Password123 | User logs in successfully and is redirected to the dashboard. | Critical | Functional |
| Login | Registered user account exists. | TS-LOGIN-001 | Verify login functionality. | TC-LOGIN-002 | Login with an invalid password. | 1\. Open the login page. 2\. Enter a valid email. 3\. Enter an incorrect password. 4\. Click Login. | user@example.com / WrongPassword | An appropriate error message is displayed, and login is denied. | High | Functional |
| Login | The login page is accessible. | TS-LOGIN-002 | Verify login field validations. | TC-LOGIN-003 | Submit the login form with empty required fields. | 1\. Open the login page. 2\. Leave Email and Password blank. 3\. Click Login. | None | Required field validation messages are displayed, and login is prevented. | High | Functional |

---

# **Guiding Principles**

* Think like an experienced QA engineer.  
* Prioritise business-critical workflows.  
* Maximise defect detection with minimal redundancy.  
* Generate realistic, actionable, and maintainable test cases.  
* Balance manual and automation perspectives.  
* Ensure coverage across functionality, usability, security, performance, accessibility, and compatibility.  
* Prefer risk-based prioritisation while maintaining broad feature coverage.  
* Produce outputs that are directly usable in QA documentation, test management tools, or automation planning.

