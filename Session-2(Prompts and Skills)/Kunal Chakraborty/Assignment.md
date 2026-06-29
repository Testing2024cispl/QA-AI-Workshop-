# Skill: Create New Account on Advantage Online Shopping

## Skill ID

SKILL_REG_001

## Skill Title

Create a new user account on Advantage Online Shopping.

## Skill Description

This skill verifies that a new user can successfully register an account on the Advantage Online Shopping website by entering valid account, personal, and address details, accepting the required terms, and confirming that the account is created and accessible.

## Prerequisites

1. The user is not logged in.
2. The website is accessible.
3. Valid and unique registration data is available.

## Required Test Data

* Username: Unique username
* Email: Valid unique email address
* Password: Valid password meeting system requirements
* First Name: Test
* Last Name: User
* Phone Number: Valid phone number
* Country: Any valid country
* City: Valid city
* Address: Valid address
* State/Province: Valid state
* Postal Code: Valid postal code

## Skill Steps

| Step No. | Action                                                                      | Expected Result                                        |
| -------- | --------------------------------------------------------------------------- | ------------------------------------------------------ |
| 1        | Open https://advantageonlineshopping.com                                    | Homepage loads successfully.                           |
| 2        | Click the User icon located at the top-right corner of the page.            | Login/Registration popup is displayed.                 |
| 3        | Click "CREATE NEW ACCOUNT".                                                 | Registration page/form is displayed.                   |
| 4        | Verify all account, personal, and address detail fields are visible.        | All required fields are displayed correctly.           |
| 5        | Enter a valid unique Username.                                              | Username is accepted without validation errors.        |
| 6        | Enter a valid Email Address.                                                | Email is accepted.                                     |
| 7        | Enter a valid Password.                                                     | Password meets complexity requirements.                |
| 8        | Re-enter the same password in the Confirm Password field.                   | Password confirmation is accepted.                     |
| 9        | Enter First Name and Last Name.                                             | Values are accepted.                                   |
| 10       | Enter Phone Number.                                                         | Value is accepted.                                     |
| 11       | Enter Country, City, Address, State, and Postal Code.                       | Address details are accepted.                          |
| 12       | Verify the Terms & Conditions checkbox is displayed.                        | Checkbox is visible and selectable.                    |
| 13       | Select the final Terms & Conditions checkbox.                               | Checkbox becomes checked.                              |
| 14       | Click the REGISTER button.                                                  | Registration request is submitted successfully.        |
| 15       | Verify successful account creation message or successful redirection.       | User receives confirmation of successful registration. |
| 16       | Verify user is automatically logged in.                                     | User account/profile icon displays logged-in status.   |
| 17       | Navigate to My Account/Profile page.                                        | Profile page opens successfully.                       |
| 18       | Verify First Name, Last Name, Email, and Username match the entered values. | Stored account information is displayed correctly.     |
| 19       | Log out of the application.                                                 | User is logged out successfully.                       |
| 20       | Log in using the newly created username and password.                       | Login is successful.                                   |
| 21       | Verify the correct username/account is displayed after login.               | Newly created account is accessible and active.        |

## Expected Outcome

A new user account is created successfully, the user can log in with the registered credentials, and all entered account details are stored correctly.

## Postconditions

1. A new user account exists in the system.
2. The user can authenticate using the newly created credentials.

