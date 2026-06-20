QA Manual Test Cases
Member Name: Soumitra Dhar

URL:https://demowebshop.tricentis.com/

Human Thinking Test Cases

TC-001 (Verify user can register successfully)
Preconditions: User is on the homepage
Steps to execute: Click Register → Enter valid details → Submit

TC-002 (Verify mandatory fields validation in registration)
Preconditions: User is on the registration page
Steps to execute: Click Register without data

TC-003 (Verify valid login functionality)
Preconditions: User must be registered
Steps to execute: Enter valid credentials → Login

TC-004 (Verify invalid login error message)
Preconditions: User is on the login page
Steps to execute: Enter invalid credentials → Login

TC-005 (Verify search with valid product name)
Preconditions: User is on the homepage
Steps to execute: Enter product name → Search

TC-006 (Verify search with invalid product name)
Preconditions: User is on the homepage
Steps to execute: Enter random text → Search

TC-007 (Verify add product to cart)
Preconditions: User is logged in
Steps to execute: Open product → Click Add to Cart

TC-008 (Verify cart quantity update)
Preconditions: Product in cart
Steps to execute: Update quantity in cart

TC-009 (Verify checkout process)
Preconditions: Items in cart
Steps to execute: Go to checkout → Enter details → Confirm

TC-010 (Verify checkout without login)
Preconditions: User not logged in
Steps to execute: Try to check out

TC-011 (Verify homepage layout alignment)
Preconditions: Open homepage
Steps to execute: Check UI alignment

TC-012 (Verify responsiveness)
Preconditions: Open the site in mobile view
Steps to execute: Resize the browser

TC-013 (Verify logout functionality)
Preconditions: User is logged in
Steps to execute: Click Logout

TC-014 (Verify registration with empty fields)
Preconditions: User is on the registration page
Steps to execute: Click Register without data

TC-015 (Verify invalid email format)
Preconditions: User is on the registration page
Steps to execute: Enter an invalid email

TC-016 (Verify registration with existing email)\
Preconditions: Email already exists
Steps to execute: Register with existing email

TC-017 (Verify password mismatch)
Preconditions: User is on the registration page
Steps to execute: Enter a different password and confirm password

TC-018 (Verify login with invalid credentials)
Preconditions: User is on the login page
Steps to execute: Enter wrong credentials

TC-019 (Verify login with empty fields)
Preconditions: User is on the login page
Steps to execute: Click login without data

TC-020 (Verify login with unregistered email)
Preconditions: User is on the login page
Steps to execute: Enter a random email

TC-021 (Verify search with special characters)
Preconditions: User is on homepage
Steps to execute: Enter @@###

TC-022 (Verify search with long input)
Preconditions: User is on homepage
Steps to execute: Enter very long string

TC-023 (Verify adding out-of-stock product)
Preconditions: Product unavailable
Steps to execute: Try to add product

TC-024 (Verify invalid cart quantity)
Preconditions: Product in cart
Steps to execute: Enter -1 or alphabets

TC-025 (Verify checkout with empty cart)
Preconditions: Cart is empty
Steps to execute: Go to checkout

TC-026 (Verify incomplete address)
Preconditions: In checkout
Steps to execute: Leave mandatory fields empty

TC-027 (Verify payment failure)
Preconditions: Items in cart
Steps to execute: Enter invalid payment details

TC-028 (Verify UI on very small screen)
Preconditions: Open the site in mobile view
Steps to execute: Resize to 320px



												
													
