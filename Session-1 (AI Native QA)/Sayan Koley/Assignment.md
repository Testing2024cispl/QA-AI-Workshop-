
---

**Member - Sayan Koley**

## Section 1: Human Thinking — Manual Test Cases

### POSITIVE TEST SCENARIOS

#### TC_POS_01 View product inventory

1. Navigate to https://grocerystoredemo.pcubeweb.com/
2. Observe all listed products across categories.
3. Verify product details like name, description, price.
4. All products should display correctly.

#### TC_POS_02 Add single product to cart

1. Navigate to homepage.
2. Click ADD button next to any product.
3. Observe the cart icon in the header.
4. Cart count should increase by 1 and product should be in cart.

#### TC_POS_03 Add multiple products to cart

1. Navigate to homepage.
2. Click ADD for 3 different products across categories.
3. Click the cart icon to open the cart page.
4. Cart should display all 3 products with correct names and prices.

#### TC_POS_04 Remove product from cart

1. Add 2 products to cart.
2. Open cart page.
3. Remove one product using the remove/delete option.
4. Removed product should disappear; remaining product should still be visible.

#### TC_POS_05 Remove all products from cart

1. Add products to cart.
2. Open cart page.
3. Remove all products one by one.
4. All products should be removed and cart should show empty state with ₹0 total.

#### TC_POS_06 Increase product quantity in cart

1. Add a product to cart.
2. Open cart page.
3. Click the + button to increase quantity of the item.
4. Quantity should increment and cart total should update accordingly.

#### TC_POS_07 Decrease product quantity in cart

1. Add a product to cart with quantity > 1.
2. Open cart.
3. Click the − button once.
4. Quantity should decrease by 1 and subtotal should update.

#### TC_POS_08 Verify cart total calculation

1. Add multiple products to cart (e.g., ₹48 + ₹30).
2. Open cart page.
3. Note the subtotal displayed.
4. Cart total should be sum of (unit price × quantity) for all items.

#### TC_POS_09 Sort products by price low to high

1. Navigate to homepage.
2. Click the Sort By dropdown.
3. Select 'Price low to high'.
4. Products within each section should reorder from lowest to highest price.

#### TC_POS_10 Sort products by price high to low

1. Navigate to homepage.
2. Click the Sort By dropdown.
3. Select 'Price high to low'.
4. Products should reorder from highest to lowest price.

#### TC_POS_11 Sort products by Discount

1. Navigate to homepage.
2. Click Sort By dropdown.
3. Select 'Discount'.
4. Products with highest discount percentage should appear first.

#### TC_POS_12 Search for a product by name

1. Click the search bar at the top.
2. Type 'Cadbury'.
3. Observe search results.
4. All Cadbury products available in the store should appear in results.

#### TC_POS_13 Navigate to a category page

1. Navigate to homepage.
2. Click on a category banner (e.g., Biscuits & Snacks).
3. Observe products listed under that category.
4. Only products belonging to the selected category should be displayed.

#### TC_POS_14 View all products in a category via 'View All'

1. On homepage, locate a category section.
2. Click 'View all' link next to category name.
3. Observe the full category listing page.
4. All products under that category should be listed on the category page.

#### TC_POS_15 Add product to cart from product detail page

1. Open a product detail page.
2. Click Add to Cart button on the detail page.
3. Observe cart badge count.
4. Cart count should increase and product should appear in cart.

#### TC_POS_16 View product detail page

1. Navigate to homepage or category page.
2. Click on any product card.
3. Observe the product detail page.
4. Product name, image, price, and Add to Cart button should be visible.

#### TC_POS_17 Add product to wishlist

1. Navigate to a product detail page.
2. Click the wishlist/heart icon on the product.
3. Navigate to My Wishlist page from the menu.
4. Product should appear in the wishlist page.

#### TC_POS_18 View wishlist page

1. Navigate to /wishlist URL.
2. Observe the wishlist section.
3. (continued)
4. Wishlist page should load and show saved products or an empty state message.

#### TC_POS_19 User sign-in via OTP

1. Click Account from navigation.
2. Enter a valid Indian mobile number (+91XXXXXXXXXX).
3. Click Send OTP.
4. Enter the OTP received and click Verify.
5. User should be logged in and account section should reflect authenticated state.

#### TC_POS_20 Navigate from category back to home

1. Navigate to a category page.
2. Click the Home link in breadcrumb or navigation.
3. Observe the landing page.
4. User should return to homepage with all categories and products visible.

### NEGATIVE TEST SCENARIOS

#### TC_NEG_01 Open cart without adding any product

1. Navigate to homepage without logging in.
2. Click cart icon without adding any item.
3. Observe cart page.
4. Cart should display empty state with ₹0 total or an appropriate empty message.

#### TC_NEG_02 Search with a non-existent product name

1. Click the search bar.
2. Type a random string like 'xyzabc999'.
3. Observe results.
4. No results found message should display; no crash or incorrect results.

#### TC_NEG_03 Sign-in with invalid mobile number (less than 10 digits)

1. Click Account/Sign in.
2. Enter a 5-digit number.
3. Click Send OTP.
4. OTP should not be sent; an error/validation message should appear for invalid number.

#### TC_NEG_04 Sign-in with empty mobile number field

1. Click Account/Sign in.
2. Leave mobile number blank.
3. Click Send OTP.
4. Form should not submit; validation error should prompt user to enter a number.

#### TC_NEG_05 Enter wrong OTP during sign-in

1. Enter a valid mobile number.
2. Click Send OTP.
3. Enter an incorrect OTP.
4. Click Verify.
5. Login should fail with an error like 'Invalid OTP' or 'Incorrect code'.

#### TC_NEG_06 Attempt checkout without being logged in

1. Add product to cart.
2. Open cart.
3. Click Checkout or proceed to order.
4. Observe behavior.
5. User should be prompted to sign in before proceeding to checkout.

#### TC_NEG_07 Decrease product quantity below 1

1. Add a product to cart.
2. Open cart.
3. Click − button when quantity is already 1.
4. Product should either be removed from cart or quantity should not go below 1.

#### TC_NEG_08 Navigate to a non-existent category URL

1. Manually type an invalid category URL: /categories/invalid-category.
2. Press Enter.
3. Observe page behavior.
4. A 404 page or 'No products found' message should display; no application crash.

#### TC_NEG_09 Submit OTP form with alphabets instead of digits

1. Click Account/Sign in.
2. Type alphabets in the mobile number field.
3. Click Send OTP.
4. Input should be rejected or not accepted; only numeric characters should be allowed.

#### TC_NEG_10 Add same product multiple times from homepage

1. Click ADD for the same product twice in quick succession.
2. Open cart.
3. Observe quantity.
4. Cart should show quantity 2 for that product, not two separate line items.

#### TC_NEG_11 Access wishlist without logging in

1. Navigate to /wishlist without authentication.
2. Observe page behavior.
3. (continued)
4. Either redirect to sign-in, or show empty wishlist without crashing.

#### TC_NEG_12 Proceed to order when store is not accepting orders

1. Add products to cart.
2. Click Checkout/Proceed.
3. Observe the 'Sorry we're currently not accepting orders' banner.
4. A clear message should block the order. No order should be placed silently.

#### TC_NEG_13 Search with only whitespace characters

1. Click the search bar.
2. Press spacebar multiple times without typing any letter.
3. Observe search results.
4. Search should not return all products; an empty result or 'No products found' message should display.

#### TC_NEG_14 Search with special characters

1. Click the search bar.
2. Type '!@#$%^&*' in the search field.
3. Observe the results.
4. No crash or unhandled error; page should either show empty results or handle the input gracefully.

#### TC_NEG_15 Rapid multiple clicks on ADD button for same product

1. Locate any product on homepage.
2. Click the ADD button rapidly 5 or more times.
3. Open cart and check item quantity.
4. Quantity should reflect actual additions; no UI freeze, duplicate entries, or count mismatch should occur.

#### TC_NEG_16 Remove all products from cart then verify empty state

1. Add multiple products to cart.
2. Open cart page.
3. Remove all products one by one.
4. Observe final cart state.
5. Cart should show empty state message and ₹0 total; no ghost line items or stale totals should remain.

#### TC_NEG_17 Mobile number with more than 10 digits at sign-in

1. Click Account/Sign in.
2. Enter an 11-digit mobile number.
3. Click Send OTP.
4. Field should reject extra digits or display a validation error; OTP should not be dispatched.

#### TC_NEG_18 Navigate to non-existent product detail URL

1. Type a fabricated product URL directly in browser: /products/fake-product-xyz.
2. Press Enter and observe.
3. (continued)
4. Application should show a 404 or redirect to homepage; no raw error stack or blank page should be shown.

---

## Section 2: AI Model Thinking — Generated Test Cases

### Positive Test Scenarios

| Test Case ID | Scenario | Steps | Expected Result |
|---|---|---|---|
| TC_POS_01 | Homepage loads with all category sections | Navigate to https://grocerystoredemo.pcubeweb.com/, Wait for full page load, Observe presence of category sections | Page should load all category sections: Biscuits & Snacks, Chocolates & Candies, Pooja Essentials, Bread & Bakery, etc. |
| TC_POS_02 | Category banner navigation works | On homepage, click a category banner image, Observe redirection, Verify URL matches category slug | User should land on /categories/biscuits-snacks with relevant products listed |
| TC_POS_03 | Product card displays correct data | Navigate to homepage, Locate any product card, Observe name and price on the card | Product name and price should match expected catalog data |
| TC_POS_04 | Sort by Featured (default state) | Click Sort By dropdown, Select 'Featured', Observe product order | Products should render in their default/featured order as set by the store |
| TC_POS_05 | Sort by Price Low to High | Click Sort By dropdown, Select 'Price low to high', Observe product order | Products should be reordered from lowest price to highest within each section |
| TC_POS_06 | Sort by Price High to Low | Click Sort By dropdown, Select 'Price high to low' | Products should be reordered from highest price to lowest |
| TC_POS_07 | Sort by Discount | Click Sort By dropdown, Select 'Discount', Observe product ordering | Products with highest discount should appear at the top of the list |
| TC_POS_08 | Add product to cart from homepage | Find any product on homepage with an ADD button, Click ADD, Check the cart badge count | Cart badge should update from 0 to 1 (or increment if already non-zero) |
| TC_POS_09 | Cart persists added products | Add 2 products to cart, Navigate to a different page, Return to cart via cart icon | Both previously added products should still be present in the cart |
| TC_POS_10 | Cart shows correct per-item price | Add a product, Open cart page, Verify price displayed next to item | Price displayed in cart should match the product price on the homepage |

---

## Section 3: My Thoughts

### What I Felt Suitable

- AI generation was effective at producing broad coverage quickly — sorting variations, cart state persistence, and URL boundary conditions were well handled with minimal manual effort.
- The systematic approach of AI helped ensure no major functional flow was missed — homepage load, category navigation, product detail, cart CRUD, search, wishlist, and auth were all covered.
- AI-generated negative cases for input boundaries are reliable and repeatable, making them automation-friendly out of the box.
- Human thinking added real observational value for this specific site.
- Combining both approaches produced a more complete and practical test suite than either alone would deliver.

### What I Felt Not Suitable

- Some AI-generated scenarios are assumption-based.
- AI missed the product review/rating submission flow entirely.
- A few AI positive cases overlap in intent.
- Human thinking leaned too heavily on auth-related cases.
- Neither thinking approach covered the 'Similar Products' section comprehensively.

---

## Section 4: Final Test Cases (AI + Manual Combined — Automation Ready)

| Test Case ID | Classification | Scenario | Steps to Reproduce | Priority | Severity |
|---|---|---|---|---|---|
| TC_01 | Positive | View product listing on homepage | Navigate to https://grocerystoredemo.pcubeweb.com/, Wait for all category sections to load, Verify product name and price are visible on each card | High | Critical |
| TC_02 | Positive | Navigate to category page via banner | Click a category banner on homepage, Observe URL and product listing | High | Critical |
| TC_03 | Positive | View product detail page | Click on any product card, Observe product detail page | High | Critical |
| TC_04 | Positive | Sort products by Price Low to High | Click Sort By dropdown, Select 'Price low to high', Observe product order | Medium | Major |
| TC_05 | Positive | Sort products by Price High to Low | Click Sort By dropdown, Select 'Price high to low', Observe product order | Medium | Major |
| TC_06 | Positive | Sort products by Discount | Click Sort By dropdown, Select 'Discount', Observe product order | Medium | Major |
| TC_07 | Positive | Add single product to cart from homepage | Click ADD next to any product, Observe cart badge count | High | Critical |
| TC_08 | Positive | Add multiple products to cart | Click ADD for 3 different products, Open cart page, Observe items | High | Critical |
| TC_09 | Positive | Increase product quantity in cart | Add a product to cart, Open cart, Click + to increase quantity | High | Major |
| TC_10 | Positive | Decrease product quantity in cart | Add a product with qty > 1, Open cart, Click − in cart | High | Major |
| TC_11 | Positive | Remove product from cart | Add 2 products, Remove one via the remove option, Observe cart | High | Critical |
| TC_12 | Positive | Verify cart total calculation | Add multiple products, Open cart, Check displayed subtotal | High | Critical |
| TC_13 | Positive | Search for product by keyword | Click search bar, Type 'Cadbury', Observe results | High | Critical |
| TC_14 | Positive | View all products in a category | Click 'View all' on any category section, Observe category page | Medium | Major |
| TC_15 | Positive | Add product to wishlist | Open product detail page, Click wishlist/heart icon, Navigate to /wishlist | Medium | Minor |
| TC_16 | Positive | Sign-in via OTP — happy path | Click Account, Enter valid 10-digit mobile, Click Send OTP, Enter OTP, Click Verify | High | Critical |
| TC_17 | Positive | Cart badge reflects correct count after multiple adds | Add 4 products one by one, Observe cart badge after each add | Medium | Major |
| TC_18 | Positive | Breadcrumb navigation on product detail page | Open a product via category, Click category name in breadcrumb | Medium | Minor |
| TC_19 | Positive | Store locator page loads | Click Store locator in navigation | Low | Minor |
| TC_20 | Positive | Remove all items from cart — empty state | Add 2 products, Remove all items, Observe cart | Medium | Major |
| TC_21 | Negative | Open cart without adding any product | Navigate to site, Click cart icon without adding items | Medium | Minor |
| TC_22 | Negative | Checkout blocked when store not accepting orders | Add product to cart, Proceed to checkout, Observe store not accepting orders state | High | Critical |
| TC_23 | Negative | Sign-in with fewer than 10 digits | Click Account, Enter a 5-digit number, Click Send OTP | High | Major |
| TC_24 | Negative | Sign-in with empty mobile number | Open sign-in modal, Leave field blank, Click Send OTP | High | Major |
| TC_25 | Negative | Sign-in with alphabets in mobile field | Enter alphabets in mobile number field, Click Send OTP | High | Major |
| TC_26 | Negative | Wrong OTP submission | Enter valid number, request OTP, Enter wrong OTP, Click Verify | High | Major |
| TC_27 | Negative | Decrease quantity below 1 in cart | Add product to cart, Click − when quantity is already 1 | Medium | Major |
| TC_28 | Negative | Search with special characters | Click search bar, Type '!@#$%', Observe results | Medium | Minor |
| TC_29 | Negative | Search with only whitespace | Click search bar, Type only spaces, Observe results | Medium | Minor |
| TC_30 | Negative | Access non-existent product URL directly | Navigate to /products/fake-product-xyz | Low | Minor |
| TC_31 | Negative | Rapid multiple ADD clicks on same product | Click ADD for same product 5+ times rapidly, Open cart | Medium | Major |
| TC_32 | Negative | Access wishlist without logging in | Navigate to /wishlist without authentication | Low | Minor |

---
