****QA Manual Test Cases
Project: DemoBlaze Testing Application: https://www.demoblaze.com/ 
Tester: Bisakha Pati**

**Human Thinking Test Cases**

## MODULE 1 — HOME
=====================================================================

TestCases_001:- Home page
1.Open https://www.demoblaze.com/
2.Verify by default it lands on the "Home" page.
3.Verify all the menus are there — Home, Contact, About us, Cart, Log in, 4.Sign up — and each one is clickable.
5.Verify the category filters — Phones, Laptops, Monitors — and after 6.clicking any filter it shows only that type of product.
7.Verify the carousel slides and Next/Previous work and images load fine.
8.Pick any product, open it, and verify the details page shows the correct image, price and description with an "Add to cart" button.
9.Add it to cart, verify the "Product added." message, and check it actually shows up in the Cart.
10.Click the logo and verify it brings you back to Home.

=====================================================================
## MODULE 2 — LOGIN
=====================================================================

TestCases_002:- Login
1.Click on Log in.
2.Verify login with valid credentials — should close the popup and show "Welcome <username>" with Log out.
3.Verify wrong password shows "Wrong password." and unknown user shows "User does not exist."
4.Verify blank fields shows "Please fill out Username and Password."
5.After logging in, refresh and move between pages — verify the session stays logged in.
6.Click Log out and verify it goes back to the logged-out state.

=====================================================================
## MODULE 3 — SIGN UP
=====================================================================

TestCases_003:- Sign up
1.Click on Sign up.
2.Verify a new unique username + password shows "Sign up successful."
3.Verify a duplicate username shows "This user already exist."
4.Verify blank fields shows "Please fill out Username and Password."
5.Verify that after signing up it does NOT auto-login (still shows Log in / Sign up).
6.Take the new credentials and log in with them — verify the account actually works.

=====================================================================
## MODULE 4 — CONTACT
=====================================================================

TestCases_004:- Contact
1.Click on Contact.
2.Verify sending a message with valid Email, Name and Message shows "Thanks for the message!!"
3.Verify what happens when all fields are blank and you hit Send — currently it still says "Thanks for the message!!" with no validation (raise as a bug).
4.Verify an invalid email format like "abc" is still accepted (raise as a bug/limitation).
5.Verify Close and the × dismiss the popup without sending.

=====================================================================
## MODULE 5 — ABOUT US
=====================================================================

TestCases_005:- About us
1.Click on About us.
2.Verify the popup opens with the video player.
3.Verify the video plays and play/pause controls work.
4.Verify clicking Close / × stops the video — check the audio doesn't keep playing in the background (raise as a bug if it does).
5.Verify reopening About us loads the video fresh with no double audio.

**AI Manual Test Cases**

## MODULE 1 — LOGIN
=================================================================
**TestCases_001:-** (Valid login — positive)
1. Go to https://www.demoblaze.com/
2. Click on "Log in"
3. Enter a valid Username and correct Password
4. Click on "Log in"
5. Verify successful login and "Welcome <username>" is shown


**TestCases_002:-** (Empty fields)
1. Go to https://www.demoblaze.com/
2. Click on "Log in"
3. Leave Username and Password blank
4. Click on "Log in"
5. Verify the alert "Please fill out Username and Password." is displayed


**TestCases_003:-** (Username only / Password only)
1. Go to https://www.demoblaze.com/
2. Click on "Log in"
3. Submit with Username only, then with Password only
4. Verify "Please fill out Username and Password." each time


**TestCases_004:-** (Password masking)
1. Go to https://www.demoblaze.com/
2. Click on "Log in"
3. Type characters into the Password field
4. Verify the characters are masked (shown as dots/asterisks)


**TestCases_005:-** (Cancel / dismiss)
1. Go to https://www.demoblaze.com/
2. Click on "Log in"
3. Dismiss using "Close" and then the ×
4. Verify the modal closes and no login occurs


==================================================================
## MODULE 2 — SIGN UP
====================================


**TestCases_006:-** (Valid registration — positive)
1. Go to https://www.demoblaze.com/
2. Click on "Sign up"
3. Enter a unique Username and Password
4. Click on "Sign up"
5. Verify the alert "Sign up successful." is displayed


**TestCases_007:-** (Duplicate username)
1. Go to https://www.demoblaze.com/
2. Click on "Sign up"
3. Enter a Username that already exists
4. Click on "Sign up"
5. Verify the alert "This user already exist." is displayed


**TestCases_008:-** (Empty fields)
1. Go to https://www.demoblaze.com/
2. Click on "Sign up"
3. Leave both fields blank and click "Sign up"
4. Verify the alert "Please fill out Username and Password." is displayed


**TestCases_009:-** (Username only / Password only)
1. Go to https://www.demoblaze.com/
2. Click on "Sign up"
3. Submit with Username only, then with Password only
4. Verify "Please fill out Username and Password." each time


==================================================================
## MODULE 3 — HOME
=================================================================


**TestCases_010:-** (Navbar links)
1. Go to https://www.demoblaze.com/
2. Click Home, Contact, About us, Cart, Log in, and Sign up
3. Verify each link opens its correct page/modal


**TestCases_011:-** (Each category individually)
1. Go to https://www.demoblaze.com/
2. Click "Phones" and verify only phones display
3. Click "Laptops" and verify only laptops display
4. Click "Monitors" and verify only monitors display


**TestCases_012:-** (Pagination Next/Previous)
1. Go to https://www.demoblaze.com/
2. Click "Next", then "Previous"
3. Verify the product set changes correctly with no duplicate or blank cards


**TestCases_013:-** (Carousel controls)
1. Go to https://www.demoblaze.com/
2. Use the carousel Next/Previous controls and the indicators
3. Verify the slides change accordingly


**TestCases_014:-** (Product card + open detail)
1. Go to https://www.demoblaze.com/
2. Verify each product card shows image, name, price, and description
3. Click a product and verify the detail page opens with matching data


==================================================================
## MODULE 4 — CONTACT
==================================================================


**TestCases_015:-** (Valid message send)
1. Go to https://www.demoblaze.com/
2. Click on "Contact"
3. Enter a valid Email, Name, and Message
4. Click on "Send message"
5. Verify the alert "Thanks for the message!!" is displayed


**TestCases_016:-** (Single-field-empty validation)
1. Go to https://www.demoblaze.com/
2. Click on "Contact"
3. Submit with Email empty only, then Name empty only, then Message empty only
4. Verify and document the validation behavior in each case


**TestCases_017:-** (Dismiss without sending)
1. Go to https://www.demoblaze.com/
2. Click on "Contact"
3. Dismiss using "Close" and the ×
4. Verify the modal closes and nothing is sent


==================================================================
## MODULE 5 — ABOUT US
==================================================================


**TestCases_018:-** (Modal opens / video loads)
1. Go to https://www.demoblaze.com/
2. Click on "About us"
3. Verify the modal opens and the video player/source loads without error


**TestCases_019:-** (Playback controls)
1. Go to https://www.demoblaze.com/
2. Click on "About us"
3. Use play, pause, and seek controls
4. Verify each control functions correctly


**TestCases_020:-** (Reopen + dismiss paths)
1. Go to https://www.demoblaze.com/
2. Open About us, close it, then reopen it
3. Dismiss using "Close" and the ×
4. Verify the modal resets on reopen and closes consistently each time


**Final Test Cases**

## MODULE 1 — LOGIN
=========================================================
**TestCases_001:-** (H) Valid login
1. Go to https://www.demoblaze.com/
2. Click on "Log in" and enter a valid Username and correct Password
3. Click on "Log in"
4. Verify the modal closes and "Welcome <username>" with "Log out" is shown


**TestCases_002:-** (H) Wrong password / unknown user
1. Go to https://www.demoblaze.com/
2. Log in with a valid Username but wrong Password
3. Verify the alert "Wrong password."
4. Log in with a Username that does not exist
5. Verify the alert "User does not exist."


**TestCases_003:-** (AI) Empty / single-field validation
1. Go to https://www.demoblaze.com/
2. Click on "Log in"
3. Submit blank, then Username-only, then Password-only
4. Verify "Please fill out Username and Password." each time


**TestCases_004:-** (H) Session persists + log out
1. Go to https://www.demoblaze.com/
2. Log in, refresh, and navigate Home → Cart → Home
3. Verify the user stays logged in
4. Click "Log out" and verify the logged-out state is restored


**TestCases_005:-** (H) Switch users — no state bleed
1. Go to https://www.demoblaze.com/
2. Log in as User A → Log out → Log in as User B
3. Verify no cart/session data from User A remains


=====================================================================
## MODULE 2 — SIGN UP
=====================================================================


**TestCases_006:-** (H) New user registration
1. Go to https://www.demoblaze.com/
2. Click on "Sign up" and enter a unique Username and Password
3. Click on "Sign up"
4. Verify the alert "Sign up successful."


**TestCases_007:-** (H) Duplicate username
1. Go to https://www.demoblaze.com/
2. Click on "Sign up" and enter an existing Username
3. Click on "Sign up"
4. Verify the alert "This user already exist."


**TestCases_008:-** (AI) Empty / single-field validation
1. Go to https://www.demoblaze.com/
2. Click on "Sign up"
3. Submit blank, then Username-only, then Password-only
4. Verify "Please fill out Username and Password." each time


**TestCases_009:-** (H+AI) Register then log in — end to end
1. Go to https://www.demoblaze.com/
2. Register a new unique user
3. Click on "Log in" and enter the same credentials
4. Verify the login succeeds (account persisted)


**TestCases_010:-** (H) No auto-login after signup
1. Go to https://www.demoblaze.com/
2. Register a new user successfully
3. Verify the user is still logged out


=====================================================================
## MODULE 3 — HOME
=====================================================================


**TestCases_011:-** (H) Default product load + data sanity
1. Go to https://www.demoblaze.com/
2. Verify products load with image, title, price, and description
3. Verify no missing titles, broken images, or invalid prices


**TestCases_012:-** (H+AI) Category filtering
1. Go to https://www.demoblaze.com/
2. Click "Phones", "Laptops", "Monitors" in turn
3. Verify the grid is scoped to the selected category each time


**TestCases_013:-** (H) Category + pagination scoping
1. Go to https://www.demoblaze.com/
2. Select a category, then click "Next"
3. Verify pagination stays within that category (no other categories leak in)


**TestCases_014:-** (AI) Pagination + carousel controls
1. Go to https://www.demoblaze.com/
2. Click "Next" then "Previous" on the product grid
3. Use the carousel Next/Previous and indicators
4. Verify both navigate correctly with no duplicate/blank cards


**TestCases_015:-** (H) Open product detail + add to cart
1. Go to https://www.demoblaze.com/
2. Open a product and verify name, price, description, image
3. Click "Add to cart" and verify "Product added." and the Cart updates


**TestCases_016:-** (AI) Navbar links + logo
1. Go to https://www.demoblaze.com/
2. Click each navbar link, then click the "PRODUCT STORE" logo
3. Verify each link works and the logo returns to home


=====================================================================
## MODULE 4 — CONTACT
=====================================================================


**TestCases_017:-** (H) Valid message send
1. Go to https://www.demoblaze.com/
2. Click on "Contact", fill Email, Name, and Message
3. Click on "Send message"
4. Verify the alert "Thanks for the message!!" and the modal closes


**TestCases_018:-** (H) Empty-form submit — defect hunt
1. Go to https://www.demoblaze.com/
2. Click on "Contact", leave all fields blank
3. Click on "Send message"
4. Verify behavior (currently accepted with no validation — log the defect)


**TestCases_019:-** (AI) Single-field-empty + dismiss
1. Go to https://www.demoblaze.com/
2. Click on "Contact"
3. Submit with each field empty in turn and document the result
4. Dismiss via "Close" / × and verify nothing is sent


=====================================================================
## MODULE 5 — ABOUT US
=====================================================================


**TestCases_020:-** (H) Modal opens and video plays
1. Go to https://www.demoblaze.com/
2. Click on "About us" and click play
3. Verify the player is shown and playback (play/pause) works


**TestCases_021:-** (H+AI) Video stops on close
1. Go to https://www.demoblaze.com/
2. Click on "About us", play the video, then click "Close" / ×
3. Verify the video stops; if audio persists, log the defect


**TestCases_022:-** (AI) Reopen reset + dismiss paths
1. Go to https://www.demoblaze.com/
2. Open About us, close and reopen it
3. Dismiss using "Close" and the ×
4. Verify the video resets on r

