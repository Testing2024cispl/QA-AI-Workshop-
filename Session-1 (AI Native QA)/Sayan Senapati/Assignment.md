Manual Test Cases:- Member:-Sayan Senapati

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








