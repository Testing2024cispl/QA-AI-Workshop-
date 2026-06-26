Manual Test Cases:- Group 3:- Member:- Sayan Senapati

Working URL-https://v0-e-commerce-lunchbox-site.vercel.app/

Module: Cart & Checkout — Discount Coupon

Base Price per Lunch Box: $150

Expected Discount Logic: 20% off listing price (i.e., $150 → $120, savings of $30 per box)

# Human Written Test Cases
## Positive Test Cases
### **TC_001 — Verify product listing price is displayed correctly.**
1.Navigate to  the mentioned URL “https://v0-e-commerce-lunchbox-site.vercel.app/”

2.Check the price displayed under each of the 6 product cards (Bamboo Bento Box, Stainless Steel Tiffin, Glass Meal Prep Set, Thermal Insulated Box, Eco Bamboo Carrier, Electric Heated Box).

### TC_002 — Add a single lunch box to cart and examine subtotal calculation.
1.Go to the product selection page where the 6 product cards appear.

2.Click "Add to Cart" on "Bamboo Bento Box"

3.Hit the Shopping Cart icon to go to the Checkout page

### TC_003 — Apply LUNCH20 coupon on a single item and calculate 20% discount

1.Add "Glass Meal Prep Set" ($150) to cart

2.Go to Checkout page

3.Locate the coupon/promo code input field

4.Enter LUNCH20 and apply it

### TC_004 — Check discount amount matches 20% condition (not a flat $20)

1.Add any one lunch box ($150) to cart

2.Apply coupon LUNCH20

3.Note the discount amount shown and the final total

### TC_005 — Apply LUNCH20 on multiple lunch boxes.

1.Add "Thermal Insulated Box" to cart

2.Increase quantity to 2— Total listing price = $300

3.Go to Checkout

4.Apply coupon LUNCH20

### TC_006 — Apply LUNCH20 with multiple different products in cart

1.Add "Stainless Steel Tiffin" ($150) to cart

2.Add "Eco Bamboo Carrier" ($150) to cart

3.Go to Checkout — Subtotal should show $300

4.Apply coupon LUNCH20

## Negative Test Cases

### TC_007 — Verify coupon code is case-insensitive (lunch20 / Lunch20)

1.Add any lunch box to cart and go to Checkout

2.Enter lunch20 (lowercase) in the coupon field and apply

### TC_008 — Verify invalid/incorrect coupon code is rejected

1.Add a lunch box to cart and go to Checkout

2.Enter an invalid code, e.g. LUNCH50 or LUNCH2O (typo)

3.Click Apply

### TC_009 — Verify empty coupon field submission

1.Add a lunch box to cart and go to Checkout

2.Leave the coupon field blank

3.Click "Apply" button

### TC_010 — Verify coupon can be removed after being applied

1.Add a lunch box to cart and go to Checkout

2.Apply LUNCH20 — confirm total becomes $120

3.Click "Remove" / "Remove coupon" option (if available)

### TC_011 — Verify LUNCH20 cannot be applied twice.

1.Add a lunch box to cart and go to Checkout

2.Apply LUNCH20

3.Attempt to apply LUNCH20 again (or re-enter and click Apply a second time)

### TC_012 — Verify discount on empty cart / before adding products

1.Navigate directly to the given working URL https://v0-e-commerce-lunchbox-site.vercel.app/checkout without adding items to cart

2.Check if a coupon input is visible/usable

### TC_013 — Verify removing a product from cart after coupon is applied recalculates discount correctly

1.Add 2 lunch boxes ($150 each = $300 subtotal) to cart

2.Apply LUNCH20 → total becomes $240 (20% of $300 = $60 off)

3.Remove 1 lunch box from the cart

### TC_014 — Verify UI display of discount breakdown at checkout

1.Add any lunch box to cart and go to Checkout

2.Apply LUNCH20

3.Review the order summary section

### TC_015 — Verify price consistency across all 6 products

1.One at a time, add each of the 6 products to cart (Bamboo Bento Box, Stainless Steel Tiffin, Glass Meal Prep Set, Thermal Insulated Box, Eco Bamboo Carrier, Electric Heated Box)

2.Apply LUNCH20 for each

3.Verify final total each time

# AI DRIVEN TEST CASES

Prompt-
You are an Software QA engineer, please give me the positive and negative test cases with id, steps and test scenarios for the mentioned url "https://v0-e-commerce-lunchbox-site.vercel.app/" by using the condition  LUNCH20 will apply 20% discount on listing price Price for every lunch box will be $150.

## Positive Test Cases

### TC_P01 — Verify listing price displayed for each product

1.Navigate to https://v0-e-commerce-lunchbox-site.vercel.app/

2.Scroll through "Our Collection" section

3.Check price label under each of the 6 products

### TC_P02 — Add single product to cart and verify cart subtotal

1.Click "Add to Cart" on "Bamboo Bento Box"

2.Click the Shopping Cart icon → navigates to Checkout page

3.Verify item listed with price

### TC_P03 — Apply LUNCH20 on a single item and verify exact 20% deduction

1.Add "Stainless Steel Tiffin" ($150) to cart

2.Go to Checkout

3.Enter LUNCH20 in the coupon field and click Apply

### TC_P04 — Validate discount calculation precisely matches 20%, not flat $20

1.Add one lunch box to cart ($150)

2.Apply LUNCH20

3.Compare displayed discount value against expected $30 (20%)


### TC_P05 — Apply LUNCH20 with quantity > 1 of same product

1.Add "Glass Meal Prep Set" to cart

2.Increase quantity to 2 (subtotal = $300)

3.Apply LUNCH20 at checkout


### TC_P06 — Apply LUNCH20 with multiple different products in cart

1.Add "Bamboo Bento Box" ($150)

2.Add "Electric Heated Box" ($150)

3.Go to Checkout — subtotal = $300

4.Apply LUNCH20


### TC_P07 — Verify coupon code accepted in lowercase

1.Add a product to cart, go to Checkout

2.Enter lunch20 (lowercase) and Apply


### TC_P08 — Verify order summary breakdown after discount applied

1.Add a lunch box to cart

2.Apply LUNCH20

3.Review order summary panel


### TC_P09 — Verify discount recalculates correctly after removing an item

1.Add 2 lunch boxes (subtotal $300)

2.Apply LUNCH20 → total = $240

3.Remove 1 item from cart


### TC_P10 — Verify coupon removal reverts price correctly

1.Add a lunch box, apply LUNCH20 (total becomes $120)

2.Click "Remove coupon" (if available)


### TC_P11 — Verify discount consistency across all 6 products

1.One at a time, add each of the 6 products, apply LUNCH20, note final total

2.Repeat for all products


## Negative Test Cases

### TC_N01 — Apply invalid/incorrect coupon code

1.Add a lunch box to cart, go to Checkout

2.Enter an invalid code, e.g. LUNCH50 or LUNCH2O

3.Click Apply


### TC_N02 — Submit empty coupon field

1.Add a product to cart, go to Checkout

2.Leave coupon field blank

3.Click "Apply"


### TC_N03 — Apply LUNCH20 twice (double application / stacking attempt)

1.Add a lunch box to cart, apply LUNCH20 once (total = $120)

2.Attempt to apply LUNCH20 again


### TC_N04 — Apply coupon on an empty cart

1.Navigate directly to https://v0-e-commerce-lunchbox-site.vercel.app/checkout without adding any product

2.Attempt to locate/use coupon field


### TC_N05 — Apply coupon with leading/trailing whitespace

1.Add a product to cart, go to Checkout

2.Enter  LUNCH20  (with spaces) in the coupon field

3.Click Apply


### TC_N06 — Verify discount does NOT apply flat $20 instead of 20%

1.Add one lunch box ($150) to cart

2.Apply LUNCH20

3.Check if discount = $20 (flat) and total = $130


### TC_N07 — Apply coupon with special characters / SQL injection attempt

1.Add a product to cart, go to Checkout

2.Enter LUNCH20'; DROP TABLE-- or <script>alert(1)</script> in coupon field

3.Click Apply


### TC_N08 — Apply coupon exceeding max input length

1.Add a product to cart, go to Checkout

2.Enter an abnormally long string (e.g., 500 characters) in the coupon field

3.Click Apply


### TC_N09 — Apply coupon after removing all items from cart

1.Add a lunch box, apply LUNCH20 successfully

2.Remove the only item from cart


### TC_N10 — Verify behavior on rapid repeated clicking of "Apply" button

1.Add a product to cart, enter LUNCH20

2.Rapidly double/triple-click the "Apply" button



### TC_N11 — Verify coupon field does not break on browser refresh after applying

1.Add a product, apply LUNCH20 (total = $120)

2.Refresh the checkout page


### TC_N12 — Verify partially matching coupon code is rejected

1.Add a product to cart, go to Checkout

2.Enter LUNCH2 or LUNCH200 (close but incorrect variants)

3.Click Apply

# My Thoughts

## Strengths

1.Broad functional coverage

2.Accelerated baseline creation

3.Inclusion of common edge cases

## Areas for Improvement

1.Lack of application-specific context

2.Insufficient field-level validation coverage

3.Assumption-driven negative scenarios


# Final Test Cases (AI + Human Written)

## Positive Test Cases

### TC_P01 — Verify listing price on homepage for all products

1.Open homepage

2.Scroll through "Our Collection"

3.Check price label under each of 6 products

### TC_P02 — Add single product to cart, verify subtotal

1.Click "Add to Cart" on Bamboo Bento Box

2.Click Shopping Cart icon to open Checkout

### TC_P03 — Apply LUNCH20 on single item — verify 20% deduction

1.Add Stainless Steel Tiffin ($150)

2.Go to Checkout 

3.Enter LUNCH20 in coupon field  

4.Click Apply

### TC_P04 — Validate discount is calculated as percentage (20%), not flat amount

1.Add 1 lunch box to cart 

2.Apply LUNCH20 

3.Inspect discount line item value in summary

### TC_P05 — Apply LUNCH20 with quantity > 1 of same product

1.Add Glass Meal Prep Set

2.Increase qty to 2 (subtotal $300)

3.Go to Checkout, apply LUNCH20

### TC_P06 — Apply LUNCH20 with multiple different products in cart

1.Add Bamboo Bento Box ($150)

2.Add Electric Heated Box ($150)

3.Checkout shows subtotal $300

4.Apply LUNCH20

### TC_P07 — Verify coupon field accepts lowercase entry

1.Add product to cart

2.Go to Checkout

3.Enter lunch20 and Apply

### TC_P08 — Verify checkout order summary breakdown

1.Add lunch box

2.Apply LUNCH20

3.Review summary panel

### TC_P09 — Verify discount recalculates after item removal

1.Add 2 lunch boxes (subtotal $300)

2.Apply LUNCH20 (total $240)

3.Remove 1 item

### TC_P10 — Verify coupon removal reverts to original price

1.Add lunch box, apply LUNCH20 (total $120)

2.Click "Remove coupon"

### TC_P11 — Verify discount consistency across all 6 products

1.Individually add each of 6 products

2.Apply LUNCH20 each time

3.Note final total

### TC_P12 — Verify coupon input field accepts exactly 7 characters (LUNCH20 length) without truncation

1.Go to Checkout

2.Click into coupon field

3.Type LUNCH20 character by character, observe field

### TC_P13 — Verify "Add to Cart" button updates cart icon/count immediately (real-time feedback)

1.Note current cart count/icon state

2.Click "Add to Cart" on any product

3.Observe cart icon

### TC_P14 — Verify navigating from product listing to Checkout and back preserves cart state

1.Add a product to cart

2.Click "Back to Shop" from Checkout

3.Click Shopping Cart icon again

### TC_P15 — Verify total price formatting (currency symbol, decimal precision) is consistent

1.Add product, apply LUNCH20

2.Inspect Subtotal, Discount, and Total values

## Negative Test Cases

### TC_N01 — Apply invalid/incorrect coupon code

1.Add product to cart

2.Enter LUNCH50 or LUNCH2O (typo)

3.Click Apply

### TC_N02 — Submit empty coupon field

1.Add product to cart

2.Leave coupon field blank

3.Click Apply

### TC_N03 — Apply LUNCH20 twice (stacking attempt)

1.Add product, apply LUNCH20 (total $120)

2.Re-enter LUNCH20, click Apply again

### TC_N04 — Apply coupon on empty cart

1.Navigate directly to /checkout with no items added

### TC_N05 — Apply coupon with leading/trailing whitespace

1.Add product to cart

2.Enter ␣␣LUNCH20␣␣ (with spaces)

3.Click Apply

### TC_N06 — Verify discount does NOT default to flat $20 instead of 20%

1.Add 1 lunch box ($150)

2.Apply LUNCH20

3.Check discount value and total

### TC_N07 — Apply coupon with special characters / injection attempt

1.Add product to cart

2.Enter LUNCH20'; DROP TABLE-- or <script>alert(1)</script>

3.Click Apply

### TC_N08 — Apply coupon exceeding reasonable max input length

1.Add product to cart

2.Paste a 500-character string into coupon field

3.Click Apply

### TC_N09 — Apply coupon, then remove all items from cart

1.Add lunch box, apply LUNCH20 successfully

2.Remove the only item from cart

### TC_N10 — Verify rapid/double-click on "Apply" button does not duplicate discount

1.Add product, enter LUNCH20

2.Double/triple-click "Apply" rapidly

### TC_N11 — Verify browser refresh after coupon applied does not produce inconsistent state

1.Add product, apply LUNCH20 (total $120)

2.Refresh the checkout page

### TC_N12 — Apply partially-matching/incorrect variant of coupon code

1.Add product to cart

2.Enter LUNCH2 or LUNCH200

3.Click Apply

### TC_N13 — Verify back button navigation after checkout does not retain stale discount/cart mismatch

1.Add product, apply LUNCH20

2.Click browser Back button

3.Click Checkout/cart icon again

### TC_N14 — Verify coupon field rejects numeric-only or alphabet-only incomplete codes

1.Add product to cart

2.Enter 20 or LUNCH only

3.Click Apply

### TC_N15 — Verify "Apply" button behavior when clicked with no product price loaded (slow network/loading state)

1.Throttle network speed (DevTools)

2.Add product to cart while page is still loading pricing data

3.Immediately apply LUNCH20


-------------------------------------SESSION 2----------------------------------



# Manual Test Cases

**Group:** Group 3
**Member:** Sayan Senapati

**Working URL:** https://v0-e-commerce-lunchbox-site.vercel.app/

## Module

**Cart & Checkout — Discount Coupon**

### Test Data

| Item                     | Value       |
| ------------------------ | ----------- |
| Base Price per Lunch Box | **$150**    |
| Coupon Code              | **LUNCH20** |
| Discount                 | **20% Off** |
| Discount Amount          | **$30**     |
| Final Price              | **$120**    |

---

# Human Written Test Cases

## Positive Test Cases

### TC_001 — Verify product listing price is displayed correctly

**Steps**

1. Navigate to the application.
2. Verify the price displayed under each of the following six products:

   * Bamboo Bento Box
   * Stainless Steel Tiffin
   * Glass Meal Prep Set
   * Thermal Insulated Box
   * Eco Bamboo Carrier
   * Electric Heated Box

**Expected Result**

* All products display a price of **$150**.

---

### TC_002 — Add a single lunch box to cart and examine subtotal calculation

**Steps**

1. Open the product listing page.
2. Click **Add to Cart** on **Bamboo Bento Box**.
3. Click the Shopping Cart icon.

**Expected Result**

* Bamboo Bento Box appears in the cart.
* Cart subtotal equals **$150**.

---

### TC_003 — Apply LUNCH20 coupon on a single item

**Steps**

1. Add **Glass Meal Prep Set ($150)** to the cart.
2. Navigate to Checkout.
3. Enter **LUNCH20**.
4. Click **Apply**.

**Expected Result**

* Discount = **$30**
* Total = **$120**

---

### TC_004 — Verify discount amount equals 20%

**Steps**

1. Add one lunch box.
2. Apply **LUNCH20**.
3. Observe discount and total.

**Expected Result**

* Discount = **20% ($30)**
* Final Total = **$120**

---

### TC_005 — Apply coupon on multiple quantities

**Steps**

1. Add **Thermal Insulated Box**.
2. Increase quantity to **2**.
3. Go to Checkout.
4. Apply **LUNCH20**.

**Expected Result**

| Subtotal | Discount | Final Total |
| -------- | -------- | ----------- |
| $300     | $60      | $240        |

---

### TC_006 — Apply coupon on multiple different products

**Steps**

1. Add **Stainless Steel Tiffin**.
2. Add **Eco Bamboo Carrier**.
3. Proceed to Checkout.
4. Apply **LUNCH20**.

**Expected Result**

| Subtotal | Discount | Final Total |
| -------- | -------- | ----------- |
| $300     | $60      | $240        |

---

## Negative Test Cases

### TC_007 — Verify coupon code is case-insensitive

**Steps**

1. Add any lunch box.
2. Go to Checkout.
3. Enter **lunch20**.
4. Click Apply.

**Expected Result**

* Coupon is accepted (if application supports case-insensitive validation).

---

### TC_008 — Verify invalid coupon code is rejected

**Steps**

1. Add a lunch box.
2. Enter **LUNCH50** or **LUNCH2O**.
3. Click Apply.

**Expected Result**

* Error message appears.
* Discount is not applied.

---

### TC_009 — Verify empty coupon submission

**Steps**

1. Add a lunch box.
2. Leave coupon field blank.
3. Click Apply.

**Expected Result**

* Validation message is displayed.

---

### TC_010 — Verify coupon removal

**Steps**

1. Apply **LUNCH20**.
2. Remove the coupon.

**Expected Result**

* Discount is removed.
* Original subtotal is restored.

---

### TC_011 — Verify coupon cannot be applied twice

**Steps**

1. Apply **LUNCH20**.
2. Attempt to apply it again.

**Expected Result**

* Coupon is applied only once.

---

### TC_012 — Verify coupon on empty cart

**Steps**

1. Navigate directly to Checkout.
2. Attempt to apply coupon.

**Expected Result**

* Coupon cannot be applied.
* Appropriate validation message appears.

---

### TC_013 — Verify discount recalculates after removing product

**Steps**

1. Add two lunch boxes.
2. Apply **LUNCH20**.
3. Remove one product.

**Expected Result**

* Discount recalculates based on remaining subtotal.

---

### TC_014 — Verify checkout discount summary

**Steps**

1. Add one lunch box.
2. Apply **LUNCH20**.
3. Review Order Summary.

**Expected Result**

Order Summary displays:

* Subtotal
* Discount
* Final Total

---

### TC_015 — Verify pricing consistency across all products

**Steps**

1. Add each of the six products individually.
2. Apply **LUNCH20**.

**Expected Result**

Every product:

* Price = **$150**
* Discount = **$30**
* Total = **$120**

---

# AI Generated Test Cases

## Prompt

> You are a Software QA Engineer. Generate positive and negative test cases with IDs, scenarios, and steps for the Lunch Box e-commerce website where **LUNCH20** provides **20% discount** on every lunch box priced at **$150**.

---

## Positive Test Cases

| ID     | Test Scenario                                     |
| ------ | ------------------------------------------------- |
| TC_P01 | Verify listing price for all products             |
| TC_P02 | Verify cart subtotal after adding one product     |
| TC_P03 | Verify exact 20% discount on one item             |
| TC_P04 | Validate percentage calculation                   |
| TC_P05 | Verify coupon for multiple quantities             |
| TC_P06 | Verify coupon for multiple products               |
| TC_P07 | Verify lowercase coupon acceptance                |
| TC_P08 | Verify order summary                              |
| TC_P09 | Verify discount recalculation after removing item |
| TC_P10 | Verify coupon removal                             |
| TC_P11 | Verify consistency across all products            |

---

## Negative Test Cases

| ID     | Test Scenario                           |
| ------ | --------------------------------------- |
| TC_N01 | Invalid coupon                          |
| TC_N02 | Empty coupon                            |
| TC_N03 | Duplicate coupon application            |
| TC_N04 | Coupon on empty cart                    |
| TC_N05 | Coupon with whitespace                  |
| TC_N06 | Verify discount is percentage, not flat |
| TC_N07 | SQL Injection / XSS input               |
| TC_N08 | Long coupon input                       |
| TC_N09 | Remove all items after coupon           |
| TC_N10 | Rapid Apply button clicks               |
| TC_N11 | Refresh after coupon applied            |
| TC_N12 | Partial coupon code                     |

---

# Analysis

## Strengths

* Broad functional coverage
* Faster baseline test creation
* Covers common edge cases
* Easy to automate

## Areas for Improvement

* Add application-specific scenarios
* Include field validation tests
* Add accessibility testing
* Add performance testing
* Include security-specific validations

---

# Final Test Cases (AI + Human Written)

## Positive Test Cases

| ID     | Test Scenario                            |
| ------ | ---------------------------------------- |
| TC_P01 | Verify listing price on homepage         |
| TC_P02 | Verify subtotal after adding one product |
| TC_P03 | Verify 20% coupon application            |
| TC_P04 | Validate percentage discount             |
| TC_P05 | Coupon with multiple quantities          |
| TC_P06 | Coupon with multiple products            |
| TC_P07 | Lowercase coupon acceptance              |
| TC_P08 | Order summary validation                 |
| TC_P09 | Discount recalculation                   |
| TC_P10 | Coupon removal                           |
| TC_P11 | Discount consistency                     |
| TC_P12 | Coupon field length validation           |
| TC_P13 | Cart icon updates immediately            |
| TC_P14 | Cart persists after navigation           |
| TC_P15 | Currency formatting validation           |

---

## Negative Test Cases

| ID     | Test Scenario                     |
| ------ | --------------------------------- |
| TC_N01 | Invalid coupon                    |
| TC_N02 | Empty coupon                      |
| TC_N03 | Duplicate coupon                  |
| TC_N04 | Coupon on empty cart              |
| TC_N05 | Coupon with whitespace            |
| TC_N06 | Prevent flat discount             |
| TC_N07 | SQL Injection / XSS attempt       |
| TC_N08 | Maximum input length              |
| TC_N09 | Remove all products after coupon  |
| TC_N10 | Rapid Apply button clicks         |
| TC_N11 | Browser refresh after coupon      |
| TC_N12 | Partial coupon variants           |
| TC_N13 | Browser Back navigation           |
| TC_N14 | Numeric/alphabetic invalid coupon |
| TC_N15 | Slow network coupon application   |

---

# Conclusion

The consolidated test suite combines **manual QA knowledge** with **AI-assisted scenario generation**, providing comprehensive coverage of:

* Functional Testing
* Coupon Validation
* Discount Calculation
* UI Verification
* Boundary Testing
* Negative Testing
* Security-Oriented Input Validation
* User Experience Validation

This test suite serves as a strong foundation for both **manual testing** and **Playwright automation**.


