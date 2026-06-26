
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
=====================================================================================


# skill.md

---
name: grocery-store-demo-test-case-generator
description: >
  Generate manual functional test cases for https://grocerystoredemo.pcubeweb.com/ — a Dukaan-based
  grocery e-commerce demo. Use this skill whenever the user asks to generate, expand, review, or
  stress-test manual test cases for this site. Covers positive flows, negative flows, and edge cases
  across all functional modules: homepage, product catalog, cart, sort/filter, search, wishlist,
  OTP authentication, checkout gate, category navigation, and URL boundary testing.
  Do NOT generate automation scripts, performance tests, or accessibility tests — manual functional only.
---

# Manual Functional Test Case Generator — Grocery Store Demo

## Site Context

**URL:** https://grocerystoredemo.pcubeweb.com/
**Platform:** Dukaan (hosted storefront)
**Currency:** INR (₹)
**Auth method:** OTP via Indian mobile number (+91XXXXXXXXXX)
**Checkout state:** Store may show "currently not accepting orders" banner — this is a known demo constraint, not a bug.

### Confirmed Categories (live as of last fetch)
- Biscuits & Snacks → `/categories/biscuits-snacks`
- Chocolates & Candies → `/categories/chocolates-candies`
- Pooja Essentials → `/categories/pooja-essentials`
- Bread & Bakery → `/categories/bread-bakery`
- Stationary → `/categories/stationary`
- Household & Kitchen Needs → `/categories/household-kitchen-needs`
- Health Care → `/categories/health-care`
- Grocery & Staples → `/categories/grocery-staples`
- Drinking Water → `/categories/drinking-water`
- Beverages → `/categories/beverages`

### Sort Options Available
Featured | Discount | Price low to high | Price high to low

### Key URLs
- Cart: `/grocerystoredemo/bag`
- Wishlist: `/wishlist`
- Store Locator: `/store-locator`
- All Categories: `/categories`

---

## Output Format

Always produce test cases in this exact table structure:

| TC ID | Type | Module | Scenario | Precondition | Steps | Expected Result | Priority | Severity |
|---|---|---|---|---|---|---|---|---|

**Type:** Positive / Negative / Edge
**Module:** Homepage | Cart | Search | Sort | Auth | Category | Product Detail | Wishlist | Checkout | Navigation | URL
**Priority:** High / Medium / Low
**Severity:** Critical / Major / Minor / Trivial

---

## Functional Modules & Coverage Rules

### 1. Homepage

**What to cover:**
- Page load and all category section visibility
- Category banner carousel clickability
- Product card data accuracy (name, price, ADD button)
- "View all" links per category section
- Sort dropdown availability and persistence

**Edge cases to include:**
- Sort applied on homepage — does it persist when navigating to a category and back?
- Does the category carousel loop correctly or break at the last item?
- What happens if a category section has zero products — does the section header still render?
- Product price displayed as ₹0 — is it still addable to cart?
- Does the homepage reload reset the sort state to "Featured"?

---

### 2. Product Catalog / Category Pages

**What to cover:**
- Category page loads correct products (no cross-category bleed)
- "View all" from homepage matches full category page product count
- Breadcrumb accuracy on category pages
- Sort applied within a category page

**Edge cases to include:**
- Navigate to a category with exactly 1 product — are layout/spacing rules intact?
- Navigate to `/categories/invalid-slug` — expect 404 or graceful fallback, not a blank white page
- What if a category has products with identical prices — does sort produce a stable order or shuffle?
- Category page accessed via direct URL vs. via banner click — behavior must be identical
- Applying sort on category page, then clicking browser Back — does sort reset or persist?

---

### 3. Product Detail Page

**What to cover:**
- Product name, image, price, description, and Add to Cart button all present
- Wishlist (heart) icon available and functional
- Add to Cart from detail page increments cart badge
- Breadcrumb shows correct path: Home > Category > Product

**Edge cases to include:**
- Navigate directly to a valid product URL — page must load without requiring prior navigation
- Navigate to `/products/fake-product-xyz` — expect 404 or redirect, not crash
- Add to cart from detail page when the same product already exists in cart — quantity should increment, not duplicate
- Product with a very long name — does the UI truncate or overflow?
- Product with no description — does the layout break or gracefully omit the field?

---

### 4. Cart

**What to cover:**
- Add single product → cart badge increments
- Add multiple distinct products → all appear as separate line items
- Add same product multiple times → single line item with incremented quantity
- Increase quantity via + button → subtotal updates
- Decrease quantity via − button → subtotal updates
- Decrease quantity to 0 → product is removed OR quantity is blocked at 1
- Remove product explicitly → line item disappears
- Remove all products → empty state message displayed, total shows ₹0
- Cart total = sum of (unit price × quantity) for all items

**Edge cases to include:**
- Rapid-click ADD (5+ times in quick succession) on the same product — quantity must reflect actual count, no duplicate line items, no UI freeze
- Add a product, navigate away, return to cart — cart must persist (session-level persistence)
- Modify quantity in cart, then refresh the page — does the quantity persist or reset?
- Cart with 10+ different products — does the cart page scroll correctly, no overflow clipping?
- Add product at ₹0 price (if any exists) — does it appear in cart with ₹0 and not break the total?
- Decrease quantity from 2 to 1, then click − again — must either remove the item or stay at 1, never show 0 or negative
- Cart badge count — does it show total number of distinct items or total units? Must be consistent with cart page
- Open cart without adding any product — empty state with ₹0, no stale data from any prior session

---

### 5. Search

**What to cover:**
- Valid keyword returns relevant products (e.g., "Cadbury" returns Cadbury items)
- Partial keyword match (e.g., "Haldir" returns Haldiram products)
- Non-existent keyword shows "No results found" message, no crash
- Search results navigate correctly to product detail on click

**Edge cases to include:**
- Whitespace-only input (spaces, tabs) — must NOT return all products; show empty/no-results state
- Special characters only (`!@#$%^&*`) — no crash, graceful empty results
- Extremely long input string (100+ characters) — no layout overflow, no server error
- Case sensitivity — "cadbury" vs "CADBURY" vs "Cadbury" must all return same results
- Single character input (e.g., "a") — system must handle without crash; results may be broad but valid
- Search term that matches a category name but not a product name (e.g., "Beverages") — does it return products from that category or show no results?
- Searching immediately after page load before assets are fully rendered — must not throw a JS error

---

### 6. Sort

**What to cover:**
- Price low to high: ascending order confirmed across visible products
- Price high to low: descending order confirmed
- Discount: highest discount % first
- Featured: returns to default ordering

**Edge cases to include:**
- Sort applied, then a product is added to cart — does the sort order hold, or does the page reflow/reset?
- Sort on homepage: does it affect all category sections simultaneously, or only one?
- Products with identical prices under "Price low to high" — order must be stable (no shuffle on re-click)
- Sort applied, then navigate to a category via banner — does sort state carry over or reset on the new page?
- Clicking the same sort option twice — no crash, order remains consistent
- Sort dropdown closed without selecting — current sort must remain unchanged

---

### 7. Authentication (OTP Sign-in)

**What to cover:**
- Valid 10-digit Indian mobile → OTP sent confirmation
- Correct OTP entered → user logged in, account state reflects authenticated status
- Invalid OTP → error message, no login

**Negative inputs:**
- Fewer than 10 digits (e.g., 5 digits) → validation error before OTP is dispatched
- More than 10 digits → field must reject extra input OR validation error before dispatch
- Empty field → form does not submit, prompt to enter number
- Alphabets in mobile field → input rejected or not accepted by the field
- Special characters in mobile field → same rejection behavior

**Edge cases to include:**
- OTP request sent, OTP expires (if there's a timer visible) — attempting to use expired OTP must show appropriate error
- OTP field accepts only 4–6 digits (whatever the actual OTP length is) — extra characters must be blocked
- Double-tap or rapid double-click on "Send OTP" button — only one OTP request must be sent, not two
- Sign-in modal opened, then closed without signing in — no partial auth state persists
- Authenticated user navigates to sign-in URL directly — should redirect or show already-logged-in state
- Session persistence after browser tab close and reopen — is the user still logged in?

---

### 8. Wishlist

**What to cover:**
- Add product via heart icon on detail page → appears in `/wishlist`
- Wishlist page loads with saved items
- Wishlist accessible without login shows empty state or redirects to sign-in (either is acceptable, must be consistent)

**Edge cases to include:**
- Add the same product to wishlist twice — must not duplicate the entry
- Wishlist with many items — page must scroll correctly, no rendering overflow
- Navigate to `/wishlist` without ever adding anything — empty state message must show, no crash
- Product added to wishlist while not logged in — behavior must be defined (prompt to login, or guest wishlist that prompts on page load)
- Remove a product from wishlist (if the feature exists) — item must disappear, no stale entry

---

### 9. Checkout Gate

**What to cover:**
- Unauthenticated user attempts checkout → redirect or modal prompt to sign in
- Authenticated user with products in cart → checkout flow initiates (or blocked by store-not-accepting banner)
- "Store is currently not accepting orders" banner present → no order placed silently, clear blocking message shown

**Edge cases to include:**
- User is logged in, store IS accepting orders, cart has 1 item — does checkout flow proceed without errors?
- User is logged in, attempts checkout with an empty cart — must block or show "cart is empty" message
- Store-not-accepting banner visible — clicking "Proceed" or "Checkout" button must not silently create an order in the background
- Session expires mid-checkout — user must be re-prompted to login, cart data must not be lost

---

### 10. Navigation & URL Boundaries

**What to cover:**
- Breadcrumb links on category and product pages navigate correctly
- Header navigation links (Home, Shop, Wishlist, Store Locator) work
- Browser Back/Forward behaves consistently with application state

**Edge cases to include:**
- Navigate to `/categories/invalid-category` → 404 or graceful fallback, no white screen or JS error
- Navigate to `/products/fake-product-xyz` → 404 or redirect, no raw stack trace
- Navigate to a correct product URL directly (bypassing homepage) → detail page loads fully
- Deep-link to a category page → products load without requiring homepage visit first
- URL with query string appended manually (e.g., `?foo=bar`) → no crash, page handles gracefully
- Navigate with browser Back after cart modification — cart state must remain consistent with what was last saved, not revert
- Double-click on a navigation link — must not duplicate the navigation or cause a state loop

---

## What NOT to Include in Generated Test Cases

- Performance benchmarks (page load time, TTFBs)
- Accessibility audits (WCAG, ARIA)
- SEO tag validation
- API-level or network-level tests
- Automated script steps (Selenium, Playwright, Cypress syntax)
- Non-functional requirements (uptime, concurrency)

---

## Prioritization Logic

Apply these priority and severity rules consistently:

| Scenario Type | Priority | Severity |
|---|---|---|
| Core purchase flow (add to cart, cart total, checkout gate) | High | Critical |
| Auth flows (valid OTP, invalid inputs) | High | Major–Critical |
| Search (valid query, empty results) | High | Critical |
| Sort (all options functional) | Medium | Major |
| Navigation / breadcrumbs | Medium | Minor–Major |
| Wishlist | Medium | Minor |
| URL boundary / 404 handling | Low | Minor |
| Edge cases on input boundaries | Medium | Major |
| Edge cases on session/state persistence | High | Major |
| Edge cases on rapid/duplicate interactions | Medium | Major |

---
