****QA Manual Test Cases
Project: DemoBlaze Testing Application: https://www.demoblaze.com/ 
Tester: Bisakha Pati**

**Human Thinking Test Cases**
**TestCases_001:-** (Valid login)
1. Go to https://www.demoblaze.com/
2. Click on "Log in"
3. Enter a valid registered Username and correct Password
4. Click on "Log in"
5. Verify the modal closes and the navbar shows "Welcome <username>" with "Log out" visible


**TestCases_002:-** (Wrong password)
1. Go to https://www.demoblaze.com/
2. Click on "Log in"
3. Enter a valid Username with an incorrect Password
4. Click on "Log in"
5. Verify the alert "Wrong password." is displayed


**TestCases_003:-** (Unknown user)
1. Go to https://www.demoblaze.com/
2. Click on "Log in"
3. Enter a Username that does not exist
4. Click on "Log in"
5. Verify the alert "User does not exist." is displayed


**TestCases_004:-** (Session persists + log out)
1. Go to https://www.demoblaze.com/
2. Log in with valid credentials
3. Refresh the page and navigate Home → Cart → Home
4. Verify the user stays logged in throughout
5. Click "Log out" and verify the logged-out state is restored


**TestCases_005:-** (Switch users — no state bleed)
1. Go to https://www.demoblaze.com/
2. Log in as User A, then click "Log out"
3. Log in as User B
4. Verify the navbar reflects only User B and no User-A session/cart data remains


==================================================================
## MODULE 2 — SIGN UP
=================================================================


**TestCases_006:-** (New user registration)
1. Go to https://www.demoblaze.com/
2. Click on "Sign up"
3. Enter a unique Username and a Password
4. Click on "Sign up"
5. Verify the alert "Sign up successful." is displayed


**TestCases_007:-** (Duplicate username)
1. Go to https://www.demoblaze.com/
2. Click on "Sign up"
3. Enter a Username that already exists
4. Click on "Sign up"
5. Verify the alert "This user already exist." is displayed


**TestCases_008:-** (Register then log in — end to end)
1. Go to https://www.demoblaze.com/
2. Register a new unique user
3. Click on "Log in" and enter the same credentials
4. Verify the login succeeds (account persisted correctly)


**TestCases_009:-** (No auto-login after signup)
1. Go to https://www.demoblaze.com/
2. Register a new user successfully
3. Verify the user is still logged OUT (navbar still shows "Log in" / "Sign up")


=================================================================
## MODULE 3 — HOME
==================================================================


**TestCases_010:-** (Default product load)
1. Go to https://www.demoblaze.com/
2. Wait for the homepage to load
3. Verify the product grid shows products with image, title, price, and description


**TestCases_011:-** (Category filtering)
1. Go to https://www.demoblaze.com/
2. Click "Phones", then "Laptops", then "Monitors"
3. Verify the grid shows only items of the selected category each time


**TestCases_012:-** (Open product detail)
1. Go to https://www.demoblaze.com/
2. Click on a product title/image
3. Verify the detail page opens with the correct name, price, description, image, and "Add to cart"


**TestCases_013:-** (Add to cart)
1. Go to https://www.demoblaze.com/
2. Open a product and click "Add to cart"
3. Verify the alert "Product added." is displayed
4. Open Cart and verify the product is listed


**TestCases_014:-** (Logo returns home)
1. Go to https://www.demoblaze.com/
2. Open any product detail page
3. Click the "PRODUCT STORE" logo
4. Verify it returns to the homepage with the full product list


==================================================================
## MODULE 4 — CONTACT
=================================================================


**TestCases_015:-** (Valid message send)
1. Go to https://www.demoblaze.com/
2. Click on "Contact"
3. Enter a valid Contact Email, Contact Name, and Message
4. Click on "Send message"
5. Verify the alert "Thanks for the message!!" is displayed and the modal closes


**TestCases_016:-** (Empty form submit — defect hunt)
1. Go to https://www.demoblaze.com/
2. Click on "Contact"
3. Leave Email, Name, and Message blank
4. Click on "Send message"
5. Verify the behavior (observed: "Thanks for the message!!" still fires — log as a defect: no validation)


**TestCases_017:-** (Dismiss without sending)
1. Go to https://www.demoblaze.com/
2. Click on "Contact"
3. Dismiss using "Close" and the ×
4. Verify the modal closes and nothing is sent


==================================================================
## MODULE 5 — ABOUT US
==================================================================


**TestCases_018:-** (Modal opens and video plays)
1. Go to https://www.demoblaze.com/
2. Click on "About us"
3. Verify the modal opens with the video player and click play
4. Verify the video plays and play/pause controls work


**TestCases_019:-** (Video stops on close — defect hunt)
1. Go to https://www.demoblaze.com/
2. Click on "About us" and start the video
3. Click "Close" or the ×
4. Verify the video stops (log a defect if audio continues after close)


**TestCases_020:-** (Reopen resets video)
1. Go to https://www.demoblaze.com/
2. Open About us, close it, then reopen it
3. Verify the video reloads/resets correctly with no double-audio


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

