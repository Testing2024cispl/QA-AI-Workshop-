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
14. Go to https://grocerystoredemo.pcubeweb.com/
15. Click on Account
16. Enter a valid registered mobile number
17. Click on Send OTP
18. Enter the valid OTP received within the time limit
19. Click on Verify
20. Verify that the user is logged in successfully
21. Verify that the user is redirected to the Account page

Your thoughts:-
What you felt Suitable:- The AI version laid out a clean, structured happy-path flow with explicit verification points ("Verify user is logged in", "Verify redirect to Account page") that map directly onto automation assertions.

What you felt Not suitable:- The AI version missed all the negative scenarios entirely — wrong phone number validation, OTP expiry, and Resend OTP. These only surfaced because I actually tried entering a wrong number and letting the timer run out on the real site.

Final Test Case:- (AI + Manual, Combined, Automation Ready)
Final Test Case_001 — Login with Mobile OTP (Automation Ready)

22. Navigate to https://grocerystoredemo.pcubeweb.com/
23. Click on the "Account" link
24. Verify that the Sign In modal is displayed with a mobile number field
25. Enter an invalid mobile number and click "Send OTP"
26. Verify that a validation error message is displayed
27. Enter a valid registered mobile number and click "Send OTP"
28. Verify that the OTP Verification modal is displayed
29. Enter the correct OTP received within the validity time and click "Verify"

TestCases_002 — Account Page After Sign-in (Manage Addresses)
QA Manual Test Cases:-
Member :- Saheli Das
Query/Test cases:- Grocery Store Demo (Human Thinking Test Cases)

31. My Orders menu is getting selected by default
32. Click on My Addressess Link from Menu bar
33. Display Add new Address with (+) button
34. Click on Add new Address with (+) button
35. Display Add new address popup modal
36. Click on Add address button without enter value
37. Check validation messages
38. Enter correct adderess with name & mobile number
39. Click on Add Address button
40. Display Added Address

AI Manual Test Cases:-
Member :- Saheli Das

Prompt:- Write test cases for adding a new address in the Grocery Store Demo account
41. Log in and navigate to the Account page
42. Verify that "My Orders" tab is selected by default
43. Click on "My Addresses"
44. Click on the "Add new Address (+)" button
45. Submit the form without entering any details
46. Verify that validation messages are displayed for mandatory fields
47. Enter a valid Name, Mobile Number and Address
48. Click on "Add Address" button
49. Verify that the address is saved successfully
50. Verify that the newly added address appears in the address list

Your thoughts:-
What you felt Suitable:- The AI version captured the full happy path and explicitly called out checking the validation messages before re-submitting — easy to turn into separate pass/fail assertions.

What you felt Not suitable:- The AI version doesn't know the exact UI element is a "(+)" icon button or that the modal is called "Add new address" — it only got those specifics because I fed it the manual steps first. On its own it would have guessed generic field names.

Final Test Case:- (AI + Manual, Combined, Automation Ready)
Final Test Case_002 — Add New Address (Automation Ready)

51. Log in to the Grocery Store Demo account
52. Verify that "My Orders" tab is selected by default on the Account page
53. Click on "My Addresses" from the menu bar
54. Verify that the "Add new Address (+)" button is displayed
55. Click on the "Add new Address (+)" button and verify the popup modal opens
56. Click "Add Address" without entering any values and verify validation messages are shown
57. Enter a valid Name, Mobile Number and Address
58. Click on "Add Address" button
59. Verify that the new address is displayed correctly in the address list

TestCases_003 — Sort & Filter Products
QA Manual Test Cases:-
Member :- Saheli Das

Query/Test cases:- Grocery Store Demo (Human Thinking Test Cases)
60. Click on Categories
61. Navigate to the Categories page
62. Display All Product categories
63. Click on one category
64. Navigate to the product category page
65. Sort and filter the product page
66. Display product lists based on sort & Filter

AI Manual Test Cases:-
Member :- Saheli Das

Prompt:- Write test cases for sorting and filtering products on the Grocery Store Demo categories page
67. Click on "Categories"
68. Verify that the Categories page displays all product categories
69. Click on any one category
70. Verify that the product listing page for that category loads
71. Click on "Sort by" and select "Price low to high"
72. Verify that products are displayed in ascending order of price
73. Select "Price high to low"
74. Verify that products are displayed in descending order of price

Your thoughts:-
What you felt Suitable:- The AI version broke my vague step "Sort and filter the product page" into two concrete, individually testable cases (low-to-high, high-to-low) with a clear expected outcome for each — much easier to automate than one broad manual step.

What you felt Not suitable:- The AI version only tested two of the four sort options shown on the site (Featured and Discount were skipped) since it wasn't told the full list — it guessed the two most common ones rather than verifying against the actual UI.

Final Test Case:- (AI + Manual, Combined, Automation Ready)
Final Test Case_003 — Sort & Filter Products (Automation Ready)

75. Click on "Categories" and verify the Categories page lists all product categories
76. Click on one category and verify navigation to its product listing page
77. Verify the product listing page displays products for the selected category
78. Click on "Sort by" and select "Price low to high"; verify products are re-ordered in ascending price order
79. Select "Price high to low"; verify products are re-ordered in descending price order

TestCases_004 — Search Product
QA Manual Test Cases:-
Member :- Saheli Das
Query/Test cases:- Grocery Store Demo (Human Thinking Test Cases)

80. Search with categories or Products
81. Display Search results

AI Manual Test Cases:-
Member :- Saheli Das

Prompt:- Write test cases for the product search functionality on Grocery Store Demo
82. Click on the search bar
83. Enter a valid product name
84. Verify that relevant search results are displayed
85. Enter a valid category name
86. Verify that relevant search results are displayed
87. Enter a keyword that does not match any product
88. Verify that a "No products found" message is displayed

Your thoughts:-
What you felt Suitable:- The AI version added a "no results found" negative case on its own, which wasn't in my manual notes — a useful gap-filler I hadn't thought to write down.

What you felt Not suitable:- The AI version uses generic placeholders like "a valid product name" instead of real product names from the site (e.g. "Cadbury", "Lays") — manual testing naturally uses real data because I'm looking at the actual catalog.

Final Test Case:- (AI + Manual, Combined, Automation Ready)
Final Test Case_004 — Search Product (Automation Ready)

89. Click on the search bar and enter a valid product or category keyword
90. Verify that the search results display matching products
91. Enter a keyword with no matching products
92. Verify that an appropriate "No products found" message is displayed instead of a blank page

TestCases_005 — Add to Cart and Proceed to Checkout

QA Manual Test Cases:-
Member :- Saheli Das
Query/Test cases:- Grocery Store Demo (Human Thinking Test Cases)

93. Click on Add + button to add a product to the cart
94. Click on Cart
95. Navigate to the Cart page
96. Click on + button to increase quantity
97. Check the updated quantity
98. Click on Proceed to Checkout button

AI Manual Test Cases:-
Member :- Saheli Das
Prompt:- Write test cases for add to cart and proceed to checkout flow on Grocery Store Demo

99. Click on the "ADD" button for a product
100. Verify that the product is added to the cart
101. Click on the Cart icon
102. Verify that the Cart page displays the added product with correct price
103. Click on the "+" button to increase quantity
104. Verify that the quantity and cart total update correctly
105. Click on "Proceed to Checkout"
106. Verify that the user is navigated to the Checkout page

Your thoughts:-

What you felt Suitable:- The AI version explicitly added "Verify that the cart total updates correctly" after the quantity change — my manual step just said "check the updated quantity" without mentioning the price total, so this is a useful addition.

What you felt Not suitable:- The AI version only tests increasing quantity, not decreasing it or removing an item entirely (quantity going to 0) — that edge case only came up because I was clicking around the cart myself.

Final Test Case:- (AI + Manual, Combined, Automation Ready)
Final Test Case_005 — Add to Cart & Checkout (Automation Ready)

107. Click on the "ADD" button for a product and verify it is added to the cart
108. Click on the Cart icon and verify navigation to the Cart page
109. Click on the "+" button and verify quantity and cart total update correctly
110. Click on "Proceed to Checkout" and verify navigation to the Checkout page

TestCases_006 — Place Order

QA Manual Test Cases:-
Member :- Saheli Das
Query/Test cases:- Grocery Store Demo (Human Thinking Test Cases)

111. Navigate to the Checkout page
112. Check that added address already populate as Shipping Address
113. Select shipping address same as Billing address
114. Select shipping method
115. Select on Credit card
116. Enter Credit Card and Credit card name, Expiry date and cvv number
117. Click on Complete order
118. Navigate to the Thank you page
119. Check the created order ID, Shipping and Billing address and Product with Quantity

AI Manual Test Cases:-
Member :- Saheli Das

Prompt:- Write test cases for placing an order on the Grocery Store Demo checkout page
120. Navigate to the Checkout page
121. Verify that the saved address is pre-filled as Shipping Address
122. Select shipping address same as Billing address
123. Select a shipping method
124. Select "Credit Card" as the payment method
125. Enter valid Card Number, Card Holder Name, Expiry Date and CVV
126. Click on "Complete Order"
127. Verify that the order is placed successfully and the Thank You page is displayed
128. Verify that the Order ID, Shipping/Billing address and product with quantity are displayed correctly

Your thoughts:-
What you felt Suitable:- The AI version's steps map almost one-to-one onto a Page Object Model automation script — each step is a single, isolated, verifiable action (enter card number, click complete order, verify Thank You page).

What you felt Not suitable:- The AI version has no idea the site currently shows "Sorry we're currently not accepting orders" — that's a real blocker that only showed up when I tried to actually place an order. AI can't catch environment-specific issues like that without being told.

Final Test Case:- (AI + Manual, Combined, Automation Ready)
Final Test Case_006 — Place Order (Automation Ready)
129. Navigate to the Checkout page and verify the saved address auto-populates as Shipping Address
130. Select shipping address same as Billing address
131. Select a shipping method
132. Select "Credit Card" and enter valid Card Number, Card Holder Name, Expiry Date and CVV
133. Click on "Complete Order"
134. Verify navigation to the Thank You page
135. Verify that the Order ID, Shipping/Billing address and product with quantity are correct on the Thank You page

TestCases_007 — Account Page (Order History & Sign Out)

QA Manual Test Cases:-
Member :- Saheli Das

Query/Test cases:- Grocery Store Demo (Human Thinking Test Cases)
136. Click on Account link
137. Check the Order has been created or not
138. Click on Sign out button
139. The user is getting logout from the Grocery Store

AI Manual Test Cases:-
Member :- Saheli Das

Prompt:- Write test cases for verifying order history and sign out on Grocery Store Demo
140. Click on "Account" link
141. Open the "My Orders" tab
142. Verify that the recently placed order is listed with correct Order ID and status
143. Click on "Sign out" button
144. Verify that the user is logged out successfully
145. Verify that the user is redirected to the homepage in a logged-out state

Your thoughts:-
What you felt Suitable:- The AI version explicitly verifies the post-logout state (redirected to homepage, logged-out), while my manual note just said "user is getting logout" — the AI phrasing is more precise about what "success" actually means here.

What you felt Not suitable:- The AI version assumes an order will always exist to check in "My Orders" — it doesn't account for what should happen if no order was placed yet (e.g. an empty-state message), which is something I'd only think to test by using the account fresh.

Final Test Case:- (AI + Manual, Combined, Automation Ready)
Final Test Case_007 — Order History & Sign Out (Automation Ready)
146. Click on "Account" link and open the "My Orders" tab
147. Verify that the recently placed order is listed with correct Order ID and status
148. Click on "Sign out" button
149. Verify that the user is logged out and redirected to the homepage in a logged-out state
150. Verify that the user is logged in successfully and redirected to the Account page

