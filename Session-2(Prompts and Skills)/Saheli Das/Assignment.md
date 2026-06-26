# AI + Manual Test Case Document #
## Grocery Store Demo ##
### Member :- Saheli Das
### Website: https://grocerystoredemo.pcubeweb.com/
### Format: For each test scenario below — 
QA Manual Test Cases (as written by hand), AI Manual Test Cases (generated from a prompt), Your thoughts on comparing the two, and a Final Test Case combining both into an automation-ready scenario.

## TestCases_001 — Account Verification & Creation ##

### QA Manual Test Cases:-
Member :- Saheli Das
#### Query/Test cases:- Grocery Store Demo (Human Thinking Test Cases)

Go to website: grocerystoredemo.pcubeweb.com ;
Click on Account;
Open Sign IN modal;
Enter your wrong Phone Number;
Click on Send OTP;
Check the validation message;
Enter your Correct Phone Number;
Click on Send OTP;
Display OTP Verification modal;
Check your phone number to get OTP for login;
Enter OTP within given time;
Verify the OTP;
Navigate to the Grocery Store Account page after Verification OTP

### AI Manual Test Cases:-
Member :- Saheli Das

#### Prompt:- Write test cases for Grocery Store Demo login using mobile number and OTP
Go to https://grocerystoredemo.pcubeweb.com/ ;
Click on Account ;
Enter a valid registered mobile number ;
Click on Send OTP ;
Enter the valid OTP received within the time limit;
Click on Verify;
Verify that the user is logged in successfully;
Verify that the user is redirected to the Account page;

## Your thoughts:-
### What you felt Suitable:- 
The AI version laid out a clean, structured happy-path flow with explicit verification points ("Verify user is logged in", "Verify redirect to Account page") that map directly onto automation assertions.

### What you felt Not suitable:- 
The AI version missed all the negative scenarios entirely — wrong phone number validation, OTP expiry, and Resend OTP. These only surfaced because I actually tried entering a wrong number and letting the timer run out on the real site.

## Final Test Case:- (AI + Manual, Combined, Automation Ready)
### Final Test Case_001 — Login with Mobile OTP (Automation Ready)

Navigate to https://grocerystoredemo.pcubeweb.com/;
Click on the "Account" link;
Verify that the Sign In modal is displayed with a mobile number field;
Enter an invalid mobile number and click "Send OTP";
Verify that a validation error message is displayed;
Enter a valid registered mobile number and click "Send OTP";
Verify that the OTP Verification modal is displayed;
Enter the correct OTP received within the validity time and click "Verify"

## TestCases_002 — Account Page After Sign-in (Manage Addresses) ##
### QA Manual Test Cases:-
Member :- Saheli Das
#### Query/Test cases:- Grocery Store Demo (Human Thinking Test Cases)

My Orders menu is getting selected by default;
Click on My Addressess Link from Menu bar;
Display Add new Address with (+) button;
Click on Add new Address with (+) button;
Display Add new address popup modal;
Click on Add address button without enter value;
Check validation messages;
Enter correct adderess with name & mobile number;
Click on Add Address button;
Display Added Address

### AI Manual Test Cases:-
Member :- Saheli Das

#### Prompt:- Write test cases for adding a new address in the Grocery Store Demo account
Log in and navigate to the Account page;
Verify that "My Orders" tab is selected by default;
Click on "My Addresses";
Click on the "Add new Address (+)" button;
Submit the form without entering any details;
Verify that validation messages are displayed for mandatory fields;
Enter a valid Name, Mobile Number and Address;
Click on "Add Address" button;
Verify that the address is saved successfully;
Verify that the newly added address appears in the address list

## Your thoughts:-
### What you felt Suitable:- 
The AI version captured the full happy path and explicitly called out checking the validation messages before re-submitting — easy to turn into separate pass/fail assertions.

### What you felt Not suitable:- 
The AI version doesn't know the exact UI element is a "(+)" icon button or that the modal is called "Add new address" — it only got those specifics because I fed it the manual steps first. On its own it would have guessed generic field names.

## Final Test Case:- (AI + Manual, Combined, Automation Ready)
### Final Test Case_002 — Add New Address (Automation Ready)

Log in to the Grocery Store Demo account;
Verify that "My Orders" tab is selected by default on the Account page;
Click on "My Addresses" from the menu bar;
Verify that the "Add new Address (+)" button is displayed;
Click on the "Add new Address (+)" button and verify the popup modal opens;
Click "Add Address" without entering any values and verify validation messages are shown;
Enter a valid Name, Mobile Number and Address;
Click on "Add Address" button;
Verify that the new address is displayed correctly in the address list

## TestCases_003 — Sort & Filter Products ##
### QA Manual Test Cases:-
Member :- Saheli Das

#### Query/Test cases:- Grocery Store Demo (Human Thinking Test Cases)
Click on Categories;
Navigate to the Categories page;
Display All Product categories;
Click on one category;
Navigate to the product category page;
Sort and filter the product page;
Display product lists based on sort & Filter

### AI Manual Test Cases:-
Member :- Saheli Das

#### Prompt:- Write test cases for sorting and filtering products on the Grocery Store Demo categories page
Click on "Categories" ;
Verify that the Categories page displays all product categories ;
Click on any one category ;
Verify that the product listing page for that category loads ;
Click on "Sort by" and select "Price low to high" ;
Verify that products are displayed in ascending order of price ;
Select "Price high to low" ;
Verify that products are displayed in descending order of price

## Your thoughts:-
### What you felt Suitable:- 
The AI version broke my vague step "Sort and filter the product page" into two concrete, individually testable cases (low-to-high, high-to-low) with a clear expected outcome for each — much easier to automate than one broad manual step.

### What you felt Not suitable:- 
The AI version only tested two of the four sort options shown on the site (Featured and Discount were skipped) since it wasn't told the full list — it guessed the two most common ones rather than verifying against the actual UI.

## Final Test Case:- (AI + Manual, Combined, Automation Ready)
### Final Test Case_003 — Sort & Filter Products (Automation Ready)

Click on "Categories" and verify the Categories page lists all product categories ;
Click on one category and verify navigation to its product listing page ;
Verify the product listing page displays products for the selected category  ;
Click on "Sort by" and select "Price low to high"; verify products are re-ordered in ascending price order ;
Select "Price high to low"; 
verify products are re-ordered in descending price order

## TestCases_004 — Search Product ##
### QA Manual Test Cases:-
Member :- Saheli Das
#### Query/Test cases:- Grocery Store Demo (Human Thinking Test Cases)

Search with categories or Products
Display Search results

### AI Manual Test Cases:-
Member :- Saheli Das

#### Prompt:- Write test cases for the product search functionality on Grocery Store Demo
Click on the search bar ;
Enter a valid product name ;
Verify that relevant search results are displayed ;
Enter a valid category name ;
Verify that relevant search results are displayed ;
Enter a keyword that does not match any product ;
Verify that a "No products found" message is displayed

## Your thoughts:-
### What you felt Suitable:- 
The AI version added a "no results found" negative case on its own, which wasn't in my manual notes — a useful gap-filler I hadn't thought to write down.

### What you felt Not suitable:- 
The AI version uses generic placeholders like "a valid product name" instead of real product names from the site (e.g. "Cadbury", "Lays") — manual testing naturally uses real data because I'm looking at the actual catalog.

## Final Test Case:- (AI + Manual, Combined, Automation Ready)
### Final Test Case_004 — Search Product (Automation Ready)

Click on the search bar and enter a valid product or category keyword ;
Verify that the search results display matching products ;
Enter a keyword with no matching products ;
Verify that an appropriate "No products found" message is displayed instead of a blank page

## TestCases_005 — Add to Cart and Proceed to Checkout ##

### QA Manual Test Cases:-
Member :- Saheli Das
#### Query/Test cases:- Grocery Store Demo (Human Thinking Test Cases)
Click on Add + button to add a product to the cart ;
Click on Cart ;
Navigate to the Cart page ;
Click on + button to increase quantity ;
Check the updated quantity ;
Click on Proceed to Checkout button

### AI Manual Test Cases:-
Member :- Saheli Das

#### Prompt:- Write test cases for add to cart and proceed to checkout flow on Grocery Store Demo

Click on the "ADD" button for a product ;
Verify that the product is added to the cart ;
Click on the Cart icon ;
Verify that the Cart page displays the added product with correct price ;
Click on the "+" button to increase quantity ;
Verify that the quantity and cart total update correctly ;
Click on "Proceed to Checkout" ;
Verify that the user is navigated to the Checkout page

## Your thoughts:-
### What you felt Suitable:- 
The AI version explicitly added "Verify that the cart total updates correctly" after the quantity change — my manual step just said "check the updated quantity" without mentioning the price total, so this is a useful addition.

### What you felt Not suitable:- 
The AI version only tests increasing quantity, not decreasing it or removing an item entirely (quantity going to 0) — that edge case only came up because I was clicking around the cart myself.

## Final Test Case:- (AI + Manual, Combined, Automation Ready)
### Final Test Case_005 — Add to Cart & Checkout (Automation Ready)

Click on the "ADD" button for a product and verify it is added to the cart ;
Click on the Cart icon and verify navigation to the Cart page ;
Click on the "+" button and verify quantity and cart total update correctly ;
Click on "Proceed to Checkout" and verify navigation to the Checkout page ;

## TestCases_006 — Place Order ##

### QA Manual Test Cases:-
Member :- Saheli Das

#### Query/Test cases:- Grocery Store Demo (Human Thinking Test Cases)

Navigate to the Checkout page ;
Check that added address already populate as Shipping Address ;
Select shipping address same as Billing address ;
Select shipping method ;
Select on Credit card ;
Enter Credit Card and Credit card name, Expiry date and cvv number ;
Click on Complete order ;
Navigate to the Thank you page ;
Check the created order ID, Shipping and Billing address and Product with Quantity

### AI Manual Test Cases:-
Member :- Saheli Das

#### Prompt:- Write test cases for placing an order on the Grocery Store Demo checkout page
Navigate to the Checkout page ;
Verify that the saved address is pre-filled as Shipping Address ;
Select shipping address same as Billing address ;
Select a shipping method ;
Select "Credit Card" as the payment method ;
Enter valid Card Number, Card Holder Name, Expiry Date and CVV ;
Click on "Complete Order" ;
Verify that the order is placed successfully and the Thank You page is displayed ;
Verify that the Order ID, Shipping/Billing address and product with quantity are displayed correctly

## Your thoughts:-
### What you felt Suitable:- 
The AI version's steps map almost one-to-one onto a Page Object Model automation script — each step is a single, isolated, verifiable action (enter card number, click complete order, verify Thank You page).

### What you felt Not suitable:- 
The AI version has no idea the site currently shows "Sorry we're currently not accepting orders" — that's a real blocker that only showed up when I tried to actually place an order. AI can't catch environment-specific issues like that without being told.

## Final Test Case:- (AI + Manual, Combined, Automation Ready)
### Final Test Case_006 — Place Order (Automation Ready)
Navigate to the Checkout page and verify the saved address auto-populates as Shipping Address ;
Select shipping address same as Billing address ;
Select a shipping method ;
Select "Credit Card" and enter valid Card Number, Card Holder Name, Expiry Date and CVV ;
Click on "Complete Order" ;
Verify navigation to the Thank You page ;
Verify that the Order ID, Shipping/Billing address and product with quantity are correct on the Thank You page

## TestCases_007 — Account Page (Order History & Sign Out) ##

### QA Manual Test Cases:-
Member :- Saheli Das

#### Query/Test cases:- Grocery Store Demo (Human Thinking Test Cases)
Click on Account link ;
Check the Order has been created or not ;
Click on Sign out button ;
The user is getting logout from the Grocery Store

### AI Manual Test Cases:-
Member :- Saheli Das

#### Prompt:- Write test cases for verifying order history and sign out on Grocery Store Demo
- Click on "Account" link ;
- Open the "My Orders" tab ;
- Verify that the recently placed order is listed with correct Order ID and status ;
- Click on "Sign out" button ;
- Verify that the user is logged out successfully ;
- Verify that the user is redirected to the homepage in a logged-out state

## Your thoughts:-
### What you felt Suitable:- 
The AI version explicitly verifies the post-logout state (redirected to homepage, logged-out), while my manual note just said "user is getting logout" — the AI phrasing is more precise about what "success" actually means here.

### What you felt Not suitable:-
The AI version assumes an order will always exist to check in "My Orders" — it doesn't account for what should happen if no order was placed yet (e.g. an empty-state message), which is something I'd only think to test by using the account fresh.

### Final Test Case:- (AI + Manual, Combined, Automation Ready)
#### Final Test Case_007 — Order History & Sign Out (Automation Ready)
- Click on "Account" link and open the "My Orders" tab ;
- Verify that the recently placed order is listed with correct Order ID and status ;
- Click on "Sign out" button ;
- Verify that the user is logged out and redirected to the homepage in a logged-out state ;
- Verify that the user is logged in successfully and redirected to the Account page

------------------------- ------------------------ Session 2 - Assignment -------------------------------------------------
# Name #

Enterprise QA Test Case Generator – Grocery Store Demo E-Commerce

# Purpose #

Generate exhaustive, structured, automation-ready QA test cases from requirements, user stories, acceptance criteria, business rules, UI designs, workflows, or feature descriptions.

The generated test cases must simulate real user behavior and provide complete test coverage for all functional and non-functional aspects of the Grocery Store application.

The skill should think like:

Senior QA Engineer ;
Business User ;
End Customer ;
Negative Tester ;
Automation Engineer ;
Security Tester ;
Core Objective

# Never generate only happy-path scenarios.

Always generate:

  ✓ Positive Scenarios ;
  ✓ Negative Scenarios ;
  ✓ Boundary Value Scenarios ;
  ✓ Validation Scenarios ;
  ✓ UI Scenarios ;
  ✓ Functional Scenarios ;
  ✓ Navigation Scenarios ;
  ✓ Error Handling Scenarios ;
  ✓ Integration Scenarios ;
  ✓ Security Scenarios ;
  ✓ Regression Scenarios ;
  ✓ Edge Cases

# Coverage Rules (Mandatory)

Before generating test cases, identify all possible feature areas.

If the feature contains multiple modules, generate test cases for every module.

## Example:

-- ------------------------------Login Feature ------------------

Generate cases for:

Mobile Number Validation ;
OTP Generation ;
OTP Verification ;
OTP Expiry ;
Resend OTP ;
Invalid OTP ;
Session Creation ;
Logout ;
Browser Refresh ;
Multiple Login Attempts

--------------------------------Product Feature---------------------

Generate cases for:

Categories ;
Search ;
Filters ;
Sorting ;
Product Details ;
Product Availability ;
Product Images

-------------------------------Cart Feature---------------------

Generate cases for:

Add to Cart ;
Remove Product ;
Increase Quantity ;
Decrease Quantity ;
Cart Calculation ;
Empty Cart ;
Duplicate Products

------------------------------Checkout Feature---------------------

Generate cases for:

Shipping Address ;
Billing Address ;
Shipping Methods ;
Payment Methods ;
Coupon Codes ;
Order Placement ;
Order Confirmation ;

------------------------------Account Feature-------------------------

Generate cases for:

My Profile ;
Address Management ;
Order History ;
Sign Out ;
Test Design Techniques (Mandatory)

## Generate scenarios using:

### Equivalence Partitioning

Valid and invalid input classes.

### Boundary Value Analysis

Minimum value ;
Maximum value ;
Just Below Minimum ;
Just Above Maximum

### Error Guessing

Generate scenarios based on common user mistakes.

## State Transition Testing

### Example:

OTP Generated ;
OTP Expired ;
OTP Resent ;
OTP Verified ;
Decision Table Testing

### Example:

| Mobile  | OTP     | Result  |
| ------- | ------- | ------- |
| Valid   | Valid   | Success |
| Valid   | Invalid | Error   |
| Invalid | Valid   | Error   |
| Invalid | Invalid | Error   |

# Smart Coverage Reminder #

When generating test cases:

DO NOT stop after:

Login Success ;
Add Address Success ;
Add to Cart Success  ;
Order Success ;

## Also generate:

What if user:
Clicks button multiple times ;
Refreshes page ;
Uses browser back button ;
Uses invalid data ;
Leaves mandatory fields blank ;
Uses special characters ;
Uses emojis ;
Uses SQL Injection text ;
Uses script tags ;
Uses expired OTP ;
Uses duplicate address ;
Uses invalid payment details 

## Priority Assignment Rules
---- High ---

Revenue impacting ;
Business critical ;

### Examples:

Login ;
Checkout ;
Payment ;
Place Order

---- Medium ---

## Important functionality

### Examples:

Search ;
Filter ;
Address

------ Low ----

## Cosmetic validations

UI alignment ;
Optional features

## Test Type Assignment Rules

Assign one or more:

Functional ;
UI ;
Validation ; 
Negative ;
Boundary ;
Security ;
Integration ;
Regression ;
Smoke ;
Sanity ;

## Output Format (RCTFC) ##

Generate all test cases using the following format:
| Req ID | Component | Test Case ID | Feature | Test Scenario | Test Steps | Test Data | Expected Result | Priority | Test Type |
| ------ | --------- | ------------ | ------- | ------------- | ---------- | --------- | --------------- | -------- | --------- |

## RCTFC Field Definition ##
### Req ID ###

Requirement identifier.

### Example:

REQ_LOGIN_001

## Component ##

Feature area.

### Examples:

Login ;
OTP ;
Address ;
Search ;
Cart ;
Checkout ;
Order ;

## Test Case ID ##

Unique identifier.

### Example:

TC_001 ;
TC_002 ;
TC_003

## Feature

Feature name.

### Example:

Login with Mobile Number

## Test Scenario ##

Brief description.

### Example:

Verify user can login using valid OTP.

## Test Steps ##

Detailed execution steps.

## Test Data ##

Input values.

### Example:

Mobile: 9876543210
OTP: 123456

## Expected Result ##

System behavior.
Priority ;
High ;
Medium ;
Low ;

## Test Type ##

Functional ;
Negative ;
Boundary ;
Validation ;
Security ;
Regression

|Req ID |	Component |	Test Case ID |	Feature	| Test Scenario |	Test Steps |	Test Data |	Expected Result |	Priority |	Test Type |
| ------ | --------- | ------------ | ------- | ------------- | ---------- | --------- | --------------- | -------- | --------- |

|REQ_LOGIN_001|	Login	TC_001|	Mobile Login|	Verify login with valid mobile number and OTP| 	1. Open website → 2. Click Account → 3. Enter valid mobile → 4. Click Send OTP → 5. Enter valid OTP → 6. Click Verify	| Mobile: 9876543210 OTP: 123456 |	User should login successfully|	High	|Functional |

|REQ_LOGIN_002|	Login|	TC_002|	Mobile Login	|Verify error message for invalid mobile number|	Enter invalid mobile number and click Send OTP|	Mobile: 12345	|Validation message should appear	|High|	Validation|

|REQ_LOGIN_003|	OTP|	TC_003|	OTP Verification|	Verify expired OTP cannot be used|	Generate OTP and wait until expiry|	OTP: Expired|	Appropriate error message displayed	|High|	Negative|

|REQ_LOGIN_004|	OTP	|TC_004	|OTP Verification|	Verify Resend OTP functionality	|Click Resend OTP after timer expires|	N/A|	New OTP generated, old OTP invalid	|High	|Functional|

|REQ_PRODUCT_005|	Product|	TC_005|	Search|	Verify product search with valid keyword|	Enter “Milk” in search bar → Click Search	|Keyword: Milk|	Relevant products displayed|	Medium|	Functional|

|REQ_PRODUCT_006|	Product|	TC_006|	Search|	Verify search with special characters|	Enter “@@@” in search bar → Click Search|	Keyword: @@@|	No products found, error message shown|	Medium|	Negative

REQ_CART_007	Cart	TC_007	Add to Cart	Verify adding product to cart	Select product → Click “Add to Cart”	Product: Bread	Product added to cart	High	Functional

|REQ_CART_008	|Cart	|TC_008	|Cart Calculation|	Verify cart total calculation|	Add 2 products → Check cart| total	Bread ₹40, Milk ₹50|	Total = ₹90|	High	|Functional|

|REQ_CART_009	|Cart	|TC_009	|Duplicate Products	|Verify duplicate product handling|	Add same product twice	|Product: Bread |	Quantity increases, not duplicate entry|	High|	Regression|

|REQ_CHECKOUT_010	|Checkout	|TC_010	|Payment|	Verify checkout with valid card	|Enter valid card details → Place order	|Card: 4111111111111111	|Payment successful, order placed	|High|	Functional|

|REQ_CHECKOUT_011|	Checkout|	TC_011|	Payment|	Verify checkout with invalid card	|Enter invalid card number → Place order|	Card: 123456|	Error message shown, payment declined|	High	|Negative|

|REQ_CHECKOUT_012|	Checkout	|TC_012	|Coupon|	Verify coupon application|	Apply valid coupon code	|Coupon: SAVE10|	Discount applied|	Medium	|Functional|

|REQ_ACCOUNT_013|	Account	|TC_013|	Profile|	Verify profile update	|Navigate to My Profile → Edit name → Save|	Name: “Saheli QA”	Profile updated successfully|	Medium|	Functional|

|REQ_ACCOUNT_014|	Account|	TC_014	|Order History|	Verify order history displays past orders	| Navigate to Order History|	N/A|	Past orders displayed	|Medium	|Functional|

|REQ_SECURITY_015|	Security|	TC_015	|SQL Injection|	Verify login input against SQL injection|	Enter “' OR 1=1 --” in mobile field	Mobile: ' OR 1=1 --|	System should block input, show error|	High	|Security|

|REQ_SECURITY_016|	Security|	TC_016|	XSS Attack|	Verify product review input against script tags|	Enter “<script>alert(1)</script>” in review	Review: <script>alert(1)</script>|	Input sanitized, no script execution|	High|	Security|

|REQ_NAVIGATION_017|	Navigation	|TC_017|	Browser Back	|Verify checkout flow with browser back|	Add product → Proceed to checkout → Click browser back|	N/A	|User redirected safely, no duplicate order|	High|	Error Handling

|REQ_UI_018|	UI|	TC_018	|Alignment|	Verify cart button alignment on mobile|	Open site on mobile → Navigate to cart|	Device: iPhone|	Cart button aligned properly|	Low	|UI Validation|


## Recommended Prompt ##

Act as a Senior QA Engineer with 10+ years of experience in E-commerce applications.

Analyze the provided requirement thoroughly.

Generate exhaustive QA test cases in RCTFC format.

Requirements:
1. Cover all user journeys.
2. Cover positive scenarios.
3. Cover negative scenarios.
4. Cover validation scenarios.
5. Cover boundary value scenarios.
6. Cover edge cases.
7. Cover security scenarios.
8. Cover UI scenarios.
9. Cover integration scenarios.
10. Cover error handling scenarios.

When the application has multiple modules, generate test cases for every module while maintaining continuous numbering.

Assign Priority and Test Type.

Do not stop at happy-path scenarios.

Generate automation-ready test cases.



