---
name: greenkart-qa
description: >
  Use this skill for any manual QA or testing task involving the GreenKart
  e-commerce demo application at https://rahulshettyacademy.com/seleniumPractise/#/.
  Triggers when the user mentions GreenKart, rahulshettyacademy seleniumPractise,
  or asks to write/extend/review manual test cases for this veggie/fruits cart app.
  Covers test case writing, exploratory testing, test data, defect reporting,
  and test execution tracking. Use even when the user only partially references
  the app (e.g., "the practice site", "the cart demo", "Selenium practice app").
compatibility: Manual QA — no automation tools required; any modern browser supported
---

# GreenKart Manual QA Skill

Comprehensive manual testing knowledge base for the GreenKart demo e-commerce application.

---

## Application Overview

| Property        | Value                                                                 |
|-----------------|-----------------------------------------------------------------------|
| **URL**         | https://rahulshettyacademy.com/seleniumPractise/#/                    |
| **Title**       | GreenKart - veg and fruits kart                                       |
| **Type**        | Single Page Application (SPA) — Angular/React frontend, hash routing  |
| **Purpose**     | Selenium/QA automation practice site by Rahul Shetty Academy          |
| **Auth**        | Optional Sign In (username + password); most flows work as guest      |

---

## Application Structure & Modules

The app has **10 functional modules** covered across 62 baseline test cases:

| Module | Area                          | TC Range    | Key Focus                                      |
|--------|-------------------------------|-------------|------------------------------------------------|
| 1      | Home Page & Navigation        | TC_001–004  | Page load, title, logo, nav links              |
| 2      | Product Listing & Display     | TC_005–009  | Product grid, names, prices, images, buttons   |
| 3      | Search Functionality          | TC_010–016  | Valid/partial/invalid/special char searches    |
| 4      | Add to Cart                   | TC_017–022  | Add items, qty +/−, cart badge count           |
| 5      | Cart Review & Management      | TC_023–031  | Cart page, subtotals, qty changes, empty cart  |
| 6      | Checkout Process              | TC_032–040  | Coupon codes, order total, place order         |
| 7      | Offers Page                   | TC_041–043  | Offer navigation, content, add offer to cart   |
| 8      | Sign In / Authentication      | TC_044–051  | Valid/invalid login, empty fields, masking     |
| 9      | End-to-End Purchase Flows     | TC_052–056  | Full flows, persistence, multi-product orders  |
| 10     | UI, Accessibility & Responsive| TC_057–062  | Layouts (desktop/tablet/mobile), console errors|

---

## Where to Find Things — Manual Tester Navigation Guide

### Navigation Bar (Top of every page)
| Element | Where to Look | What to Verify |
|---|---|---|
| GreenKart Logo | Top-left corner | Visible; clicking returns to home |
| Search Bar | Top-center | Accepts input; filters products live |
| Cart Icon | Top-right | Shows badge count of items added |
| Home Link | Nav menu | Navigates to product listing |
| Offers Link | Nav menu | Navigates to Offers page |
| Sign In Link | Nav menu | Navigates to login page |

### Home Page — Product Grid
| Element | What to Verify |
|---|---|
| Product Name | Clearly readable (e.g., Brocolli, Tomato) |
| Product Price | Shown as `Rs.XX` format |
| Product Image | Thumbnail loads without broken icon |
| ADD TO CART button | Present on every product card; clickable |
| +/− Qty buttons | Appear after adding to cart; update count |
| Qty counter | Shows current quantity between + and − |

### Cart Page (click Cart Icon to open)
| Element | What to Verify |
|---|---|
| Item Name | Matches product added from home page |
| Unit Price | Same price as shown on product card |
| Quantity | Reflects how many were added |
| Subtotal | Unit price × quantity |
| Grand Total | Sum of all subtotals |
| PROCEED TO CHECKOUT button | Visible and clickable when cart has items |
| Empty cart message | Shown when no items in cart |

### Checkout Page
| Element | What to Verify |
|---|---|
| Item Summary | Lists all cart products with qty and price |
| Coupon Code Field | Accepts text input |
| Apply Button | Triggers coupon validation |
| Discount Line | Appears after valid coupon; shows amount |
| Total Amount | Updates after coupon; less than original |
| Place Order Button | Completes the purchase; shows confirmation |

### Sign In Page (`#/login`)
| Element | What to Verify |
|---|---|
| Username Field | Accepts text |
| Password Field | Input is masked (shows dots/asterisks) |
| Sign In Button | Submits the form |
| Error Message | Appears below form on invalid credentials |

### Offers Page (`#/offers`)
| Element | What to Verify |
|---|---|
| Offer Products | Displayed with special pricing or badges |
| ADD TO CART (Offers) | Works same as home page; updates cart badge |

---

## Test Data

### Products Available (sample)
| Product Name | Price (Rs.) |
|---|---|
| Brocolli | 15 |
| Cauliflower | 40 |
| Cucumber | 40 |
| Tomato | 35 |
| Spinach | 30 |
| Mushroom | 45 |
| Onion | 25 |
| Beetroot | 20 |

> Prices may vary; always assert dynamically from UI rather than hardcoding.

### Coupon Codes
| Code | Status | Effect |
|---|---|---|
| `rahulshettyacademy` | Valid | Applies discount on total |
| `INVALID123` | Invalid | Shows error message |
| *(blank)* | Empty | Shows validation error |

### Login Credentials
| Type | Username | Password | Expected Outcome |
|---|---|---|---|
| Valid | rahul | rahul | Login success |
| Invalid Username | wronguser | rahul | Error message |
| Invalid Password | rahul | wrongpass | Error message |
| Empty | (blank) | (blank) | Validation error |

> These are demo credentials; verify against the live site as they may change.

---

## Existing Test Cases Reference (GreenKart_TestCases.docx)

The attached Word document contains **62 manual test cases** already documented:

- **Format:** TC ID | Test Case Title | Test Steps | Expected Result | Actual Result | Priority | Status
- **Priority Legend:** 🔴 High | 🟠 Medium | 🟢 Low
- **Status Values:** Pending | Pass | Fail
- **Prepared:** QA Team, 17/06/2026

When adding new test cases, continue numbering from **TC_063** onward and follow the same table format. Match the priority scheme and keep steps numbered (1. 2. 3. ...).

---

## Common Test Patterns

### Search Tests
```
Valid partial:     Type 'Broc'  → shows Brocolli
Full name:         Type 'Cauliflower' → shows only Cauliflower
Case insensitive:  Type 'cau' → shows Cauliflower
No results:        Type 'XYZ123' → empty list / no-match message
Special chars:     Type '@#$%' → graceful handling, no crash
Clear search:      Erase text → all products return
```

### Cart Arithmetic Assertions
```
Subtotal per item = price × quantity
Grand total       = sum of all subtotals
After coupon      = grand total − discount amount
Badge count       = number of unique products in cart
```

### End-to-End Flow Skeleton
```
1. Navigate to home  →  2. Search product  →  3. ADD TO CART
→  4. Adjust qty (+/−)  →  5. Click Cart icon
→  6. Verify cart items & total  →  7. PROCEED TO CHECKOUT
→  8. Apply coupon  →  9. Verify discounted total
→  10. Place Order  →  11. Assert confirmation
```

---

## Manual Test Execution Guidance

### How to Execute Tests Step by Step

**Before starting any test session:**
1. Open the browser (Chrome / Firefox / Edge)
2. Navigate to: `https://rahulshettyacademy.com/seleniumPractise/#/`
3. Clear browser cache/cookies if re-running tests that involve cart or login
4. Keep the browser DevTools (F12) open on the Console tab to watch for JS errors (TC_062)

---

### Search Functionality — Manual Steps
| Scenario | Steps to Execute | What to Check |
|---|---|---|
| Valid partial search | Type `Broc` in search bar | Only products matching "Broc" appear (e.g., Brocolli) |
| Full name search | Type `Cauliflower` | Only Cauliflower shown |
| Case insensitive | Type `cau` in lowercase | Cauliflower still appears |
| No match | Type `XYZ123` | Product grid empty or shows "no results" |
| Special characters | Type `@#$%` | No crash; empty or graceful message |
| Clear search | Type anything, then erase fully | All products return to view |

---

### Cart Operations — Manual Steps
| Scenario | Steps to Execute | What to Check |
|---|---|---|
| Add one item | Click ADD TO CART on any product | Cart badge shows `1`; +/− buttons appear |
| Increase qty | Click `+` button beside product | Qty increases by 1 per click |
| Decrease qty | Click `−` button | Qty decreases; at 0 the item is removed |
| Add 3 different items | ADD TO CART on 3 separate products | Badge shows `3` |
| Open cart | Click Cart icon (top-right) | Cart page opens with all added items |
| Verify subtotal | Price × Qty for any item | Subtotal matches manual calculation |
| Empty cart | Remove all items via `−` | Empty cart message appears |

---

### Checkout & Coupon — Manual Steps
1. Add at least one item to cart
2. Click the **Cart icon** → Cart page opens
3. Click **PROCEED TO CHECKOUT**
4. On checkout page — verify item summary (names, qty, price)
5. Enter coupon code in the coupon field:
   - Valid: `rahulshettyacademy` → discount should appear and total reduces
   - Invalid: `INVALID123` → error message shown, total unchanged
   - Blank: click Apply without typing → validation message shown
6. Verify updated total = original total − discount
7. Click **Place Order** → confirmation message or order ID shown

---

### Sign In — Manual Steps
| Scenario | Username | Password | Expected Result |
|---|---|---|---|
| Valid login | `rahul` | `rahul` | Redirected to home; logged-in state visible |
| Wrong username | `wronguser` | `rahul` | Error message displayed |
| Wrong password | `rahul` | `wrongpass` | Error message displayed |
| Both empty | *(blank)* | *(blank)* | Validation error shown |
| Username empty | *(blank)* | `rahul` | Username field validation error |
| Password empty | `rahul` | *(blank)* | Password field validation error |
| Password masking | Any | Type text | Characters show as dots/asterisks |

---

### Responsive Layout — Manual Steps
| Viewport | How to Set It | What to Check |
|---|---|---|
| Desktop 1920×1080 | Normal browser, maximize window | No overflow, all elements aligned |
| Tablet 768px | F12 → Toggle device toolbar → set width 768 | Nav and grid usable, no horizontal scroll |
| Mobile 375px | F12 → Toggle device toolbar → set width 375 | Cart, search, and products all functional |

---

### End-to-End Purchase Flow — Manual Execution Checklist
```
[ ] 1. Navigate to https://rahulshettyacademy.com/seleniumPractise/#/
[ ] 2. Search for 'Tomato' — verify product appears
[ ] 3. Click ADD TO CART — verify badge shows 1
[ ] 4. Click + three times — verify qty shows 4 total (1 original + 3)
[ ] 5. Click Cart icon — verify Tomato listed with correct qty and subtotal
[ ] 6. Click PROCEED TO CHECKOUT — verify item summary shown
[ ] 7. Enter coupon 'rahulshettyacademy' → click Apply — verify discount applied
[ ] 8. Verify discounted total = original total − discount
[ ] 9. Click Place Order — verify confirmation message appears
```

---

## Defect Reporting Template

When a test fails, log it using this format:

```
Defect ID    : DEF_XXX
TC ID        : TC_XXX
Module       : (e.g., Checkout Process)
Summary      : One-line description of the issue
Environment  : Browser name + version, OS
Steps to Reproduce:
  1.
  2.
  3.
Expected Result : (from test case)
Actual Result   : (what actually happened)
Severity        : Critical / Major / Minor / Trivial
Priority        : High / Medium / Low
Screenshot      : (attach if applicable)
Reported By     : (your name)
Date            : DD/MM/YYYY
```

---

---

## Checklist: When Writing/Extending Test Cases

- [ ] Use TC_XXX numbering; next available is TC_063
- [ ] Include numbered test steps (1. 2. 3. ...)
- [ ] State Expected Result clearly (what the user sees/gets)
- [ ] Assign Priority: High / Medium / Low
- [ ] Set Status to **Pending** for new/unexecuted cases
- [ ] Cover both positive (happy path) and negative (error) scenarios
- [ ] For cart math, assert computed values not just UI visibility
- [ ] For auth tests, include empty-field edge cases
- [ ] For E2E, trace the full flow from home → confirmation

---

## Priority Guidance

| Scenario Type | Default Priority |
|---|---|
| Page load / navigation | High |
| Core cart operations (add, remove, qty) | High |
| Checkout & coupon | High |
| Authentication (valid/invalid) | High |
| Search (valid & invalid) | High / Medium |
| UI layout & responsiveness | Medium |
| Cosmetic / image display | Low |
| Console error checks | Medium |
| Offers page | Medium–High |

---

## Notes & Known Behaviours

- The app is a **Single Page Application (SPA)** with hash routing (`#/`). The browser URL may not fully change between pages — navigate using the in-app links, not the browser back button, to avoid unexpected states.
- **Cart state** is stored in session/local storage. Refreshing the browser (TC_054) may or may not retain cart items — this is a deliberate test scenario; do not assume either outcome.
- The coupon code `rahulshettyacademy` is the known valid code for this practice app.
- **Product list and prices** may change over time. Always read them from the screen during execution rather than assuming fixed values.
- Use **browser DevTools (F12) → Console tab** during TC_062 to check for JavaScript errors; no red errors should appear during normal navigation.
- For **responsive testing** (TC_057–059), use the browser's built-in device toolbar (F12 → toggle device toolbar) rather than resizing the window manually, for more accurate viewport simulation.
