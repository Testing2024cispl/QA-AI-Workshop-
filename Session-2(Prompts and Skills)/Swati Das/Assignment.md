
---
 
**Member:** Swati Das
 
## Section 1: Human Thinking — Manual Test Cases
*Written from a tester's perspective: real user journeys, edge cases observed through application exploration, domain intuition, and state validation.*
 
### POSITIVE TEST SCENARIOS
 
**TC_POS_01 View product inventory**
* Navigate to `https://www.saucedemo.com/` and log in with valid credentials (`standard_user`).
* Observe all listed products on the inventory page.
* Verify product details like name, description, price, and images.
* *Expected Result:* All 6 default items should display correctly with accurate prices, high-quality images, and specific descriptions.
 
**TC_POS_02 Add single product to cart from inventory page**
* Log in and navigate to the homepage/inventory page.
* Click the "Add to cart" button next to the "Sauce Labs Backpack".
* Observe the cart icon badge in the upper right header.
* *Expected Result:* The cart badge count should increase to `1`, and the button text should change from "Add to cart" to "Remove".
 
**TC_POS_03 Add multiple products to cart**
* Log in and navigate to the inventory page.
* Click "Add to cart" for 3 different items (Backpack, Bike Light, Bolt T-Shirt).
* Click the cart icon to open the cart page.
* *Expected Result:* The cart badge should display `3`. The cart page should accurately list all 3 distinct products with their respective names and prices.
 
**TC_POS_04 Remove product from cart via inventory page**
* Log in and add the "Sauce Labs Backpack" to the cart.
* Click the "Remove" button directly on the inventory page for that same item.
* Observe the cart icon badge.
* *Expected Result:* The cart badge should decrease by 1 (or disappear if it was the only item), and the button text should change back to "Add to cart".
 
**TC_POS_05 Remove product from inside the cart page**
* Add 2 items to the cart and click the cart icon to navigate to `/cart.html`.
* Click the "Remove" button next to one of the items.
* *Expected Result:* The selected item should instantly disappear from the cart list, and the cart badge count in the header should decrease to `1`.
 
**TC_POS_06 View product detail page**
* Log in and click on the title link "Sauce Labs Fleece Jacket".
* Observe the product page layout and elements.
* *Expected Result:* User should be redirected to `/inventory-item.html?id=4` displaying a large high-resolution image, title, detailed description, price, and an "Add to cart" button.
 
**TC_POS_07 Add product to cart from product detail page**
* Navigate to the item detail page for "Sauce Labs Onesie".
* Click the "Add to cart" button on this detail page.
* Observe the cart badge count.
* *Expected Result:* Cart count badge should update to `1`, and the button should dynamically toggle to "Remove".
 
**TC_POS_08 Navigate from product detail page back to inventory**
* Open any product detail page.
* Click the "Back to products" secondary navigation link.
* *Expected Result:* The user should successfully return to `/inventory.html` with the scroll position preserved or reset gracefully, showing all available catalog items.
 
**TC_POS_09 Sort products by Name (A to Z)**
* Click the product sort container dropdown in the top-right.
* Select 'Name (A to Z)'.
* *Expected Result:* Items should re-order alphabetically by title starting with "Sauce Labs Backpack" and ending with "Test.allTheThings() T-Shirt (Red)".
 
**TC_POS_10 Sort products by Name (Z to A)**
* Click the product sort container dropdown.
* Select 'Name (Z to A)'.
* *Expected Result:* Items should immediately invert order, listing "Test.allTheThings() T-Shirt (Red)" at the top and "Sauce Labs Backpack" at the bottom.
 
**TC_POS_11 Sort products by Price (low to high)**
* Click the product sort container dropdown.
* Select 'Price (low to high)'.
* *Expected Result:* The item cards should re-arrange dynamically from the lowest price item ($7.99) to the highest price item ($49.99).
 
**TC_POS_12 Sort products by Price (high to low)**
* Click the product sort container dropdown.
* Select 'Price (high to low)'.
* *Expected Result:* The item cards should re-arrange dynamically starting from the highest price item ($49.99) down to the lowest ($7.99).
 
**TC_POS_13 Complete full checkout workflow with single item**
* Add an item to the cart, navigate to `/cart.html`, and click "Checkout".
* Fill in First Name, Last Name, and Postal Code on `/checkout-step-one.html` and click "Continue".
* Review the item total, tax calculation, and final total on `/checkout-step-two.html`. Click "Finish".
* *Expected Result:* User should hit `/checkout-complete.html` showing a "Thank you for your order!" success message.
 
**TC_POS_14 Verify tax application in checkout total overview**
* Add multiple items with different price points to the cart.
* Complete Step 1 of Checkout and proceed to Step 2 (Overview).
* Formulate mathematical check: `Item total + Tax = Total`.
* *Expected Result:* The calculated tax percentage must be applied to the subtotal correctly, and the total must mathematically equal the item total plus the displayed tax.
 
**TC_POS_15 Sidebar menu expanding and collapsing**
* Click the burger menu icon (`bm-burger-button`) on the top left.
* Observe the menu slide out. Click the "X" close button (`react-burger-cross-btn`).
* *Expected Result:* The navigation sidebar should open cleanly revealing "All Items", "About", "Logout", and "Reset App State". Clicking close should hide it completely without breaking main page layouts.
 
**TC_POS_16 User logout**
* Open the sidebar menu from the inventory dashboard.
* Click the "Logout" option link.
* *Expected Result:* The user session should terminate immediately, redirecting back to `https://www.saucedemo.com/` with all fields cleared.
 
**TC_POS_17 Reset application state via sidebar menu**
* Add 3 items to your shopping cart (badge displays `3`).
* Open the sidebar menu and click "Reset App State".
* Close the sidebar or observe the background cart badge.
* *Expected Result:* The application session storage state should reset immediately; the cart badge must clear back to empty, and all "Remove" buttons should revert to "Add to cart".
 
**TC_POS_18 Login with unique valid persona profiles**
* Authenticate sequentially using profiles: `problem_user`, `performance_glitch_user`, `error_user`, and `visual_user`.
* *Expected Result:* Login should succeed for all profiles; unique functional traits mapped to these profiles (e.g., specific broken images or delayed loading) should manifest without system crashes.
 
---
 
### NEGATIVE TEST SCENARIOS
 
**TC_NEG_01 Login with invalid credentials**
* Type `invalid_user` into Username and `wrong_sauce` into Password. Click "Login".
* *Expected Result:* Authentication blocks, and a clear error message is displayed: *"Epic sadface: Username and password do not match any user in this service"*.
 
**TC_NEG_02 Login with empty username field**
* Leave the Username input field blank, enter `secret_sauce` into Password, and click "Login".
* *Expected Result:* Login fails with inline validation text: *"Epic sadface: Username is required"*.
 
**TC_NEG_03 Login with empty password field**
* Enter `standard_user` into Username, leave the Password field completely blank, and click "Login".
* *Expected Result:* Login fails with inline validation text: *"Epic sadface: Password is required"*.
 
**TC_NEG_04 Direct URL access to secure pages without login session**
* Clear browser cookies/session storage or open an incognito window.
* Attempt to navigate directly to `https://www.saucedemo.com/inventory.html` or `https://www.saucedemo.com/cart.html`.
* *Expected Result:* Access is strictly blocked; the application redirects user to the root login index page displaying a validation message: *"Epic sadface: You can only access '/inventory.html' after logging in"*.
 
**TC_NEG_05 Submit Checkout Step 1 with empty First Name**
* Proceed to checkout with items in the cart.
* Leave "First Name" blank, fill out "Last Name" and "Zip/Postal Code". Click "Continue".
* *Expected Result:* Form validation blocks transition, highlighting the error: *"Error: First Name is required"*.
 
**TC_NEG_06 Submit Checkout Step 1 with empty Last Name**
* Enter "Jane" in First Name, leave "Last Name" blank, and provide a Zip/Postal Code. Click "Continue".
* *Expected Result:* Form validation blocks transition, highlighting the error: *"Error: Last Name is required"*.
 
**TC_NEG_07 Submit Checkout Step 1 with empty Zip/Postal Code**
* Enter "Jane" in First Name, "Doe" in Last Name, and leave "Zip/Postal Code" completely blank. Click "Continue".
* *Expected Result:* Form validation blocks transition, highlighting the error: *"Error: Postal Code is required"*.
 
**TC_NEG_08 Navigate to a completely non-existent system sub-URL**
* Log in, then manually append a random path to the browser address bar: `https://www.saucedemo.com/non-existent-page`. Press Enter.
* *Expected Result:* The application UI gracefully catches the routing error (either displaying a custom clean 404 container or redirecting cleanly without showing raw stack traces).
 
---
 
## Section 2: AI Model Thinking — Generated Test Cases
*Generated by systematically analyzing strict DOM properties, form data states, URL transitions, and state boundary configurations.*
 
| Test Case ID | Scenario | Steps | Expected Result |
| :--- | :--- | :--- | :--- |
| **TC_AI_01** | Root URL loading state and structural landing components verification | Navigate to `https://www.saucedemo.com/`, monitor network state completion, and observe standard DOM nodes. | Page load finishes with status `200`. Main input IDs `#user-name` and `#password` are interactive and visible in viewport. |
| **TC_AI_02** | HTML state mapping post-successful login validation | Type `standard_user`, input `secret_sauce`, click input submit node `#login-button`. Verify active window path. | Browser session initializes state, location path shifts seamlessly to `/inventory.html`, element `.title` resolves to "Products". |
| **TC_AI_03** | Sequential structural validation of full inventory listing grid | Log in, locate structural parent container element `.inventory_list`, evaluate child structural components `.inventory_item`. | Total collection length exactly matches integer value `6`. Every nested unit contains title, image element, price prefix, and toggle button wrapper. |
| **TC_AI_04** | Dynamic class property modifications on item selection | Navigate to `/inventory.html`, click first occurring target button sequence `.btn_primary.btn_inventory`. | The exact clicked button node transforms its structural state properties: class shifts to `.btn_secondary.btn_inventory` and labels text as "Remove". |
| **TC_AI_05** | Cart storage item count synchronization accuracy check | Add 2 items, click element link `.shopping_cart_link`. Check textual data of badge DOM entity `.shopping_cart_badge`. | String literal within `.shopping_cart_badge` parses precisely to integer structural equivalent value `2`. |
| **TC_AI_06** | Browser history tracking and backward action verification | Log in, move sequentially from `/inventory.html` down into `/cart.html`. Invoke native browser back action via window control. | Current state shifts back to `/inventory.html` securely. Item configurations and selection choices remain structurally locked. |
| **TC_AI_07** | State retention during browser screen refresh actions | Put 1 item in cart. Execute native webpage hard reload action (`Ctrl + F5` or window environment refresh). | Session preserves configuration data; shopping cart state badge maintains integrity showing value `1`. |
| **TC_AI_08** | Interrupted checkout pipeline termination processing | Add items to cart, select checkout option, progress into `/checkout-step-one.html`, click cancel control element `#cancel`. | Form values drop cleanly, current window location instantly routes backwards back into the prior `/cart.html` index view. |
| **TC_AI_09** | Empty data profile validation handling during checkout start | Navigate directly to empty cart array layout `/cart.html`. Trigger transition click via element `#checkout`. | Application loads step 1 profile fields. *(Note: SauceDemo native application parameters permit step 1 processing on empty state arrays).* |
| **TC_AI_10** | Error close control item action handler dismissals | Input invalid character combinations into login. Generate visible error message banner `.error-message-container`. Click `.error-button`. | Target class node container `.error-message-container` deletes its visible state layout or returns cleanly to hidden status attributes. |
 
---
 
## Section 3: My Thoughts
 
### What I Felt Suitable
* **AI Speed on Schema & Data State Inversions:** The AI model is highly systematic at scanning basic form inputs, tracking ID fields, and laying down clear boundary parameter matrices (like field-by-field validation tracking for step-one checkouts).
* **Human Discovery of Process Flows:** Human intuition excels at mapping edge workflows that aren't obvious from looking at a single form—such as the explicit operation of the "Reset App State" menu option combined with checking items on the background page, or handling user personas like `locked_out_user`.
* **Deduplication Synergy:** Merging both approaches yields an enterprise-grade suite where automation paths (CSS selectors from AI) combine with exploratory workflows (Human edge cases).
 
### What I Felt Not Suitable
* **AI Context blindspots:** The AI sometimes misses UI nuances, like noticing if product images are mismatched or broken (which happens specifically under the `problem_user` configuration). It tests structure, whereas humans test contextual visual correctness.
* **Human Structural Omissions:** Manual test script drafting easily misses systematic browser execution checks, like confirming explicit hard refresh preservation rules or backward browser history actions.
 
---
 
## Section 4: Final Test Cases (AI + Manual Combined — Automation Ready)
*Deduplicated, merged, prioritized, and augmented with automated selectors for test framework implementation.*
 
| Test Case ID | Classification | Scenario | Steps to Reproduce | Priority | Severity |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **TC_01** | Positive | Verify successful login with standard user profile | 1. Navigate to URL.<br>2. Input `standard_user` in `#user-name`.<br>3. Input `secret_sauce` in `#password`.<br>4. Click `#login-button`. | High | Critical |
| **TC_02** | Positive | View full product listing grid details on inventory load | 1. Log in to system.<br>2. Verify URL is on `/inventory.html`.<br>3. Inspect `.inventory_item` nodes for image, title, price, and add button. | High | Critical |
| **TC_03** | Positive | Add single item to cart from home catalog layout | 1. Log in to system.<br>2. Click first button item `.btn_primary.btn_inventory`.<br>3. Evaluate `.shopping_cart_badge` element string contents. | High | Critical |
| **TC_04** | Positive | Add multiple items to cart and check data persistence | 1. Add 3 distinct items across inventory list grid.<br>2. Verify cart badge displays `3`.<br>3. Navigate directly into `/cart.html` view. | High | Critical |
| **TC_05** | Positive | Remove product item choice from inside cart view | 1. Add item to cart.<br>2. Navigate into cart page view via `.shopping_cart_link`.<br>3. Click the target item row button selection labeled `.btn_secondary.cart_button`. | High | Major |
| **TC_06** | Positive | Review single product specification details card | 1. Log in successfully.<br>2. Click primary title link element `.inventory_item_name` for an item.<br>3. Verify redirection to `/inventory-item.html?id=*`. | Medium | Major |
| **TC_07** | Positive | Sort items alphabetically: Name (A to Z) | 1. Locate sort dropdown menu element `.product_sort_container`.<br>2. Click and pick entry variable option code `az`.<br>3. Verify title order sorting arrays. | Medium | Minor |
| **TC_08** | Positive | Sort items alphabetically: Name (Z to A) | 1. Locate sort dropdown menu element `.product_sort_container`.<br>2. Click and pick entry variable option code `za`.<br>3. Verify title order sorting arrays. | Medium | Minor |
| **TC_09** | Positive | Sort item lists by numerical value: Price (low to high) | 1. Locate sort dropdown menu element `.product_sort_container`.<br>2. Click and pick entry variable option code `lohi`.<br>3. Check price sequence ascending state. | Medium | Major |
| **TC_10** | Positive | Sort item lists by numerical value: Price (high to low) | 1. Locate sort dropdown menu element `.product_sort_container`.<br>2. Click and pick entry variable option code `hilo`.<br>3. Check price sequence descending state. | Medium | Major |
| **TC_11** | Positive | Execute end-to-end checkout pipeline confirmation sequence | 1. Add item to cart -> Proceed to `/cart.html` -> Click `#checkout`.<br>2. Populate fields `#first-name`, `#last-name`, `#postal-code`. Click `#continue`.<br>3. Check overview details. Click `#finish`. | High | Critical |
| **TC_12** | Positive | Validate app state reset function parameters via menu | 1. Add 2 items into cart array layout.<br>2. Trigger sidebar toggle action `#react-burger-menu-btn`.<br>3. Choose link `#reset_sidebar_link`. Check cart. | High | Major |
| **TC_13** | Positive | Execute session termination logout sequence | 1. Trigger sidebar toggle action `#react-burger-menu-btn`.<br>2. Click menu interaction endpoint `#logout_sidebar_link`.<br>3. Verify routing back to login page. | High | Critical |
| **TC_14** | Positive | Retain active session selection parameters across manual refresh | 1. Add item into cart layout space.<br>2. Execute native system browser reload instruction script command.<br>3. Check if card state and badge retain data value `1`. | Medium | Major |
| **TC_15** | Negative | Attempt access with invalid credential profile pairing | 1. Type input values `invalid_user` and `wrong_sauce` on login form entries.<br>2. Trigger click behavior handler action item `#login-button`. | High | Major |
| **TC_16** | Negative | Missing field constraint checking: Blank Username entry validation | 1. Leave `#user-name` entry empty. Populate `#password` field entry values.<br>2. Click `#login-button`. Inspect error banner message. | High | Major |
| **TC_17** | Negative | Missing field constraint checking: Blank Password entry validation | 1. Populate `#user-name` data field entries. Leave `#password` completely empty.<br>2. Click `#login-button`. Inspect error banner message. | High | Major |
| **TC_18** | Negative | Enforce platform perimeter security against unauthenticated route access | 1. Clear session cookies entirely.<br>2. Request manual browser entry mapping destination route `/inventory.html`.<br>3. Verify redirection back to index. | High | Critical |
| **TC_19** | Negative | Profile missing checkout data constraints: First Name absent checks | 1. Go to checkout step 1 form.<br>2. Leave `#first-name` blank. Fill `#last-name` and `#postal-code`.<br>3. Click input element button action `#continue`. | High | Major |
| **TC_20** | Negative | Profile missing checkout data constraints: Last Name absent checks | 1. Go to checkout step 1 form.<br>2. Fill `#first-name`. Leave `#last-name` blank. Fill `#postal-code`.<br>3. Click input element button action `#continue`. | High | Major |
| **TC_21** | Negative | Profile missing checkout data constraints: Postal Code absent checks | 1. Go to checkout step 1 form.<br>2. Fill `#first-name` and `#last-name`. Leave `#postal-code` blank.<br>3. Click input element button action `#continue`. | High | Major |
| **TC_22** | Negative | Dismiss active warning banners via error close control points | 1. Generate active error container state message panel view.<br>2. Click close toggle button vector entity `.error-button`.<br>3. Verify structural closure state. | Medium | Minor |

---

=====================================================================================
# skill.md
=====================================================================================

# SKILL: Manual Functional Test Case Generator — Swag Labs (SauceDemo)

## Overview

This skill guides the generation of **manual functional test cases only** for the Swag Labs e-commerce demo application at [https://www.saucedemo.com](https://www.saucedemo.com). All test cases must be functional in nature. Non-functional testing (performance, load, security, accessibility, usability benchmarking) and automation scripts are **explicitly out of scope**.

---

## Application Summary

Swag Labs is a React.js-based e-commerce demo application. It simulates an online shopping experience with the following key modules:

- Login / Authentication
- Product Inventory (listing, sorting, product detail)
- Shopping Cart (add, remove, badge count)
- Checkout (step 1: information, step 2: overview, confirmation)
- Navigation Menu (hamburger menu: logout, reset app state, about, all items)
- Session Management (auto-logout after ~10 minutes)

---

## Known User Credentials

| Username               | Password      | Behavior                                                    |
|------------------------|---------------|-------------------------------------------------------------|
| `standard_user`        | `secret_sauce` | Full happy-path workflow works correctly                    |
| `locked_out_user`      | `secret_sauce` | Login blocked with error message                            |
| `problem_user`         | `secret_sauce` | Logs in; UI bugs present (wrong images, last name errors)   |
| `performance_glitch_user` | `secret_sauce` | Logs in with deliberate delay on login                   |
| `error_user`           | `secret_sauce` | Random UI/functional errors during interactions             |
| `visual_user`          | `secret_sauce` | Logs in; visual/layout anomalies present                    |

---

## Test Case Structure (Standard Format)

Every generated test case must follow this structure:

```
Test Case ID   : <MODULE>_TC_XXX
Test Case Title: <Short descriptive title>
Module         : <Login | Inventory | Cart | Checkout | Navigation | Session>
Priority       : <P0 – Critical | P1 – High | P2 – Medium | P3 – Low>
Precondition   : <State required before test execution>
Test Steps     :
  1. <Action>
  2. <Action>
  ...
Expected Result: <Observable, verifiable outcome>
Test Data      : <Specific inputs used>
Edge Case Flag : <Yes / No>
```

---

## Module 1: Login / Authentication

### Functional Scenarios

**LOGIN_TC_001** — Valid credentials (standard_user)
- Steps: Navigate to URL → Enter `standard_user` / `secret_sauce` → Click Login
- Expected: User is redirected to `/inventory.html`; "Products" heading visible

**LOGIN_TC_002** — Valid credentials (performance_glitch_user)
- Steps: Enter `performance_glitch_user` / `secret_sauce` → Click Login
- Expected: User lands on inventory page (may take longer than standard_user; this is by design, still should succeed)

**LOGIN_TC_003** — Valid credentials (problem_user)
- Steps: Enter `problem_user` / `secret_sauce` → Click Login
- Expected: User lands on `/inventory.html`

**LOGIN_TC_004** — Valid credentials (error_user)
- Steps: Enter `error_user` / `secret_sauce` → Click Login
- Expected: User lands on `/inventory.html`

**LOGIN_TC_005** — Locked out user
- Steps: Enter `locked_out_user` / `secret_sauce` → Click Login
- Expected: Error displayed: "Epic sadface: Sorry, this user has been locked out."

**LOGIN_TC_006** — Invalid username, valid password
- Steps: Enter `invalid_user` / `secret_sauce` → Click Login
- Expected: Error: "Epic sadface: Username and password do not match any user in this service"

**LOGIN_TC_007** — Valid username, invalid password
- Steps: Enter `standard_user` / `wrong_pass` → Click Login
- Expected: Error: "Username and password do not match any user in this service"

**LOGIN_TC_008** — Empty username field
- Steps: Leave username blank, enter `secret_sauce` → Click Login
- Expected: Error: "Epic sadface: Username is required"

**LOGIN_TC_009** — Empty password field
- Steps: Enter `standard_user`, leave password blank → Click Login
- Expected: Error: "Epic sadface: Password is required"

**LOGIN_TC_010** — Both fields empty
- Steps: Leave both blank → Click Login
- Expected: Error: "Epic sadface: Username is required"

### Edge Cases — Login

**LOGIN_TC_E01** — Username with leading/trailing spaces
- Input: `" standard_user "` / `secret_sauce`
- Expected: Login fails with credential mismatch error (spaces are not trimmed)

**LOGIN_TC_E02** — Password with leading/trailing spaces
- Input: `standard_user` / `" secret_sauce "`
- Expected: Login fails (passwords are case/space sensitive)

**LOGIN_TC_E03** — Username in UPPERCASE
- Input: `STANDARD_USER` / `secret_sauce`
- Expected: Login fails (field is case-sensitive)

**LOGIN_TC_E04** — Password in UPPERCASE
- Input: `standard_user` / `SECRET_SAUCE`
- Expected: Login fails (field is case-sensitive)

**LOGIN_TC_E05** — Username with special characters
- Input: `standard_user!@#` / `secret_sauce`
- Expected: Login fails with mismatch error; no crash

**LOGIN_TC_E06** — Very long username string (255+ characters)
- Input: String of 300 random characters
- Expected: Application handles gracefully; error shown; no page crash

**LOGIN_TC_E07** — SQL injection in username field
- Input: `' OR '1'='1` / `secret_sauce`
- Expected: Login fails; no unintended access; application stable

**LOGIN_TC_E08** — Browser Back button after successful login
- Steps: Login → Navigate to inventory → Click browser Back
- Expected: Redirected back to login page or inventory; no broken state

**LOGIN_TC_E09** — Direct URL access to `/inventory.html` without login
- Steps: Without logging in, navigate directly to `https://www.saucedemo.com/inventory.html`
- Expected: Redirected to login page with message "You can only access '/inventory.html' when you are logged in"

**LOGIN_TC_E10** — Dismiss error message via ✕ icon
- Steps: Trigger any login error → Click the ✕ (close) icon on error banner
- Expected: Error banner dismissed; fields remain with previous input

---

## Module 2: Product Inventory Page

### Functional Scenarios

**INV_TC_001** — Product listing displayed after login
- Expected: 6 products shown on inventory page with name, description, price, image, and "Add to cart" button

**INV_TC_002** — Product image visible for all items
- Expected: Each product has a visible image thumbnail

**INV_TC_003** — Product name is a clickable link
- Steps: Click on a product title
- Expected: Navigates to the product detail page (`/inventory-item.html`)

**INV_TC_004** — Product image is clickable
- Steps: Click on a product image
- Expected: Navigates to the product detail page

**INV_TC_005** — Add to Cart from inventory page
- Steps: Click "Add to cart" on any product
- Expected: Button changes to "Remove"; cart badge shows count = 1

**INV_TC_006** — Remove item from inventory page
- Steps: After adding an item, click "Remove"
- Expected: Button reverts to "Add to cart"; cart badge count decrements

**INV_TC_007** — Add multiple items to cart
- Steps: Add 3 different products
- Expected: Cart badge shows 3

**INV_TC_008** — Sort by Name (A → Z)
- Steps: Select "Name (A to Z)" from sort dropdown
- Expected: Products listed alphabetically ascending

**INV_TC_009** — Sort by Name (Z → A)
- Expected: Products listed alphabetically descending

**INV_TC_010** — Sort by Price (Low → High)
- Expected: Products ordered from lowest to highest price

**INV_TC_011** — Sort by Price (High → Low)
- Expected: Products ordered from highest to lowest price

**INV_TC_012** — Product detail page content
- Steps: Click any product
- Expected: Detail page shows name, description, price, image, "Add to cart" button, and "Back to products" link

**INV_TC_013** — Add to cart from product detail page
- Steps: On detail page → Click "Add to cart"
- Expected: Button changes to "Remove"; cart badge = 1

**INV_TC_014** — "Back to products" link on detail page
- Steps: Click "Back to products"
- Expected: Returns to `/inventory.html` with previous cart state preserved

### Edge Cases — Inventory

**INV_TC_E01** — problem_user: Product images
- Steps: Login as `problem_user` → View inventory
- Expected: Note — known bug: some products display wrong images; verify this as a known defect

**INV_TC_E02** — Cart badge not visible when count is 0
- Expected: When no items are in cart, badge icon is not displayed on the cart icon

**INV_TC_E03** — Add same item from inventory and then from detail page
- Steps: Add product from inventory list → Navigate to its detail page → Observe button state
- Expected: Button on detail page already shows "Remove" (state is consistent)

**INV_TC_E04** — Sort resets after navigation
- Steps: Sort by "Price (Low to High)" → Click on a product → Return via Back to Products
- Expected: Verify if sort preference is retained or resets (document actual vs expected behavior)

**INV_TC_E05** — Verify all 6 product prices are correct and match detail page
- Steps: Note each product price on inventory → Open each detail page
- Expected: Prices are consistent between listing and detail pages

**INV_TC_E06** — All 6 "Add to cart" buttons functional
- Steps: Click "Add to cart" for all 6 items
- Expected: Cart badge reads 6; all buttons show "Remove"

---

## Module 3: Shopping Cart

### Functional Scenarios

**CART_TC_001** — Navigate to cart
- Steps: Click cart icon (top right)
- Expected: Navigates to `/cart.html`; displays added items

**CART_TC_002** — Cart displays correct item details
- Expected: Each cart item shows product name, description, quantity = 1, and price

**CART_TC_003** — Remove item from cart page
- Steps: On cart page, click "Remove" for an item
- Expected: Item removed from list; cart badge decrements

**CART_TC_004** — Cart count badge updates in real time
- Expected: Badge reflects current number of items at all times

**CART_TC_005** — Continue Shopping button
- Steps: On cart page, click "Continue Shopping"
- Expected: Returns to inventory page; previously added items still in cart

**CART_TC_006** — Checkout button navigates to step 1
- Steps: On cart page with items, click "Checkout"
- Expected: Navigates to `/checkout-step-one.html`

**CART_TC_007** — Empty cart checkout attempt
- Steps: Navigate to cart with no items → Click "Checkout"
- Expected: Navigates to checkout step 1; verify behavior (should ideally warn or proceed)

**CART_TC_008** — Cart persists across page navigation
- Steps: Add items → Navigate to inventory → Return to cart
- Expected: Items still present in cart

### Edge Cases — Cart

**CART_TC_E01** — Cart state after sorting
- Steps: Add items → Sort inventory → Go to cart
- Expected: Cart contents unchanged regardless of sort applied

**CART_TC_E02** — Direct URL access to `/cart.html` when logged in but cart is empty
- Expected: Cart page shows empty state with "Continue Shopping" and "Checkout" buttons visible

**CART_TC_E03** — Remove all items from cart and verify badge disappears
- Steps: Add 2 items → Go to cart → Remove all → Go back to inventory
- Expected: Cart badge not displayed; inventory shows "Add to cart" for all products

**CART_TC_E04** — Add item to cart, navigate away, return — verify quantity is still 1
- Expected: Quantity does not change to 2 on revisit

**CART_TC_E05** — Cart badge count visibility at exactly 1 item
- Expected: Badge displays "1" not blank or hidden

---

## Module 4: Checkout — Step 1 (Customer Information)

### Functional Scenarios

**CHK1_TC_001** — Valid checkout information entry
- Steps: Enter First Name: "John", Last Name: "Doe", Zip Code: "10000" → Click Continue
- Expected: Navigates to `/checkout-step-two.html`

**CHK1_TC_002** — Leave First Name blank
- Steps: Leave First Name empty, fill Last Name and Zip → Click Continue
- Expected: Error: "Error: First Name is required"

**CHK1_TC_003** — Leave Last Name blank
- Steps: Fill First Name and Zip, leave Last Name empty → Click Continue
- Expected: Error: "Error: Last Name is required"

**CHK1_TC_004** — Leave Zip Code blank
- Steps: Fill First Name and Last Name, leave Zip empty → Click Continue
- Expected: Error: "Error: Postal Code is required"

**CHK1_TC_005** — All three fields blank
- Steps: Click Continue with all fields empty
- Expected: Error: "Error: First Name is required"

**CHK1_TC_006** — Cancel button on step 1
- Steps: On checkout step 1 page → Click "Cancel"
- Expected: Returns to `/cart.html`; cart items still present

### Edge Cases — Checkout Step 1

**CHK1_TC_E01** — Numeric-only First Name
- Input: First Name: "12345", Last Name: "Doe", Zip: "10000"
- Expected: System accepts (no alphabetical validation enforced); proceeds to step 2

**CHK1_TC_E02** — Special characters in name fields
- Input: First Name: "@#John!", Last Name: "Doe$%", Zip: "10000"
- Expected: System should accept or show validation message; no crash

**CHK1_TC_E03** — Very long strings in all fields (100+ characters each)
- Expected: Fields accept or truncate gracefully; no crash; error message if invalid

**CHK1_TC_E04** — Zip code with letters
- Input: Zip: "ABC123"
- Expected: System proceeds (no numeric validation enforced) or shows validation error

**CHK1_TC_E05** — problem_user: Last Name field cannot be modified
- Steps: Login as `problem_user` → Go to checkout step 1 → Attempt to type in Last Name field
- Expected: Known bug — Last Name field clears itself or does not retain input; document as defect

**CHK1_TC_E06** — Dismiss error banner on checkout step 1
- Steps: Trigger a validation error → Click ✕ on error banner
- Expected: Error dismissed; user can re-enter information

**CHK1_TC_E07** — Whitespace-only in First Name
- Input: First Name: "   " (spaces only)
- Expected: Should fail validation with "First Name is required"

---

## Module 5: Checkout — Step 2 (Order Overview)

### Functional Scenarios

**CHK2_TC_001** — Order overview shows correct items
- Expected: All cart items listed with name, quantity = 1, and price

**CHK2_TC_002** — Item subtotal is mathematically correct
- Expected: Subtotal = sum of all individual item prices

**CHK2_TC_003** — Tax is displayed
- Expected: Tax amount visible (calculated at ~8%)

**CHK2_TC_004** — Total = Subtotal + Tax
- Expected: Total price = Item total + Tax; verify arithmetic

**CHK2_TC_005** — Cancel button on step 2
- Steps: Click "Cancel"
- Expected: Returns to inventory page; cart items still preserved

**CHK2_TC_006** — Finish button completes order
- Steps: Click "Finish"
- Expected: Navigates to `/checkout-complete.html`

### Edge Cases — Checkout Step 2

**CHK2_TC_E01** — Price accuracy with multiple items
- Steps: Add 3 items with known prices → Proceed to step 2
- Expected: Each price, subtotal, tax, and total display accurately with no rounding error

**CHK2_TC_E02** — Direct URL access to `/checkout-step-two.html` without completing step 1
- Expected: Redirected to correct page or step 1; no broken state or empty overview shown

**CHK2_TC_E03** — Only 1 item in cart at checkout
- Expected: Overview shows 1 item; subtotal equals that item's price; tax and total correct

---

## Module 6: Checkout — Confirmation

### Functional Scenarios

**CONF_TC_001** — Order confirmation page content
- Expected: "Thank you for your order!" message displayed; Pony Express image visible; "Back Home" button present

**CONF_TC_002** — Back Home button
- Steps: Click "Back Home"
- Expected: Returns to inventory page (`/inventory.html`); cart is empty; badge gone

**CONF_TC_003** — Cart is cleared after successful checkout
- Expected: Cart badge not visible; all products show "Add to cart" again

### Edge Cases — Confirmation

**CONF_TC_E01** — Browser Back from confirmation page
- Steps: After order confirmed → Click browser Back
- Expected: Returns to checkout step 2 (or checkout complete); application stable; no double-order triggered

**CONF_TC_E02** — Refresh on confirmation page
- Steps: After order confirmed → Refresh browser
- Expected: Confirmation page reloads cleanly or redirects; no crash

---

## Module 7: Navigation Menu (Hamburger Menu)

### Functional Scenarios

**NAV_TC_001** — Open hamburger menu
- Steps: Click ☰ icon (top left)
- Expected: Slide-out menu opens with options: All Items, About, Logout, Reset App State

**NAV_TC_002** — "All Items" link
- Steps: Open menu → Click "All Items"
- Expected: Navigates to `/inventory.html`; menu closes

**NAV_TC_003** — "About" link
- Steps: Open menu → Click "About"
- Expected: Navigates to Sauce Labs official website (external page)

**NAV_TC_004** — Logout
- Steps: Open menu → Click "Logout"
- Expected: Session cleared; redirected to login page (`/`)

**NAV_TC_005** — "Reset App State"
- Steps: Add items to cart → Open menu → Click "Reset App State"
- Expected: Cart is emptied; all "Remove" buttons revert to "Add to cart"; badge removed

**NAV_TC_006** — Close menu without selecting
- Steps: Open menu → Click ✕ or click outside menu
- Expected: Menu closes; current page state unchanged

### Edge Cases — Navigation

**NAV_TC_E01** — Logout clears session; back button cannot re-access inventory
- Steps: Logout → Click browser Back
- Expected: Redirected to login page; inventory not accessible without re-authentication

**NAV_TC_E02** — Reset App State resets UI state but does not log out
- Expected: User remains logged in; only cart/button states are reset

**NAV_TC_E03** — Hamburger menu accessible from all pages
- Steps: Check menu availability on inventory, cart, checkout step 1, step 2, and confirmation pages
- Expected: ☰ icon present and functional on all pages

---

## Module 8: Session Management

### Functional Scenarios

**SES_TC_001** — Auto-logout after inactivity (~10 minutes)
- Steps: Login → Remain idle for 10 minutes → Attempt to interact
- Expected: User is logged out; redirected to login page

**SES_TC_002** — Session not shared between tabs (verify independently)
- Steps: Login in Tab A → Open new Tab B manually to `/inventory.html`
- Expected: Tab B reflects same logged-in session (same browser)

**SES_TC_003** — Manual logout clears all session state
- Steps: Add items to cart → Logout → Log back in
- Expected: Cart is empty after fresh login

---

## Test Generation Rules

When generating test cases from this skill, follow these rules strictly:

1. **Scope**: Only manual functional test cases. No automation code, no performance metrics, no security testing.
2. **Format**: Always use the standardized test case format defined above.
3. **Edge Case Flag**: Mark `Edge Case Flag: Yes` for all boundary, negative, and abnormal input scenarios.
4. **User-specific cases**: When a test involves `problem_user` or `error_user`, tag the expected result with `[KNOWN DEFECT]` where applicable.
5. **Priority Assignment**:
   - P0: Core authentication and checkout completion flows
   - P1: Cart operations, navigation, key validations
   - P2: Sorting, product details, session edge cases
   - P3: UI state edge cases, minor behavioral anomalies
6. **No duplication**: Do not regenerate a test case that already exists in a module unless the input data varies meaningfully.
7. **Verifiable expected results**: Every expected result must be observable and verifiable by a human tester without tooling.
8. **One test, one scenario**: Each test case tests exactly one behavior or condition.

---

## Modules and Coverage Summary

| Module              | Happy Path TCs | Edge Case TCs |
|---------------------|---------------|---------------|
| Login               | 10            | 10            |
| Inventory           | 14            | 6             |
| Cart                | 8             | 5             |
| Checkout Step 1     | 6             | 7             |
| Checkout Step 2     | 6             | 3             |
| Confirmation        | 3             | 2             |
| Navigation Menu     | 6             | 3             |
| Session Management  | 3             | 0             |
| **Total**           | **56**        | **36**        |

**Grand Total: 92 manual functional test cases**

---

## Out of Scope (Do NOT Generate)

- Performance/load test cases
- Security/penetration test cases
- Accessibility (WCAG) test cases
- API/network-level test cases
- Any automation scripts or code
- Visual regression test cases
- Cross-browser compatibility test cases
- Database validation test cases
