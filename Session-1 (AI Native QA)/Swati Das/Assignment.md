
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
