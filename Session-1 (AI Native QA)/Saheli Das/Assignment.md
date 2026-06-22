AI + Manual Test Case Document
Grocery Store Demo
Member :- Saheli Das
Website: https://grocerystoredemo.pcubeweb.com/
Format: For each test scenario below — QA Manual Test Cases (as written by hand), AI Manual Test Cases (generated from a prompt), Your thoughts on comparing the two, and a Final Test Case combining both into an automation-ready scenario.

TestCases_001 — Account Verification & Creation

QA Manual Test Cases:-
Member :- Saheli Das
Query/Test cases:- Grocery Store Demo (Human Thinking Test Cases)

1. Go to website: grocerystoredemo.pcubeweb.com
2. Click on Account
3. Open Sign IN modal
4. Enter your wrong Phone Number
5. Click on Send OTP
6. Check the validation message
7. Enter your Correct Phone Number
8. Click on Send OTP
9. Display OTP Verification modal
10. Check your phone number to get OTP for login
11. Enter OTP within given time
12. Verify the OTP
13. Navigate to the Grocery Store Account page after Verification OTP

AI Manual Test Cases:-
Member :- Saheli Das

Prompt:- Write test cases for Grocery Store Demo login using mobile number and OTP
 Go to https://grocerystoredemo.pcubeweb.com/
 Click on Account
 Enter a valid registered mobile number
 Click on Send OTP
 Enter the valid OTP received within the time limit
 Click on Verify
 Verify that the user is logged in successfully
 Verify that the user is redirected to the Account page

Your thoughts:-
What you felt Suitable:- The AI version laid out a clean, structured happy-path flow with explicit verification points ("Verify user is logged in", "Verify redirect to Account page") that map directly onto automation assertions.

What you felt Not suitable:- The AI version missed all the negative scenarios entirely — wrong phone number validation, OTP expiry, and Resend OTP. These only surfaced because I actually tried entering a wrong number and letting the timer run out on the real site.

Final Test Case:- (AI + Manual, Combined, Automation Ready)
Final Test Case_001 — Login with Mobile OTP (Automation Ready)

Navigate to https://grocerystoredemo.pcubeweb.com/
Click on the "Account" link
Verify that the Sign In modal is displayed with a mobile number field
Enter an invalid mobile number and click "Send OTP"
Verify that a validation error message is displayed
Enter a valid registered mobile number and click "Send OTP"
Verify that the OTP Verification modal is displayed
Enter the correct OTP received within the validity time and click "Verify"

TestCases_002 — Account Page After Sign-in (Manage Addresses)
QA Manual Test Cases:-
Member :- Saheli Das
Query/Test cases:- Grocery Store Demo (Human Thinking Test Cases)

14. My Orders menu is getting selected by default
15. Click on My Addressess Link from Menu bar
16. Display Add new Address with (+) button
17. Click on Add new Address with (+) button
18. Display Add new address popup modal
19. Click on Add address button without enter value
20. Check validation messages
21. Enter correct adderess with name & mobile number
22. Click on Add Address button
23. Display Added Address

AI Manual Test Cases:-
Member :- Saheli Das

Prompt:- Write test cases for adding a new address in the Grocery Store Demo account
Log in and navigate to the Account page
Verify that "My Orders" tab is selected by default
Click on "My Addresses"
Click on the "Add new Address (+)" button
Submit the form without entering any details
Verify that validation messages are displayed for mandatory fields
Enter a valid Name, Mobile Number and Address
Click on "Add Address" button
Verify that the address is saved successfully
Verify that the newly added address appears in the address list

Your thoughts:-
What you felt Suitable:- The AI version captured the full happy path and explicitly called out checking the validation messages before re-submitting — easy to turn into separate pass/fail assertions.

What you felt Not suitable:- The AI version doesn't know the exact UI element is a "(+)" icon button or that the modal is called "Add new address" — it only got those specifics because I fed it the manual steps first. On its own it would have guessed generic field names.

Final Test Case:- (AI + Manual, Combined, Automation Ready)
Final Test Case_002 — Add New Address (Automation Ready)

Log in to the Grocery Store Demo account
Verify that "My Orders" tab is selected by default on the Account page
Click on "My Addresses" from the menu bar
54. Verify that the "Add new Address (+)" button is displayed
Click on the "Add new Address (+)" button and verify the popup modal opens
Click "Add Address" without entering any values and verify validation messages are shown
Enter a valid Name, Mobile Number and Address
Click on "Add Address" button
Verify that the new address is displayed correctly in the address list

TestCases_003 — Sort & Filter Products
QA Manual Test Cases:-
Member :- Saheli Das

Query/Test cases:- Grocery Store Demo (Human Thinking Test Cases)
24. Click on Categories
25. Navigate to the Categories page
26. Display All Product categories
27. Click on one category
28. Navigate to the product category page
29. Sort and filter the product page
30. Display product lists based on sort & Filter

AI Manual Test Cases:-
Member :- Saheli Das

Prompt:- Write test cases for sorting and filtering products on the Grocery Store Demo categories page
Click on "Categories"
Verify that the Categories page displays all product categories
Click on any one category
Verify that the product listing page for that category loads
Click on "Sort by" and select "Price low to high"
Verify that products are displayed in ascending order of price
Select "Price high to low"
Verify that products are displayed in descending order of price

Your thoughts:-
What you felt Suitable:- The AI version broke my vague step "Sort and filter the product page" into two concrete, individually testable cases (low-to-high, high-to-low) with a clear expected outcome for each — much easier to automate than one broad manual step.

What you felt Not suitable:- The AI version only tested two of the four sort options shown on the site (Featured and Discount were skipped) since it wasn't told the full list — it guessed the two most common ones rather than verifying against the actual UI.

Final Test Case:- (AI + Manual, Combined, Automation Ready)
Final Test Case_003 — Sort & Filter Products (Automation Ready)

Click on "Categories" and verify the Categories page lists all product categories
Click on one category and verify navigation to its product listing page
Verify the product listing page displays products for the selected category
Click on "Sort by" and select "Price low to high"; 
Verify products are re-ordered in ascending price order
Select "Price high to low"; 
Verify products are re-ordered in descending price order

TestCases_004 — Search Product
QA Manual Test Cases:-
Member :- Saheli Das
Query/Test cases:- Grocery Store Demo (Human Thinking Test Cases)

31. Search with categories or Products
32. Display Search results

AI Manual Test Cases:-
Member :- Saheli Das

Prompt:- Write test cases for the product search functionality on Grocery Store Demo
Click on the search bar
Enter a valid product name
Verify that relevant search results are displayed
Enter a valid category name
Verify that relevant search results are displayed
Enter a keyword that does not match any product
Verify that a "No products found" message is displayed

Your thoughts:-
What you felt Suitable:- The AI version added a "no results found" negative case on its own, which wasn't in my manual notes — a useful gap-filler I hadn't thought to write down.

What you felt Not suitable:- The AI version uses generic placeholders like "a valid product name" instead of real product names from the site (e.g. "Cadbury", "Lays") — manual testing naturally uses real data because I'm looking at the actual catalog.

Final Test Case:- (AI + Manual, Combined, Automation Ready)
Final Test Case_004 — Search Product (Automation Ready)

Click on the search bar and enter a valid product or category keyword
Verify that the search results display matching products
Enter a keyword with no matching products
Verify that an appropriate "No products found" message is displayed instead of a blank page

TestCases_005 — Add to Cart and Proceed to Checkout

QA Manual Test Cases:-
Member :- Saheli Das
Query/Test cases:- Grocery Store Demo (Human Thinking Test Cases)

33. Click on Add + button to add a product to the cart
34. Click on Cart
35. Navigate to the Cart page
36. Click on + button to increase quantity
37. Check the updated quantity
38. Click on Proceed to Checkout button

AI Manual Test Cases:-
Member :- Saheli Das
Prompt:- Write test cases for add to cart and proceed to checkout flow on Grocery Store Demo

Click on the "ADD" button for a product
Verify that the product is added to the cart
Click on the Cart icon
Verify that the Cart page displays the added product with correct price
Click on the "+" button to increase quantity
Verify that the quantity and cart total update correctly
Click on "Proceed to Checkout"
Verify that the user is navigated to the Checkout page

Your thoughts:-

What you felt Suitable:- The AI version explicitly added "Verify that the cart total updates correctly" after the quantity change — my manual step just said "check the updated quantity" without mentioning the price total, so this is a useful addition.

What you felt Not suitable:- The AI version only tests increasing quantity, not decreasing it or removing an item entirely (quantity going to 0) — that edge case only came up because I was clicking around the cart myself.

Final Test Case:- (AI + Manual, Combined, Automation Ready)
Final Test Case_005 — Add to Cart & Checkout (Automation Ready)

Click on the "ADD" button for a product and verify it is added to the cart
Click on the Cart icon and verify navigation to the Cart page
Click on the "+" button and verify quantity and cart total update correctly
Click on "Proceed to Checkout" and verify navigation to the Checkout page

TestCases_006 — Place Order

QA Manual Test Cases:-
Member :- Saheli Das
Query/Test cases:- Grocery Store Demo (Human Thinking Test Cases)

39. Navigate to the Checkout page
40. Check that added address already populate as Shipping Address
41. Select shipping address same as Billing address
42. Select shipping method
43. Select on Credit card
44. Enter Credit Card and Credit card name, Expiry date and cvv number
45. Click on Complete order
46. Navigate to the Thank you page
47. Check the created order ID, Shipping and Billing address and Product with Quantity

AI Manual Test Cases:-
Member :- Saheli Das

Prompt:- Write test cases for placing an order on the Grocery Store Demo checkout page
Navigate to the Checkout page
Verify that the saved address is pre-filled as Shipping Address
Select shipping address same as Billing address
Select a shipping method
Select "Credit Card" as the payment method
Enter valid Card Number, Card Holder Name, Expiry Date and CVV
Click on "Complete Order"
Verify that the order is placed successfully and the Thank You page is displayed
Verify that the Order ID, Shipping/Billing address and product with quantity are displayed correctly

Your thoughts:-
What you felt Suitable:- The AI version's steps map almost one-to-one onto a Page Object Model automation script — each step is a single, isolated, verifiable action (enter card number, click complete order, verify Thank You page).

What you felt Not suitable:- The AI version has no idea the site currently shows "Sorry we're currently not accepting orders" — that's a real blocker that only showed up when I tried to actually place an order. AI can't catch environment-specific issues like that without being told.

Final Test Case:- (AI + Manual, Combined, Automation Ready)
Final Test Case_006 — Place Order (Automation Ready)

Navigate to the Checkout page and verify the saved address auto-populates as Shipping Address
Select shipping address same as Billing address
Select a shipping method
Select "Credit Card" and enter valid Card Number, Card Holder Name, Expiry Date and CVV
Click on "Complete Order"
Verify navigation to the Thank You page
Verify that the Order ID, Shipping/Billing address and product with quantity are correct on the Thank You page

TestCases_007 — Account Page (Order History & Sign Out)

QA Manual Test Cases:-
Member :- Saheli Das

Query/Test cases:- Grocery Store Demo (Human Thinking Test Cases)
48. Click on Account link
49. Check the Order has been created or not
50. Click on Sign out button
51. The user is getting logout from the Grocery Store

AI Manual Test Cases:-
Member :- Saheli Das

Prompt:- Write test cases for verifying order history and sign out on Grocery Store Demo
Click on "Account" link
Open the "My Orders" tab
Verify that the recently placed order is listed with correct Order ID and status
Click on "Sign out" button
Verify that the user is logged out successfully
Verify that the user is redirected to the homepage in a logged-out state

Your thoughts:-
What you felt Suitable:- The AI version explicitly verifies the post-logout state (redirected to homepage, logged-out), while my manual note just said "user is getting logout" — the AI phrasing is more precise about what "success" actually means here.

What you felt Not suitable:- The AI version assumes an order will always exist to check in "My Orders" — it doesn't account for what should happen if no order was placed yet (e.g. an empty-state message), which is something I'd only think to test by using the account fresh.

Final Test Case:- (AI + Manual, Combined, Automation Ready)
Final Test Case_007 — Order History & Sign Out (Automation Ready)

Click on "Account" link and open the "My Orders" tab
Verify that the recently placed order is listed with correct Order ID and status
Click on "Sign out" button
Verify that the user is logged out and redirected to the homepage in a logged-out state
Verify that the user is logged in successfully and redirected to the Account page

