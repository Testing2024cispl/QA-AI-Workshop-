[e2e_test_cases_automationexercise.md](https://github.com/user-attachments/files/29156507/e2e_test_cases_automationexercise.md)
# E2E Test Cases: Complete Purchase Flow
## Website: https://automationexercise.com

---

##  Test Flow Overview

| Step | Feature | Description |
|------|---------|-------------|
| 1 | User Registration | Create a new user account |
| 2 | User Login | Login with registered credentials |
| 3 | Browse Products | Navigate and filter products |
| 4 | Add to Cart | Add product to shopping cart |
| 5 | View Cart | Review cart items and quantities |
| 6 | Checkout | Enter shipping and payment details |
| 7 | Order Confirmation | Verify successful order placement |

---

## ✅ MANUAL TEST CASES

### TC-E2E-001: Complete Purchase Flow - Happy Path

| Field | Details |
|-------|---------|
| **Test Case ID** | TC-E2E-001 |
| **Test Case Name** | Complete Purchase Flow |
| **Priority** | P0 - Critical |
| **Pre-requisites** | valid email |

**Test Steps:**

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | **Navigate to** `https://automationexercise.com`** | Home page loads successfully with visible navigation menu |
| 2 | **Click on "Signup / Login" button** | Login/Signup page displays with "New User Signup!" and "Login to your account" sections |
| 3 | Enter a unique name in "Name" field | Name is accepted and displayed in the field |
| 4 | Enter a valid email address in "Email" field | Email is accepted and displayed |
| 5 | Click "Signup" button | Account creation is initiated, redirect to Registration page |
| 6 | Fill in account information (Title, Name, Email, Password, Date of Birth) | All fields are filled correctly |
| 7 | Select "Sign up for our newsletter!" checkbox | Checkbox is selected |
| 8 | Select "Receive special offers from our partners!" checkbox | Checkbox is selected |
| 9 | Fill in address information (First name, Last name, Company, Address, Country, State, City, Zipcode, Mobile Number) | All address fields are filled |
| 10 | Click "Create Account" button | Account is created, success message displayed |
| 11 | Click "Continue" button | Redirected to home page with logged-in state |
| 12 | Verify "Logged in as [username]" message is visible | User is logged in successfully |
| 13 | Click on "Products" in navigation | Products page loads with product listing |
| 14 | Click "Add to Cart" on any product | Product added success message appears |
| 15 | Click "View Cart" in the success message | Cart page opens with added product |
| 16 | Verify product is displayed in cart | Product name, price, and quantity are visible |
| 17 | Click "Proceed to Checkout" button | Checkout page displays with address details |
| 18 | Review order summary and delivery address | All details are correctly displayed |
| 19 | Add comment in "Add a comment about your order" text area | Comment is entered successfully |
| 20 | Click "Place Order" button | Payment page/modal appears |
| 21 | Enter payment details (Card Number, Card CVV, Expiry Date, Card Holder Name) | All payment fields are filled |
| 22 | Click "Pay and Confirm Order" button | Order is placed successfully |
| 23 | Verify success message "Your order has been placed successfully!" | Success message is displayed |
| 24 | Click "Continue" button | Returned to home page |
| 25 | Click "Delete Account" in the account menu | Account deletion initiated |
| 26 | Confirm deletion | Account deleted, returned to home page |

**Pass Criteria:** All 26 steps executed successfully with expected results at each step.

---

### TC-E2E-002: User Registration with Required Fields Only

| Field | Details |
|-------|---------|
| **Test Case ID** | TC-E2E-002 |
| **Test Case Name** | User Registration - Minimal Required Fields |
| **Priority** | P1 - High |
| **Pre-requisites** | None |

**Test Steps:**

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Navigate to login page --> Login/Signup page loads |
| 2 | Enter unique name and email --> Fields accept input |
| 3 | Click "Signup" --> Redirected to registration page |
| 4 | Fill only mandatory fields (Title, Password, Date of Birth, First Name, Last Name, Address, Country, State, City, Zipcode, Mobile Number) --> Fields filled |
| 5 | Leave newsletter checkboxes unchecked --> Checkboxes remain unchecked |
| 6 | Click "Create Account" --> Account created successfully |
| 7 | Verify "Account Created" message --> Success message displayed |

**Pass Criteria:** Account created with only required fields filled.

---

### TC-E2E-003: Login with Valid Credentials

| Field | Details |
|-------|---------|
| **Test Case ID** | TC-E2E-003 |
| **Test Case Name** | User Login - Valid Credentials |
| **Priority** | P0 - Critical |
| **Pre-requisites** | User must be already registered |

**Test Steps:**

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Navigate to login page | Login form displayed |
| 2 | Enter registered email address | Email accepted |
| 3 | Enter correct password | Password accepted (masked) |
| 4 | Click "Login" button | User logged in successfully |
| 5 | Verify "Logged in as [username]" message | Message visible in header |
| 6 | Verify "Logout" option is available | Logout button visible |

**Pass Criteria:** User successfully logged in with valid credentials.

---

### TC-E2E-004: Login with Invalid Credentials

| Field | Details |
|-------|---------|
| **Test Case ID** | TC-E2E-004 |
| **Test Case Name** | User Login - Invalid Credentials |
| **Priority** | P0 - Critical |
| **Pre-requisites** | None |

**Test Steps:**

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Navigate to login page | Login form displayed |
| 2 | Enter invalid email (e.g., `invalid@nonexistent.com`) | Email accepted |
| 3 | Enter incorrect password | Password accepted |
| 4 | Click "Login" button | Error message displayed |
| 5 | Verify "Your email or password is incorrect" message | Appropriate error shown |

**Pass Criteria:** System rejects invalid credentials with appropriate error message.

---

### TC-E2E-005: Add Multiple Products to Cart

| Field | Details |
|-------|---------|
| **Test Case ID** | TC-E2E-005 |
| **Test Case Name** | Add Multiple Products to Cart |
| **Priority** | P1 - High |
| **Pre-requisites** | User logged in |

**Test Steps:**

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Login to the application | Home page with logged-in state |
| 2 | Navigate to Products page | Product listing displayed |
| 3 | Add Product A to cart | Success message, cart updated |
| 4 | Continue shopping | Return to products page |
| 5 | Add Product B to cart | Success message, cart updated |
| 6 | Navigate to View Cart | Both products visible |
| 7 | Verify total price = Price A + Price B | Total calculated correctly |

**Pass Criteria:** Multiple products added with correct total calculation.

---

### TC-E2E-006: Update Product Quantity in Cart

| Field | Details |
|-------|---------|
| **Test Case ID** | TC-E2E-006 |
| **Test Case Name** | Update Cart Product Quantity |
| **Priority** | P1 - High |
| **Pre-requisites** | Product in cart |

**Test Steps:**

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Add product to cart | Product added successfully |
| 2 | Navigate to cart | Cart page displays product |
| 3 | Note initial quantity (default: 1) | Quantity visible |
| 4 | Change quantity to 3 | New quantity entered |
| 5 | Click "Update" button | Cart updated with new quantity |
| 6 | Verify total = unit price × 3 | Total reflects correct calculation |

**Pass Criteria:** Quantity updated and total recalculated correctly.

---

### TC-E2E-007: Remove Product from Cart

| Field | Details |
|-------|---------|
| **Test Case ID** | TC-E2E-007 |
| **Test Case Name** | Remove Product from Cart |
| **Priority** | P1 - High |
| **Pre-requisites** | Product in cart |

**Test Steps:**

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Add product to cart | Product added successfully |
| 2 | Navigate to cart | Product visible in cart |
| 3 | Click "X" or "Remove" button for product | Product removed from cart |
| 4 | Verify cart is empty or product removed | Cart reflects removal |
| 5 | Verify "Cart is empty" message | Appropriate message displayed |

**Pass Criteria:** Product successfully removed from cart.

---

### TC-E2E-008: Checkout with Empty Cart

| Field | Details |
|-------|---------|
| **Test Case ID** | TC-E2E-008 |
| **Test Case Name** | Checkout - Empty Cart Prevention |
| **Priority** | P2 - Medium |
| **Pre-requisites** | User logged in |

**Test Steps:**

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Login to the application | Logged in state |
| 2 | Navigate directly to cart (empty cart) | Empty cart message displayed |
| 3 | Attempt to click "Proceed to Checkout" button | Button should be disabled OR |
| 4 | Click "Proceed to Checkout" | Error message or prevented |

**Pass Criteria:** Checkout prevented with empty cart.

---

##  AI-ENHANCED TEST CASES

### TC-AI-001: Boundary Value Testing - Cart Quantity Limits

| Field | Details |
|-------|---------|
| **Test Case ID** | TC-AI-001 |
| **Test Case Name** | Cart Quantity - Boundary Value Analysis |
| **Priority** | P2 - Medium |
| **AI Contribution** | Edge case identification, boundary value analysis |

**Test Scenarios:**

| Scenario | Quantity Input | Expected Result |
|----------|----------------|-----------------|
| Minimum | 0 | Product removed or error displayed |
| Just above minimum | 1 | Accepted (normal case) |
| Typical value | 5 | Accepted |
| High value | 99 | Accepted if within limits |
| Maximum allowed | 100 (if limit exists) | Accepted or error if exceeded |
| Above maximum | 101 | Error or capped at max |

**Test Steps:**

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Add product to cart | Product added successfully |
| 2 | Navigate to cart | Cart page displayed |
| 3 | Try setting quantity to 0 | Appropriate action (remove or error) |
| 4 | Try setting quantity to 101 | Error message or capped value |
| 5 | Verify negative values are blocked | Negative input rejected |

**AI Rationale:** Tests system behavior at limits to identify potential overflow issues or missing validations.

---

### TC-AI-002: Input Validation - Special Characters in Registration

| Field | Details |
|-------|---------|
| **Test Case ID** | TC-AI-002 |
| **Test Case Name** | Registration - Input Validation for Special Characters |
| **Priority** | P2 - Medium |
| **AI Contribution** | Security-focused input testing, XSS prevention verification |

**Test Scenarios:**

| Field | Test Input | Expected Result |
|-------|------------|-----------------|
| Name | `<script>alert('XSS')</script>` | Sanitized or rejected |
| Name | `'; DROP TABLE users; --` | Treated as plain text |
| Name | `Test@#$%^&*()` | Accepted or appropriate error |
| Address | `123 Main St<script>` | Sanitized |
| City | `New York<script>` | Sanitized |
| Mobile | `+1-234-567-8900` | Accepted (valid format) |

**Test Steps:**

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Navigate to signup page | Registration form displayed |
| 2 | Enter name with script tags | Input accepted or sanitized |
| 3 | Complete registration | Account created |
| 4 | View account details | Script tags escaped/rendered safely |

**AI Rationale:** Validates input sanitization to prevent XSS and SQL injection vulnerabilities.

---

### TC-AI-003: Email Format Validation

| Field | Details |
|-------|---------|
| **Test Case ID** | TC-AI-003 |
| **Test Case Name** | Registration - Email Format Validation |
| **Priority** | P1 - High |
| **AI Contribution** | Comprehensive email format testing |

**Test Scenarios:**

| Email Format | Expected Result |
|--------------|-----------------|
| `valid@email.com` | ✅ Accepted |
| `valid@email.co.uk` | ✅ Accepted |
| `invalid` | ❌ Rejected |
| `invalid@` | ❌ Rejected |
| `@email.com` | ❌ Rejected |
| `invalid@.com` | ❌ Rejected |
| `test@domain.com ` (trailing space) | ⚠️ Trimmed or rejected |
| `TEST@EMAIL.COM` (uppercase) | ✅ Accepted (case-insensitive) |
| `test+tag@email.com` | ✅ Accepted |
| `test@sub.domain.email.com` | ✅ Accepted |
| `test@email..com` | ❌ Rejected |

**Test Steps:**

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Navigate to signup | Signup form displayed |
| 2 | Test each email format | Correct acceptance/rejection |
| 3 | Verify error messages | Clear, user-friendly messages |

---

### TC-AI-004: Password Strength Validation

| Field | Details |
|-------|---------|
| **Test Case ID** | TC-AI-004 |
| **Test Case Name** | Registration - Password Strength Validation |
| **Priority** | P1 - High |
| **AI Contribution** | Security best practice testing |

**Test Scenarios:**

| Password | Complexity | Expected Result |
|----------|------------|-----------------|
| `12345` | Weak | ⚠️ Warning or accepted with notice |
| `password` | Weak | ⚠️ Warning or rejected |
| `P@ssw0rd` | Medium | ✅ Accepted |
| `Str0ng!P@ss#2024` | Strong | ✅ Accepted |
| Empty | None | ❌ Rejected |
| `   ` (spaces only) | Weak | ❌ Rejected |
| Less than 6 chars | Too short | ❌ Rejected |

---

### TC-AI-005: Session Management - Concurrent Login

| Field | Details |
|-------|---------|
| **Test Case ID** | TC-AI-005 |
| **Test Case Name** | Session - Concurrent Login Handling |
| **Priority** | P2 - Medium |
| **AI Contribution** | Session behavior analysis |

**Test Scenarios:**

| Scenario | Expected Behavior |
|----------|-------------------|
| Login from two different browsers simultaneously | Both sessions active OR previous session terminated |
| Close browser without logging out | Session timeout after inactivity |
| Click "Remember Me" and close browser | Session persists across browser restart |
| Login after session timeout | Redirected to login page |

**Test Steps:**

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Login with "Remember Me" | Logged in successfully |
| 2 | Close browser completely | - |
| 3 | Reopen browser and navigate to site | User remains logged in OR prompted to login |
| 4 | Verify session handling | Correct behavior based on implementation |

---

### TC-AI-006: UI/UX - Responsive Design Testing

| Field | Details |
|-------|---------|
| **Test Case ID** | TC-AI-006 |
| **Test Case Name** | Cross-Device - Responsive UI Behavior |
| **Priority** | P2 - Medium |
| **AI Contribution** | Device-specific edge case identification |

**Test Scenarios:**

| Device/Viewport | Screen Width | Expected Behavior |
|-----------------|--------------|-------------------|
| Desktop | 1920px | Full layout, all elements visible |
| Laptop | 1366px | Full layout maintained |
| Tablet landscape | 1024px | Responsive layout, may stack elements |
| Tablet portrait | 768px | Mobile-optimized layout |
| Mobile Large | 425px | All elements accessible, no horizontal scroll |
| Mobile Small | 320px | Minimal required elements, readable text |

**Key Elements to Verify:**
- [ ] Navigation menu collapses properly
- [ ] Product grid adjusts columns (3 → 2 → 1)
- [ ] Buttons remain tappable (min 44px touch target)
- [ ] Text remains readable (min 16px font)
- [ ] Cart icon accessible on mobile
- [ ] Forms are usable without horizontal scrolling

---

### TC-AI-007: Error Handling - Network Failure During Checkout

| Field | Details |
|-------|---------|
| **Test Case ID** | TC-AI-007 |
| **Test Case Name** | Checkout - Network Failure Handling |
| **Priority** | P1 - High |
| **AI Contribution** | Failure scenario coverage |

**Test Scenarios:**

| Scenario | Network Condition | Expected Behavior |
|----------|-------------------|-------------------|
| Slow network | 2G connection | Loading indicator displayed, operation completes |
| Connection timeout | Network timeout | Error message with retry option |
| Payment gateway failure | 500 error | Clear error, cart data preserved |
| Session expiry during checkout | Session timeout | Redirected to login, cart preserved |

**Test Steps:**

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Add product to cart | Product added |
| 2 | Start checkout process | Checkout form displayed |
| 3 | Simulate network failure | Appropriate error displayed |
| 4 | Verify cart data preserved | Products still in cart |
| 5 | Retry checkout | Checkout resumes successfully |

---

### TC-AI-008: Data Persistence - Cart After Browser Close

| Field | Details |
|-------|---------|
| **Test Case ID** | TC-AI-008 |
| **Test Case Name** | Cart - Data Persistence Across Sessions |
| **Priority** | P1 - High |
| **AI Contribution** | State management verification |

**Test Scenarios:**

| Scenario | Expected Behavior |
|----------|-------------------|
| Add items, close browser, reopen | Cart items preserved (localStorage/session) |
| Add items, clear browser cache | Cart items cleared |
| Add items, incognito mode, close | Cart items cleared |
| Login before adding items | Cart items saved to account |

---

### TC-AI-009: Price Calculation Accuracy

| Field | Details |
|-------|---------|
| **Test Case ID** | TC-AI-009 |
| **Test Case Name** | Cart - Price Calculation Precision |
| **Priority** | P0 - Critical |
| **AI Contribution** | Financial calculation edge cases |

**Test Scenarios:**

| Scenario | Input | Expected Result |
|----------|-------|-----------------|
| Single item | ₹500 × 1 | ₹500 |
| Multiple quantity | ₹500 × 3 | ₹1500 |
| Decimal pricing | ₹499.99 × 2 | ₹999.98 (not rounded) |
| Currency symbol | ₹1,234.56 | Proper formatting |
| Very large quantity | ₹100 × 1000 | ₹100,000 |
| Empty cart total | No items | ₹0 or "Free" |

---

### TC-AI-010: Accessibility - Screen Reader Compatibility

| Field | Details |
|-------|---------|
| **Test Case ID** | TC-AI-010 |
| **Test Case Name** | Accessibility - Screen Reader Testing |
| **Priority** | P2 - Medium |
| **AI Contribution** | WCAG compliance verification |

**Test Elements:**

| Element | Accessibility Check |
|----------|---------------------|
| Images | Alt text present and descriptive |
| Form fields | Labels properly associated |
| Buttons | Clear, descriptive text |
| Links | Meaningful link text (not "click here") |
| Headings | Proper H1-H6 hierarchy |
| Color contrast | Minimum 4.5:1 ratio |
| Focus indicators | Visible focus states |
| Error messages | Associated with form fields |

---

## 📊 Test Summary Matrix

| Category | Test Cases | 
|----------|------------|
| Manual Test Cases --> 8 
| AI-Enhanced Test Cases --> 10 
| **Total** | **18** | |

---

## Test Execution Order (Recommended)

```
Phase 1: Authentication (P0)
├── TC-E2E-003: Valid Login
├── TC-E2E-004: Invalid Login
└── TC-E2E-001: Registration Flow

Phase 2: Core E2E Flow (P0)
├── TC-E2E-001: Complete Purchase (Full Run)
├── TC-E2E-005: Multiple Products
├── TC-E2E-006: Quantity Update
└── TC-E2E-007: Remove Product

Phase 3: Validation & Security (P1)
├── TC-AI-002: Input Validation
├── TC-AI-003: Email Validation
├── TC-AI-004: Password Strength
└── TC-AI-009: Price Calculation

Phase 4: Edge Cases & UX (P2)
├── TC-AI-001: Boundary Values
├── TC-AI-005: Session Management
├── TC-AI-006: Responsive Design
└── TC-AI-010: Accessibility
```



### User Registration Test Data

| Field | Valid Data | Invalid Data |
|-------|------------|--------------|
| Name | `John Doe` | `` (empty), `<script>` |
| Email | `john@example.com` | `invalid`, `@test.com`, `test@.com` |
| Password | `P@ssw0rd123` | `123`, `password`, `` (empty) |
| Mobile | `+1234567890` | `abc`, `` (empty) |
| Zipcode | `12345` | `abc`, `` (empty) |

### Payment Test Data

| Field | Valid Test Data |
|-------|-----------------|
| Card Number | `4111111111111111` (Visa test) |
| CVV | `123` |
| Expiry | `12/25` |
| Holder Name | `JOHN DOE` |

