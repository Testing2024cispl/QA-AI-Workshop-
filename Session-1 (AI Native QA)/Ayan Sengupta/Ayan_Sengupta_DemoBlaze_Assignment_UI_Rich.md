<div align="center">

# 🧪 QA AI Workshop — Assignment Template

## 🛒 DemoBlaze E2E Purchase Flow

**Manual Thinking + AI Generated + Final Automation-Ready Test Case**

</div>

---

## 📌 Assignment Snapshot

| 🧾 Field | ✅ Details |
|---|---|
| **Member Name** | **Ayan Sengupta** |
| **Assigned Website** | [https://www.demoblaze.com/](https://www.demoblaze.com/) |
| **Flow Type** | **Complete Product Purchase E2E Flow** |
| **Submission Type** | **Manual + AI + Final Automation-Ready Test Case** |
| **Primary User Journey** | Sign Up → Login → Product Selection → Add to Cart → Checkout → Purchase Confirmation → Logout |
| **Automation Stack** | Java + Selenium WebDriver + TestNG + Cucumber |

---

## 🧭 Table of Contents

- [QA Manual Test Cases](#-qa-manual-test-cases)
- [Human Thinking Test Cases](#-human-thinking-test-cases)
- [AI Manual Test Cases](#-ai-manual-test-cases)
- [Your Thoughts](#-your-thoughts)
- [Final Test Case](#-final-test-case)
- [Automation Framework and Tech Stack](#-automation-framework-and-tech-stack)
- [Final Automation-Ready Test Cases](#-final-automation-ready-test-cases)
- [Final E2E Automation Flow Summary](#-final-e2e-automation-flow-summary)
- [Automation Priority](#-automation-priority)

---

# ✅ QA Manual Test Cases

**Member 1:** Ayan Sengupta  
**Query/Test Cases:** DemoBlaze — Complete Product Purchase E2E Flow  
**Website:** [https://www.demoblaze.com/](https://www.demoblaze.com/)

---

# 🧠 Human Thinking Test Cases

> Manual test cases prepared by understanding the visible DemoBlaze UI, modal behavior, cart flow, checkout form, and purchase confirmation behavior.

---

## 🟦 Sign Up Flow

| Test Case ID | Type | Scenario | Test Steps | Expected Result |
|---|---|---|---|---|
| **TestCases_001** | 🟢 Positive | Verify successful sign up with valid username and password | 1. Go to [https://www.demoblaze.com/](https://www.demoblaze.com/) <br> 2. Click on **Sign up** from the header. <br> 3. Verify Sign up modal is displayed. <br> 4. Enter a new valid username. <br> 5. Enter a valid password. <br> 6. Click **Sign up**. <br> 7. Verify success alert. <br> 8. Accept/close the alert. | User should be registered successfully and success alert should be displayed. |
| **TestCases_002** | 🔴 Negative | Verify sign up validation with blank username and blank password | 1. Go to website. <br> 2. Click **Sign up**. <br> 3. Verify modal is displayed. <br> 4. Enter blank username/spaces. <br> 5. Enter blank password/spaces. <br> 6. Click **Sign up**. | Error alert/toast/inline validation should appear and user should not be registered. |
| **TestCases_003** | 🔴 Negative | Verify sign up validation with blank username and valid password | 1. Open Sign up modal. <br> 2. Keep username blank/space. <br> 3. Enter valid password. <br> 4. Click **Sign up**. | System should prevent registration and display validation message. |
| **TestCases_004** | 🔴 Negative | Verify sign up validation with valid username and blank password | 1. Open Sign up modal. <br> 2. Enter valid username. <br> 3. Keep password blank. <br> 4. Click **Sign up**. | System should prevent registration and display validation message. |
| **TestCases_005** | 🔴 Negative | Verify sign up with already registered username | 1. Open Sign up modal. <br> 2. Enter already registered username. <br> 3. Enter password. <br> 4. Click **Sign up**. | System should show duplicate user validation message. |

---

## 🟪 Login Flow

| Test Case ID | Type | Scenario | Test Steps | Expected Result |
|---|---|---|---|---|
| **TestCases_006** | 🟢 Positive | Verify successful login with registered username and password | 1. Go to website. <br> 2. Click **Log in** from header. <br> 3. Verify login modal is displayed. <br> 4. Enter registered username. <br> 5. Enter registered password. <br> 6. Click **Log in**. <br> 7. Verify user is logged in. | Welcome username/email should appear in header. |
| **TestCases_007** | 🔴 Negative | Verify login with blank username and blank password | 1. Open Login modal. <br> 2. Keep username blank/spaces. <br> 3. Keep password blank/spaces. <br> 4. Click **Log in**. | Validation alert/message should appear and login should fail. |
| **TestCases_008** | 🔴 Negative | Verify login with blank username and valid password | 1. Open Login modal. <br> 2. Keep username blank/spaces. <br> 3. Enter valid password. <br> 4. Click **Log in**. | Validation alert/message should appear and login should fail. |
| **TestCases_009** | 🔴 Negative | Verify login with valid username and blank password | 1. Open Login modal. <br> 2. Enter valid username. <br> 3. Keep password blank. <br> 4. Click **Log in**. | Validation alert/message should appear and login should fail. |
| **TestCases_010** | 🔴 Negative | Verify login with valid username and invalid password | 1. Open Login modal. <br> 2. Enter registered username. <br> 3. Enter invalid password. <br> 4. Click **Log in**. | Error message should appear and user should not be logged in. |
| **TestCases_011** | 🔴 Negative | Verify login with invalid username and valid password | 1. Open Login modal. <br> 2. Enter invalid/non-registered username. <br> 3. Enter valid password. <br> 4. Click **Log in**. | Error message should appear and login should fail. |
| **TestCases_012** | 🔴 Negative | Verify login with invalid username and invalid password | 1. Open Login modal. <br> 2. Enter invalid username. <br> 3. Enter invalid password. <br> 4. Click **Log in**. | Error message should appear and login should fail. |

---

## 🟨 Cross Browser Testing

| Test Case ID | Type | Scenario | Test Steps | Expected Result |
|---|---|---|---|---|
| **TestCases_013** | 🧩 Compatibility | Verify website opens and runs properly in different browsers | 1. Open Chrome, Firefox, and Edge. <br> 2. Navigate to DemoBlaze. <br> 3. Run the major E2E flow in each browser. | Website UI and core purchase flow should work without major functional or UI breakage. |

---

## 🟩 Add to Cart Flow

| Test Case ID | Type | Scenario | Test Steps | Expected Result |
|---|---|---|---|---|
| **TestCases_014** | 🟢 Positive | Verify user can add product to cart | 1. Go to DemoBlaze. <br> 2. Click a product from product list. <br> 3. Verify product details page opens. <br> 4. Verify **Add to cart** button. <br> 5. Click **Add to cart**. <br> 6. Verify success alert. <br> 7. Navigate to cart. | Product should be added and visible in cart with correct title and price. |
| **TestCases_015** | 🔴 Negative / Observation | Verify out-of-stock product handling, if inventory feature exists | 1. Try to identify out-of-stock product. <br> 2. Attempt to add it to cart. | System should prevent adding out-of-stock product if stock validation exists. |
| **TestCases_016** | 🔴 Negative / Observation | Verify quantity greater than available stock, if quantity feature exists | 1. Open product details. <br> 2. Try to add quantity greater than stock, if quantity field exists. | System should prevent adding quantity greater than available stock if inventory validation exists. |

---

## 🟥 Checkout Flow

| Test Case ID | Type | Scenario | Test Steps | Expected Result |
|---|---|---|---|---|
| **TestCases_017** | 🟢 Positive | Verify user can checkout with product added to cart | 1. Add product to cart. <br> 2. Open cart. <br> 3. Verify product name and price. <br> 4. Click **Place Order**. <br> 5. Fill order details. <br> 6. Click **Purchase**. | Purchase should be completed and confirmation popup should appear. |
| **TestCases_018** | 🟢 Positive | Verify order confirmation details after checkout | 1. Complete purchase with valid data. <br> 2. Verify thank you message. <br> 3. Verify order ID, amount, card number, name, and date. | Correct purchase confirmation details should be displayed. |
| **TestCases_019** | 🔴 Negative | Verify system prevents purchase without billing details | 1. Add product to cart. <br> 2. Click **Place Order**. <br> 3. Keep billing/order details blank. <br> 4. Click **Purchase**. | System should prevent purchase or show validation message. |
| **TestCases_020** | 🔴 Negative / Observation | Verify invalid card details behavior | 1. Fill order form. <br> 2. Enter invalid card details. <br> 3. Click **Purchase**. | System should reject invalid card details if validation is implemented. |
| **TestCases_021** | 🔴 Negative / Observation | Verify payment failure behavior | 1. Fill order form. <br> 2. Use payment data expected to fail. <br> 3. Click **Purchase**. | System should show payment failure message if payment validation is implemented. |

---

# 🤖 AI Manual Test Cases

> **Prompt Used:**  
> See the screenshots, analyze and understand the feature and flow of DemoBlaze. Write manual functional test cases for DemoBlaze complete E2E purchase flow where a user logs in, selects a product, adds it to the cart, places an order, and verifies successful purchase confirmation. Output should be in table format. Both positive and negative test cases should be included.

## 🧾 DemoBlaze Complete E2E Purchase Flow — AI Generated Manual Functional Test Cases

| Test Case ID | Test Type | Test Scenario | Pre-Condition | Test Steps | Test Data | Expected Result |
|---|---|---|---|---|---|---|
| **TestCases_001** | 🟢 Positive | Verify successful login with valid credentials | User should have valid DemoBlaze account | 1. Go to website. <br> 2. Click **Log in**. <br> 3. Enter valid username. <br> 4. Enter valid password. <br> 5. Click **Log in**. | Username: valid user <br> Password: valid password | User should be logged in and welcome username should be displayed. |
| **TestCases_002** | 🔴 Negative | Verify login validation with blank username and password | User should be on login modal | 1. Open Login modal. <br> 2. Keep username blank. <br> 3. Keep password blank. <br> 4. Click **Log in**. | Username: Blank <br> Password: Blank | Validation message should appear and login should fail. |
| **TestCases_003** | 🔴 Negative | Verify login with invalid username and valid password | User should be on login modal | 1. Enter invalid username. <br> 2. Enter valid password. <br> 3. Click **Log in**. | Username: invaliduser@yopmail.com <br> Password: valid password | User should not be logged in. |
| **TestCases_004** | 🔴 Negative | Verify login with valid username and wrong password | Registered username should exist | 1. Enter valid username. <br> 2. Enter wrong password. <br> 3. Click **Log in**. | Username: valid user <br> Password: wrong password | Login should fail with proper error message. |
| **TestCases_005** | 🟢 Positive | Verify product categories and listing | User should be logged in | 1. Go to homepage. <br> 2. Verify categories. <br> 3. Click **Phones**. <br> 4. Verify product list. | Category: Phones | Products should be displayed based on selected category. |
| **TestCases_006** | 🟢 Positive | Verify product details page | Product should be visible | 1. Click **Samsung galaxy s6**. <br> 2. Verify product image, name, price, and description. | Product: Samsung galaxy s6 | Product details should be displayed correctly. |
| **TestCases_007** | 🟢 Positive | Verify add to cart functionality | User should be on product details page | 1. Click **Add to cart**. <br> 2. Verify product added alert. <br> 3. Accept alert. | Product: Samsung galaxy s6 | Product should be added successfully. |
| **TestCases_008** | 🟢 Positive | Verify product on cart page | Product should be added to cart | 1. Click **Cart**. <br> 2. Verify product image, title, and price. | Product: Samsung galaxy s6 <br> Price: 360 | Added product should be visible in cart. |
| **TestCases_009** | 🟢 Positive | Verify cart total amount | Product should be in cart | 1. Open cart. <br> 2. Check product price. <br> 3. Check total amount. | Product Price: 360 | Total should match product price. |
| **TestCases_010** | 🟢 Positive | Verify Place Order modal opens | Product should be in cart | 1. Click **Place Order**. <br> 2. Verify modal fields. | Total: 360 | Place Order modal should open with all fields. |
| **TestCases_011** | 🟢 Positive | Verify successful purchase with valid order details | Place Order modal should be open | 1. Enter name, country, city, card, month, year. <br> 2. Click **Purchase**. | Name: Bikas Pal <br> Country: India <br> City: Kolkata <br> Card: 646444646 <br> Month: 12 <br> Year: 2026 | Purchase confirmation popup should appear. |
| **TestCases_012** | 🟢 Positive | Verify purchase confirmation details | Purchase should be completed | 1. Verify confirmation popup. <br> 2. Verify ID, amount, card, name, and date. | Amount: 360 USD | Confirmation popup should contain purchase details. |
| **TestCases_013** | 🟢 Positive | Verify OK button on confirmation popup | Confirmation popup should be displayed | 1. Click **OK**. | Action: OK | Popup should close successfully. |
| **TestCases_014** | 🔴 Negative | Verify blank Name validation | Place Order modal should be open | 1. Keep name blank. <br> 2. Fill other details. <br> 3. Click **Purchase**. | Name: Blank | Purchase should not complete if validation is implemented. |
| **TestCases_015** | 🔴 Negative | Verify blank Credit Card validation | Place Order modal should be open | 1. Fill name/country/city/month/year. <br> 2. Keep card blank. <br> 3. Click **Purchase**. | Credit Card: Blank | Purchase should not complete if validation is implemented. |
| **TestCases_016** | 🔴 Negative | Verify all order fields blank | Place Order modal should be open | 1. Keep all fields blank. <br> 2. Click **Purchase**. | All fields blank | Validation message should appear. |
| **TestCases_017** | 🔴 Negative | Verify invalid card value | Place Order modal should be open | 1. Enter invalid card value. <br> 2. Click **Purchase**. | Card: abcd@123 | Invalid card should be rejected if validation is implemented. |
| **TestCases_018** | 🟢 Positive | Verify product delete from cart | Product should be in cart | 1. Open cart. <br> 2. Click **Delete**. <br> 3. Verify product removed. | Product: Samsung galaxy s6 | Product should be removed from cart. |
| **TestCases_019** | 🔴 Negative | Verify Place Order with empty cart | Cart should be empty | 1. Open cart. <br> 2. Try Place Order if available. | Cart: Empty | System should not allow valid purchase with empty cart. |
| **TestCases_020** | 🟢 Positive | Verify logout after purchase flow | User should be logged in | 1. Complete/stay in flow. <br> 2. Click **Log out**. | Action: Logout | User should be logged out successfully. |

---

# 💭 Your Thoughts

## ✅ What you felt Suitable — Where AI outperformed human thinking

| Area | Observation |
|---|---|
| **Structure** | AI organized the test cases in a clean table format with Test Case ID, Type, Scenario, Pre-Condition, Test Steps, Test Data, and Expected Result. |
| **Readability** | AI made the test cases easier to review and more suitable for documentation. |
| **Automation Readiness** | AI added clear expected results and test data, making the cases easier to convert into automation scripts. |
| **E2E Coverage** | AI covered login, product listing, product details, add to cart, cart validation, checkout, confirmation popup, delete from cart, and logout. |
| **Confirmation Validation** | AI added strong validation points for confirmation message, order ID, amount, card number, customer name, and date. |

## ⚠️ What you felt Not suitable — Where AI made mistakes or missed

| Area | Observation |
|---|---|
| **Missed Sign Up Flow** | AI did not include the Sign Up flow, even though it is important for a new user journey. |
| **Missed Wider QA Coverage** | AI missed cross-browser testing, out-of-stock scenarios, inventory quantity validation, and payment failure thoughts from the human test cases. |
| **Assumptions** | AI assumed all Place Order fields have strict validation, which must be manually verified against actual DemoBlaze behavior. |
| **Website-Specific Limitations** | Some human ideas like password eye icon, stock quantity, CVV, and real payment failure may not exist in DemoBlaze, so these should be treated carefully as observations/theoretical cases. |
| **Final Improvement Needed** | Final test cases should combine AI’s structured format with human edge-case thinking and actual DemoBlaze UI behavior. |

---

# 🧩 Final Test Case

> AI + Manual thinking combined into a polished, automation-ready DemoBlaze E2E test design.

---

# ⚙️ Automation Framework and Tech Stack

| Area | Technology / Approach |
|---|---|
| **Programming Language** | Java |
| **Automation Tool** | Selenium WebDriver |
| **Test Runner** | TestNG |
| **BDD Framework** | Cucumber |
| **Cucumber-TestNG Integration** | `AbstractTestNGCucumberTests` |
| **Test Data Handling** | TestNG `DataProvider` and `.properties` files |
| **Configuration Handling** | `.properties` files |
| **Test Execution Style** | Cucumber Feature Files + Step Definitions + TestNG Runner |
| **Validation Approach** | Assertions and UI verification through Selenium |
| **Reporting** | TestNG/Cucumber execution report |

## 🧱 Framework Approach

1. Cucumber Feature Files will define the DemoBlaze E2E purchase flow in readable BDD format.
2. Step Definition classes will contain the implementation of `Given`, `When`, `Then`, and `And` steps.
3. The Test Runner class will extend `AbstractTestNGCucumberTests` to execute Cucumber scenarios with TestNG.
4. Test data such as username, password, customer name, country, city, card number, month, year, product name, and expected messages will be handled using TestNG `DataProvider` and `.properties` files.
5. Common configuration values such as browser name, application URL, timeout values, and environment details will be stored in `.properties` files.
6. Selenium WebDriver will interact with DemoBlaze UI elements such as Sign up modal, Login modal, product cards, Add to cart button, Cart page, Place Order modal, and Purchase confirmation popup.
7. Assertions will verify successful login, product details, cart details, total amount, order confirmation message, order ID, amount, card number, customer name, and date.
8. The flow will be reusable and maintainable so positive and negative scenarios can be executed with multiple data sets.

---

# 🚀 Final Automation-Ready Test Cases

## 🧾 Summary-Level Automation Coverage

| TC ID | Test Scenario | Preconditions | Test Steps | Test Data | Expected Result | Priority |
|---|---|---|---|---|---|---|
| **TC_001** | User Sign Up with Valid Data | User is on DemoBlaze homepage | Click Sign Up → Enter username/password → Click Sign Up | Username, Password | User account is created and success alert is displayed | 🟡 Medium |
| **TC_002** | Login with Valid Credentials | Registered user exists | Click Login → Enter username/password → Click Login | Username, Password | User is logged in and username appears in header | 🔴 High |
| **TC_003** | Login with Blank Credentials | User is on Login modal | Click Login without entering data | Blank Username, Blank Password | Validation message or login failure is displayed | 🟡 Medium |
| **TC_004** | Verify Product Details Page | User is logged in | Select category → Click product | Product Name | Product image, name, price, and description are displayed | 🔴 High |
| **TC_005** | Add Product to Cart | User is on Product Details page | Click Add to Cart | Product Name | Product added alert is displayed | 🔴 High |
| **TC_006** | Verify Product in Cart | Product added to cart | Navigate to Cart page | Product Name | Product name and price match selected product | 🔴 High |
| **TC_007** | Verify Cart Total Amount | Product exists in cart | Open Cart page | Product Price | Total amount equals product price | 🔴 High |
| **TC_008** | Delete Product from Cart | Product exists in cart | Click Delete | Product Name | Product is removed from cart | 🟡 Medium |
| **TC_009** | Open Place Order Modal | Product exists in cart | Click Place Order | N/A | Place Order modal is displayed | 🔴 High |
| **TC_010** | Verify Place Order Modal Close Functionality | Place Order modal is open | Click Close and X icon | N/A | Modal closes successfully | 🟡 Medium |
| **TC_011** | Complete Purchase with Valid Data | Product exists in cart | Fill order details → Click Purchase | Name, Country, City, Card, Month, Year | Purchase confirmation popup appears | 🔴 High |
| **TC_012** | Verify Purchase Confirmation Details | Purchase completed | Capture confirmation details | Order Details | Order ID, Amount, Card Number, Name, and Date are displayed | 🔴 High |
| **TC_013** | Purchase with Mandatory Fields Blank | Place Order modal is open | Leave fields blank → Click Purchase | Blank Data | Validation/purchase failure behavior is displayed | 🟡 Medium |
| **TC_014** | Logout Successfully | User is logged in | Click Logout | N/A | User is logged out and Login option appears | 🔴 High |

---

## 📋 Detailed Final Automation-Ready Test Cases

| Test Case ID | Test Type | Module / Flow | Test Scenario | Pre-Condition | Test Steps | Test Data | Expected Result |
|---|---|---|---|---|---|---|---|
| **TestCases_001** | 🟢 Positive | Sign Up Flow | Verify successful sign up with valid username and password | Website should be accessible and username should be new | 1. Go to website. <br> 2. Click **Sign up**. <br> 3. Verify Sign up modal. <br> 4. Enter new username. <br> 5. Enter valid password. <br> 6. Click **Sign up**. <br> 7. Verify success alert. <br> 8. Accept alert. | Username: New unique username <br> Password: Valid password | User should be registered successfully. |
| **TestCases_002** | 🔴 Negative | Sign Up Flow | Verify sign up validation with blank username and blank password | Website should be accessible | 1. Open Sign up modal. <br> 2. Keep username blank. <br> 3. Keep password blank. <br> 4. Click **Sign up**. <br> 5. Verify alert/message. | Username: Blank <br> Password: Blank | Registration should not be completed. |
| **TestCases_003** | 🔴 Negative | Sign Up Flow | Verify duplicate username validation | User should already exist | 1. Open Sign up modal. <br> 2. Enter existing username. <br> 3. Enter password. <br> 4. Click **Sign up**. <br> 5. Verify duplicate alert/message. | Existing username <br> Valid password | Duplicate registration should be prevented. |
| **TestCases_004** | 🟢 Positive | Login Flow | Verify successful login with valid credentials | Registered account should exist | 1. Open Login modal. <br> 2. Enter valid username. <br> 3. Enter valid password. <br> 4. Click **Log in**. <br> 5. Verify header username. | Valid username <br> Valid password | User should login successfully. |
| **TestCases_005** | 🔴 Negative | Login Flow | Verify login validation with blank credentials | Website should be accessible | 1. Open Login modal. <br> 2. Keep username/password blank. <br> 3. Click **Log in**. | Blank username <br> Blank password | Login should fail with validation message. |
| **TestCases_006** | 🔴 Negative | Login Flow | Verify login with valid username and invalid password | Valid username should exist | 1. Open Login modal. <br> 2. Enter valid username. <br> 3. Enter invalid password. <br> 4. Click **Log in**. | Valid username <br> Invalid password | Login should fail. |
| **TestCases_007** | 🔴 Negative | Login Flow | Verify login with invalid username and valid password | Website should be accessible | 1. Open Login modal. <br> 2. Enter invalid username. <br> 3. Enter password. <br> 4. Click **Log in**. | Invalid username <br> Valid password | Login should fail. |
| **TestCases_008** | 🟢 Positive | Product Listing Flow | Verify product categories on homepage | User should be on homepage | 1. Open DemoBlaze. <br> 2. Verify Phones, Laptops, Monitors categories. | Categories | Categories should be displayed. |
| **TestCases_009** | 🟢 Positive | Product Listing Flow | Verify products after selecting category | Homepage should be loaded | 1. Click **Phones** category. <br> 2. Verify phone products displayed. | Category: Phones | Phone products should display. |
| **TestCases_010** | 🟢 Positive | Product Details Flow | Verify product details page | Product should be visible | 1. Click **Samsung galaxy s6**. <br> 2. Verify image, name, price, description. | Product: Samsung galaxy s6 | Product details should display correctly. |
| **TestCases_011** | 🟢 Positive | Add to Cart Flow | Verify product added to cart | Product details page should be open | 1. Click **Add to cart**. <br> 2. Verify “Product added.” alert. <br> 3. Accept alert. | Product: Samsung galaxy s6 | Product should be added successfully. |
| **TestCases_012** | 🟢 Positive | Cart Flow | Verify added product on cart page | Product should be added to cart | 1. Click **Cart**. <br> 2. Verify product image, title, and price. | Product: Samsung galaxy s6 <br> Price: 360 | Product should display in cart. |
| **TestCases_013** | 🟢 Positive | Cart Flow | Verify total amount | Product should be in cart | 1. Capture product price. <br> 2. Capture total amount. <br> 3. Compare values. | Product Price: 360 | Total should match product price. |
| **TestCases_014** | 🟢 Positive | Cart Flow | Verify product delete functionality | Product should be in cart | 1. Click **Delete**. <br> 2. Verify product removed. <br> 3. Verify total updated/cleared. | Product: Samsung galaxy s6 | Product should be removed. |
| **TestCases_015** | 🟢 Positive | Checkout Flow | Verify Place Order modal opens | Product should be in cart | 1. Click **Place Order**. <br> 2. Verify fields: Total, Name, Country, City, Credit card, Month, Year. | Total: 360 | Modal should open with order fields. |
| **TestCases_016** | 🟢 Positive | Checkout Flow | Verify successful purchase | Place Order modal should be open | 1. Enter valid order details. <br> 2. Click **Purchase**. | Name: Bikas Pal <br> Country: India <br> City: Kolkata <br> Card: 646444646 <br> Month: 12 <br> Year: 2026 | Purchase confirmation should appear. |
| **TestCases_017** | 🟢 Positive | Purchase Confirmation Flow | Verify confirmation details | Purchase should be completed | 1. Verify thank you message. <br> 2. Verify order ID, amount, card number, name, date. | Amount: 360 USD <br> Name: Bikas Pal | Confirmation details should be displayed. |
| **TestCases_018** | 🟢 Positive | Purchase Confirmation Flow | Verify OK button | Confirmation popup should be visible | 1. Click **OK**. <br> 2. Verify popup closes. | Action: OK | Popup should close. |
| **TestCases_019** | 🔴 Negative | Checkout Flow | Verify purchase with all fields blank | Place Order modal should be open | 1. Keep all fields blank. <br> 2. Click **Purchase**. <br> 3. Verify behavior. | All fields blank | Purchase should not complete if validation exists. |
| **TestCases_020** | 🔴 Negative | Checkout Flow | Verify purchase with blank Name | Place Order modal should be open | 1. Keep Name blank. <br> 2. Fill other fields. <br> 3. Click **Purchase**. | Name: Blank | Validation should appear if implemented. |
| **TestCases_021** | 🔴 Negative | Checkout Flow | Verify purchase with blank Credit Card | Place Order modal should be open | 1. Keep Credit card blank. <br> 2. Fill other fields. <br> 3. Click **Purchase**. | Credit Card: Blank | Validation should appear if implemented. |
| **TestCases_022** | 🔴 Negative | Checkout Flow | Verify invalid credit card behavior | Place Order modal should be open | 1. Enter invalid card value. <br> 2. Click **Purchase**. | Card: abcd@123 | Invalid card should be rejected if validation exists. |
| **TestCases_023** | 🔴 Negative | Checkout Flow | Verify blank Country field | Place Order modal should be open | 1. Keep Country blank. <br> 2. Fill remaining fields. <br> 3. Click **Purchase**. | Country: Blank | Validation should appear if implemented. |
| **TestCases_024** | 🔴 Negative | Checkout Flow | Verify blank City field | Place Order modal should be open | 1. Keep City blank. <br> 2. Fill remaining fields. <br> 3. Click **Purchase**. | City: Blank | Validation should appear if implemented. |
| **TestCases_025** | 🔴 Negative | Checkout Flow | Verify blank Month and Year | Place Order modal should be open | 1. Keep Month and Year blank. <br> 2. Click **Purchase**. | Month: Blank <br> Year: Blank | Validation should appear if implemented. |
| **TestCases_026** | 🟢 Positive | Checkout Modal Flow | Verify Close button functionality | Place Order modal should be open | 1. Click **Close**. | Action: Close | Modal should close. |
| **TestCases_027** | 🟢 Positive | Checkout Modal Flow | Verify X icon functionality | Place Order modal should be open | 1. Click **X** icon. | Action: X icon | Modal should close. |
| **TestCases_028** | 🔴 Negative | Cart / Checkout Flow | Verify Place Order with empty cart | Cart should be empty | 1. Open empty cart. <br> 2. Try Place Order if available. | Cart: Empty | Valid purchase should not be allowed. |
| **TestCases_029** | 🟢 Positive | Logout Flow | Verify logout | User should be logged in | 1. Click **Log out**. <br> 2. Verify Login/Sign up shown. | Action: Logout | User should logout successfully. |
| **TestCases_030** | 🧩 Compatibility | Cross Browser Testing | Verify E2E flow across browsers | Browsers should be installed | 1. Execute flow in Chrome. <br> 2. Execute flow in Firefox. <br> 3. Execute flow in Edge. | Chrome, Firefox, Edge | Flow should work across browsers. |

---

# 🧭 Final E2E Automation Flow Summary

```text
Launch Browser
   ↓
Read URL / Browser from .properties
   ↓
Open DemoBlaze Website
   ↓
Sign Up / Login
   ↓
Verify Logged-in User
   ↓
Select Category
   ↓
Open Product Details
   ↓
Add Product to Cart
   ↓
Verify Cart Product + Total
   ↓
Place Order
   ↓
Fill Order Data from DataProvider / .properties
   ↓
Purchase
   ↓
Verify Confirmation Popup
   ↓
Logout
```

---

# 🎯 Automation Priority

| Priority | Scenarios |
|---|---|
| 🔴 **High Priority** | Login with valid credentials, Product details verification, Add to cart, Cart validation, Place order, Purchase confirmation validation, Logout |
| 🟡 **Medium Priority** | Sign up validation, Blank login validation, Blank checkout field validation, Cart delete functionality, Place Order modal Close/X functionality |
| 🟢 **Low Priority** | Cross browser testing, Empty cart checkout behavior, Invalid credit card behavior depending on actual DemoBlaze validation support |

---

<div align="center">

## ✅ End of Assignment

**Prepared By:** Ayan Sengupta  
**Website:** [DemoBlaze](https://www.demoblaze.com/)  
**Flow:** Complete Product Purchase E2E Flow

</div>
