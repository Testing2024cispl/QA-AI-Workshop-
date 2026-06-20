QA Member - Supravat Chakraborty

URL - https://automationexercise.com/ 

—----------------------------------------------------------------------------------------------------------------------------

Manual Test Scenarios

1. To check whether a user is able to login if they don’t have account
2. To check if user is able to register themselves
Verify mandatory field validations
Very email validation
Verify password validation
Verify age validation (if any)
Verify zip code field validation
Verify mobile number field validation
To check if registered users are able to login successfully
Verify with blank validation
Verify with valid credentials
Verify with invalid credentials
To check if user is able to logout
To check if user is able to search a product
To check if user is able to add products into carts (Single product)
Verify user is able to add a single product to cart
Verify user is able to delete that product from cart
Verify user added multiple products to cart and delete them except one
To check if user is able to add products into carts (multiple products)
Verify user is able to add multiple products to cart
Verify user is able to delete that products from cart
Verify user added multiple products to cart and delete them and add them again
To check if user is able to place an order with single product
Verify the check out page mandatory fields validation
Verify card field validation
Verify expiration date validation
Verify cvv validation
To check if user is able to place an order with multiple products
Verify the check out page mandatory fields validation
Verify card field validation
Verify expiration date validation
Verify cvv validation
To check if user is able to delete their account
To check if user is able to login with deleted user information
To check if user is able to place order without logged in

—----------------------------------------------------------------------------------------------------------------------------

AI Test Scenarios

A. Registration

Positive Scenarios

REG-001	Verify user can register with all mandatory valid details
REG-002	Verify user can register with all mandatory and optional fields populated
REG-003	Verify account is created successfully after submitting valid data
REG-004	Verify confirmation/success message is displayed after registration
REG-005	Verify registered user can log in using newly created credentials
REG-006	Verify email format validation accepts valid email formats
REG-007	Verify password meeting all policy requirements is accepted
REG-008	Verify registration works with minimum allowed password length
REG-009	Verify registration works with maximum allowed field lengths
REG-010	Verify leading/trailing spaces are handled correctly in non-password fields

Negative Scenarios

REG-011	Verify registration fails when mandatory fields are blank
REG-012	Verify registration fails with invalid email format
REG-013	Verify registration fails when email already exists
REG-014	Verify registration fails when password is below minimum length
REG-015	Verify registration fails when password does not meet complexity rules
REG-016	Verify registration fails when password and confirm password do not match
REG-017	Verify special character restrictions in name fields
REG-018	Verify numeric-only values are not accepted in name fields
REG-019	Verify registration fails when field length exceeds maximum allowed limit
REG-020	Verify registration fails when user submits empty form
REG-021	Verify registration fails when spaces are entered in mandatory fields
REG-022	Verify duplicate account creation is prevented
REG-023	Verify form validation messages are displayed correctly for each invalid field
REG-024	Verify Submit button behavior when mandatory fields are incomplete


B. Login

Positive Scenarios

Verify user can login with valid registered email and password
Verify user is redirected to appropriate landing page after login
Verify logged-in username/account information is displayed
Verify login works with remembered credentials if Remember Me feature exists
Verify user can access authorized pages after successful login

Negative Scenarios

Verify login fails with invalid email
Verify login fails with invalid password
Verify login fails when both email and password are invalid
Verify login fails when email field is blank
Verify login fails when password field is blank
Verify login fails when both fields are blank
Verify appropriate error message is displayed for invalid login
Verify login does not allow deleted account credentials
Verify email field validation for invalid email formats
Verify login fails for unregistered email address


C. Logout

Positive Scenarios

Verify logged-in user can logout successfully
Verify user is redirected to login/home page after logout
Verify session is terminated after logout
Verify cart data retention after logout as per business rules


Negative Scenarios

Verify user cannot access secured pages using browser back button after logout
Verify direct URL access to secured pages is blocked after logout
Verify session timeout behaves correctly if configured


D. Delete Account

Positive Scenarios

Verify logged-in user can delete account successfully
Verify confirmation message is displayed before account deletion
Verify account is permanently removed after confirmation
Verify user is logged out automatically after account deletion
Verify deleted account can no longer login
Verify deleted account data follows business retention rules

Negative Scenarios

Verify account deletion can be cancelled from confirmation popup
Verify unauthenticated users cannot access delete account functionality
Verify direct URL access to delete account page without login is restricted
Verify system handles deletion request failure gracefully
Verify multiple deletion requests do not create inconsistencies


E. Product Search

Positive Scenarios

Verify user can search using full product name
Verify user can search using partial product name
Verify search results display matching products
Verify search is not case-sensitive
Verify search works with product SKU if supported
Verify search works using category keywords
Verify search returns multiple matching products
Verify product details are accessible from search results
Verify search works after user login
Verify search works for guest users

Negative Scenarios

Verify no-result message is displayed for invalid keyword
Verify search handles special characters correctly
Verify search handles numeric-only input correctly
Verify search handles excessively long search strings
Verify search handles blank input appropriately
Verify search trims leading/trailing spaces
Verify search results do not show unrelated products
Verify search handles unsupported characters gracefully


F. Add to Cart

Positive Scenarios

Verify user can add a single product to cart
Verify user can add multiple different products to cart
Verify user can add multiple quantities of same product
Verify cart count updates correctly after adding products
Verify correct product details appear in cart
Verify correct quantity appears in cart
Verify correct subtotal calculation in cart
Verify guest user can add products to cart
Verify logged-in user can add products to cart
Verify cart persists during session as per business rules

Negative Scenarios

Verify out-of-stock products cannot be added to cart
Verify cart prevents quantity exceeding available stock
Verify invalid quantity values are rejected
Verify quantity cannot be zero
Verify quantity cannot be negative
Verify duplicate additions update quantity correctly
Verify cart handles product removal correctly
Verify cart updates correctly when product becomes unavailable


G. Purchase Order / Checkout

Positive Scenarios

Verify user can place order with valid shipping and payment details
Verify order confirmation page is displayed after successful purchase
Verify unique order number is generated
Verify purchased items match cart contents
Verify correct order total is calculated
Verify taxes are calculated correctly
Verify shipping charges are calculated correctly
Verify order details are saved successfully
Verify order confirmation email is sent
Verify inventory is updated after successful purchase
Verify user can place order with single product
Verify user can place order with multiple products
Verify billing and shipping address handling works correctly
Verify guest checkout functionality if supported
Verify registered user checkout functionality

Negative Scenarios

Verify checkout cannot proceed with empty cart
Verify checkout fails when mandatory shipping details are missing
Verify checkout fails when mandatory billing details are missing
Verify checkout fails with invalid payment information
Verify checkout fails when payment authorization is declined
Verify checkout fails when product becomes out of stock during checkout
Verify invalid postal code validation
Verify invalid phone number validation
Verify order is not created when payment fails
Verify duplicate order creation is prevented on multiple clicks of Place Order
Verify user receives proper error message when checkout fails
Verify session expiration during checkout is handled correctly
Verify cart remains intact when order submission fails
Verify system prevents purchase of removed/discontinued products
Verify order total is recalculated correctly after quantity changes during checkout


#End-to-End Business Flow Scenarios

Register → Login → Search Product → Add to Cart → Purchase Order → Logout
Register → Login → Add Multiple Products → Purchase Order
Guest User → Search Product → Add to Cart → Checkout
Login → Purchase Order → Logout → Login Again → Verify Order History
Register → Delete Account → Verify Login Not Allowed
Login → Add Products → Logout → Verify Cart Behavior as per Requirements
Search Product → Add to Cart → Remove Product → Verify Cart Updates
Checkout Failure → Verify Cart Retention → Retry Purchase Successfully


—-----------------------------------------------------------------------------------------------

Suitable Points

Human scenarios focus on real business workflows, while AI scenarios provide broader functional coverage. Together they create a balanced test suite.
Human scenarios include practical validations such as Card, CVV, ZIP Code, Mobile Number, and Login with Deleted Account, which enrich the overall coverage.
AI scenarios provide structured organization with modules, test case IDs, and clear positive/negative classifications, making them suitable for long-term regression testing.
AI scenarios cover edge cases such as payment failures, stock issues, duplicate orders, invalid searches, and session handling that humans often miss.
Combining both approaches results in comprehensive coverage of business flows, validations, negative testing, security checks, and end-to-end journeys.

Not Suitable Points

Human scenarios contain duplicate test cases, while AI scenarios may introduce unnecessary generic scenarios that are not part of the actual requirements.
Human scenarios lack proper categorization and positive/negative separation, making maintenance difficult.
AI-generated scenarios sometimes assume features that may not exist (e.g., Remember Me, Guest Checkout, Order History, Session Timeout).
Human scenarios focus mainly on happy paths and basic validations, leaving gaps in exception handling and security testing.
The merged list can become very large, requiring prioritization into Smoke, Sanity, Regression, and Full Functional suites before execution.


Human-generated scenarios = Strong business understanding, practical user flows.
AI-generated scenarios = Strong coverage, structure, edge cases, and maintainability.
Combined approach = Best practice for QA because it maximizes coverage while ensuring business relevance.

—---------------------------------------------------------------------------------------------
AI + Manual Test Scenarios (Merged)

1. Registration

Positive Scenarios

Verify user can register with all mandatory valid details
Verify user can register with all mandatory and optional fields populated
Verify account is created successfully after registration
Verify success/confirmation message is displayed
Verify newly registered user can login successfully
Verify registration works with minimum allowed password length
Verify registration works with maximum allowed field lengths
Verify leading/trailing spaces are handled correctly

Negative Scenarios

Verify mandatory field validations
Verify registration with blank form
Verify email field validation
Verify duplicate email registration is not allowed
Verify password validation rules
Verify password and confirm password mismatch validation
Verify age validation (if applicable)
Verify ZIP/Postal code validation
Verify mobile number validation
Verify name field validation (numeric/special characters restriction)
Verify maximum field length validation
Verify spaces-only values are rejected
Verify field-specific error messages are displayed correctly


2. Login

Positive Scenarios

Verify registered user can login with valid credentials
Verify successful login redirects user to correct page
Verify logged-in user information is displayed
Verify authenticated user can access secured pages

Negative Scenarios

Verify login attempt with unregistered account
Verify login with invalid email
Verify login with invalid password
Verify login with both invalid email and password
Verify login with blank email
Verify login with blank password
Verify login with both fields blank
Verify invalid email format validation
Verify login using deleted account credentials
Verify appropriate error message is displayed for invalid login


3. Logout

Positive Scenarios

Verify logged-in user can logout successfully
Verify user is redirected appropriately after logout
Verify session is terminated after logout

Negative Scenarios

Verify secured pages cannot be accessed after logout using browser back button
Verify secured URLs cannot be accessed directly after logout
Verify session timeout behavior works correctly


4. Product Search

Positive Scenarios

Verify user can search product using complete product name
Verify user can search product using partial product name
Verify search results display matching products
Verify search is case-insensitive
Verify search works for guest users
Verify search works for logged-in users
Verify user can open product details from search results

Negative Scenarios

Verify search with invalid keyword
Verify search with blank input
Verify search with special characters
Verify search with numeric-only input
Verify search with excessively long text
Verify unrelated products are not displayed
Verify leading/trailing spaces are handled correctly


5. Cart Management

Positive Scenarios

Verify user can add a single product to cart
Verify user can add multiple products to cart
Verify user can increase quantity of product
Verify cart count updates correctly
Verify product details are displayed correctly in cart
Verify subtotal calculation is correct
Verify logged-in user can add products to cart
Verify guest user can add products to cart
Verify user can remove a single product from cart
Verify user can remove all products from cart
Verify user can remove multiple products while retaining one product
Verify user can remove products and add them again successfully

Negative Scenarios

Verify out-of-stock products cannot be added to cart
Verify quantity cannot exceed available stock
Verify quantity cannot be zero
Verify quantity cannot be negative
Verify invalid quantity values are rejected
Verify cart updates correctly when product becomes unavailable


6. Checkout / Purchase Order

Positive Scenarios

Verify user can place order with a single product
Verify user can place order with multiple products
Verify order can be placed using valid shipping and billing information
Verify order confirmation page is displayed
Verify unique order number is generated
Verify purchased products match cart contents
Verify order total calculation is correct
Verify taxes are calculated correctly
Verify shipping charges are calculated correctly
Verify inventory is updated after successful order
Verify order confirmation email is sent
Verify registered user can complete checkout
Verify guest user can complete checkout (if supported)

Negative Scenarios

Verify checkout with empty cart is not allowed
Verify checkout mandatory field validations
Verify billing address validation
Verify shipping address validation
Verify ZIP/Postal code validation during checkout
Verify phone number validation during checkout
Verify card number validation
Verify expiration date validation
Verify CVV validation
Verify invalid payment information is rejected
Verify expired card is rejected
Verify payment decline is handled correctly
Verify order is not created when payment fails
Verify duplicate orders are not created by multiple clicks on Place Order
Verify cart remains intact after payment failure
Verify out-of-stock products cannot be purchased during checkout
Verify session expiration during checkout is handled correctly
Verify order placement without login (according to business rules)
Verify proper error message is displayed when checkout fails


7. Delete Account

Positive Scenarios

Verify logged-in user can delete account successfully
Verify confirmation prompt is displayed before deletion
Verify account is removed successfully after confirmation
Verify user is automatically logged out after account deletion

Negative Scenarios

Verify account deletion can be cancelled
Verify deleted account cannot login
Verify unauthenticated users cannot access delete account functionality
Verify direct URL access to delete account page is restricted
Verify system handles account deletion failure gracefully


8. End-to-End Scenarios

Register → Login → Search Product → Add Single Product → Checkout → Logout
Register → Login → Search Product → Add Multiple Products → Checkout
Guest User → Search Product → Add Product → Checkout
Login → Add Products → Remove Some Products → Checkout
Register → Delete Account → Verify Login Not Allowed
Login → Logout → Verify Secured Pages Are Not Accessible
Login → Add Product → Remove Product → Verify Cart Updates Correctly
Checkout Failure → Retry Checkout Successfully
Login → Add Multiple Products → Remove All Products → Verify Empty Cart
Place Order → Logout → Login Again → Verify Order History (if available)




