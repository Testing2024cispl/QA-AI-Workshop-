# Assignment Submission: End-to-End Test Cases for BlazeDemo.com

**Member:- Raktim Banerjee**  
**Query/Test cases:- BlazeDemo.com** (Write test cases based on your given website)

---

## Human Thinking Test Cases

### TestCases_001: Verify departure city selection with no destination
1. Go to BlazeDemo.com
2. Select "Paris" from the "Choose your departure city" dropdown.
3. Leave the "Choose your destination city" dropdown as the default (e.g., "Buenos Aires").
4. Click on the "Find Flights" button.
5. Verify that the user is navigated to the "Choose your destination city" page.
6. Verify that the selected departure city is correctly displayed on the new page.

### TestCases_002: Verify successful flight selection and reservation
1. Go to BlazeDemo.com
2. Select "Boston" from the departure cities.
3. Select "London" from the destination cities.
4. Click "Find Flights".
5. On the results page, click the "Choose This Flight" button for the first available flight.
6. On the purchase page, fill in all required fields (Name, Address, City, State, Zip Code, Card Type, Credit Card Number, Credit Card Month, Credit Card Year, Name on Card).
7. Click the "Purchase Flight" button.
8. Verify that the user is navigated to the confirmation page.
9. Verify that the confirmation page displays a success message (e.g., "Thank you for your purchase today!").
10. Verify that the flight details (e.g., Airline, Flight Number, Price) are displayed correctly.

### TestCases_003: Verify form validation on the purchase page
1. Go to BlazeDemo.com
2. Select "San Diego" as departure and "New York" as destination.
3. Click "Find Flights".
4. Click "Choose This Flight" for any available flight.
5. Leave all fields on the purchase form blank.
6. Click the "Purchase Flight" button.
7. Check if the page shows validation errors or if the form fails to submit, requiring mandatory fields to be filled.

---

## AI Manual Test Cases

**Member:- Raktim Banerjee**  
**Prompt:-** Write test cases for a complete End-to-End flight booking flow on BlazeDemo.com, from selecting cities to completing a purchase.

### TestCases_001: End-to-End Flight Booking Flow
1. Go to BlazeDemo.com
2. Select a departure city (e.g., "Mexico City").
3. Select a destination city (e.g., "Cairo").
4. Click on "Find Flights".
5. On the next page, verify that a list of available flights is displayed.
6. Select a flight by clicking the "Choose This Flight" button.
7. On the purchase page, fill in the passenger information form with valid data:
    - Name: John Doe
    - Address: 123 Main St
    - City: Anytown
    - State: CA
    - Zip Code: 12345
    - Card Type: Visa
    - Credit Card Number: 4111111111111111
    - Credit Card Month: 12
    - Credit Card Year: 2025
    - Name on Card: John Doe
8. Click the "Purchase Flight" button.
9. Verify that the user is redirected to a confirmation page.
10. Verify that the confirmation page contains a unique "Id" or confirmation number.
11. Verify that the confirmation page shows the total price and flight details.

### Your thoughts:
- **What you felt Suitable:** The AI test case correctly identifies the core E2E flow of a travel booking site: searching for flights, selecting one, and completing a purchase. It includes steps for verifying both success and key data (like flight ID and price), which are good for a robust automation script.

- **What you felt Not suitable:** The AI test case lacks "negative" test scenarios, such as verifying validation for empty fields, navigating back, or testing incorrect inputs. It also assumes the existence of specific test data (like a valid credit card), which might not be necessary for a simple demo site.

---

## Final Test Case

**AI + Manual, Combine them and make a proper test case for Automation ready.**

### TestCases_Final_001: Complete E2E Flight Booking with Positive & Negative Validation

**Objective:** To automate a full E2E booking flow, including error validation and successful purchase, on BlazeDemo.com.

**Pre-conditions:** The test environment is clean, and no prior session data interferes.

**Test Data:**
- Departure City: "San Diego"
- Destination City: "Dublin"
- Passenger Details: (Use static or generated data) e.g., Name: "Test User", Address: "123 Test Ave", City: "Testville", State: "CA", Zip: "90210", Card: "4242424242424242", Expiry: "12/2028".

**Automation Ready Test Steps:**

| Step | Action | Expected Result | Verification Point |
| :--- | :--- | :--- | :--- |
| 1 | Navigate to `https://blazedemo.com/`. | Homepage loads successfully. | Verify URL and page title. |
| 2 | Select a valid "Departure City" from the dropdown. | Value is selected. | Confirm selected option value. |
| 3 | Select a valid "Destination City" from the dropdown. | Value is selected. | Confirm selected option value. |
| 4 | Click the "Find Flights" button. | User is navigated to the flight results page (`/reserve.php`). | Verify URL contains `/reserve.php`. |
| 5 | Verify at least one flight is displayed in the results table. | Flight list is not empty. | Check for presence of flight rows or `//table/tbody/tr`. |
| 6 | Click the "Choose This Flight" button for the first flight. | User is navigated to the purchase page (`/purchase.php`). | Verify URL contains `/purchase.php`. Also, capture and store Flight Number/Price for later verification. |
| 7 | ***(Negative Check)*** Clear all form fields and click "Purchase Flight". | The form should fail to submit, or browser validation is triggered. (Note: BlazeDemo has no client-side validation, so it will submit with empty fields). | Observe behavior. As this site lacks validation, the script will proceed, but this step is added for manual clarity. The actual automation will proceed to step 8. |
| 8 | Fill in all mandatory fields on the purchase form with valid test data. | All fields are populated. | Verify text fields are not empty. |
| 9 | Click the "Purchase Flight" button. | User is navigated to the confirmation page (`/confirmation.php`). | Verify URL contains `/confirmation.php`. |
| 10 | Verify the success message is displayed on the confirmation page. | Text like "Thank you for your purchase today!" is visible. | Assert that the text is present on the page. |
| 11 | Verify the flight details on the confirmation page match those selected in Step 6. | Airline, Flight Number, and Price from Step 6 match the details on the final page. | Assert that the stored data from Step 6 is present on the page. |
| 12 | Verify a unique "Id" is displayed on the confirmation page. | A non-empty string is displayed as the order ID. | Assert that the element containing the ID is visible and not empty. |
