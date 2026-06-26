# Search and Login Test Cases

## My Own Test Cases

### Search

#### Positive Scenarios

  -----------------------------------------------------------------------
  TC ID                   Test Case               Expected Result
  ----------------------- ----------------------- -----------------------
  SEARCH_001              Search using a valid    Relevant product
                          product name            displayed

  SEARCH_002              Search using partial    Matching products
                          product name            displayed

  SEARCH_003              Search using product    Relevant products
                          keyword                 displayed

  SEARCH_004              Search and click on a   Product detail page
                          result                  opens

  SEARCH_005              Search with different   Correct products
                          product categories      displayed
  -----------------------------------------------------------------------

#### Negative Scenarios

  -----------------------------------------------------------------------
  TC ID                   Test Case               Expected Result
  ----------------------- ----------------------- -----------------------
  SEARCH_006              Search for non-existing "No products found"
                          product                 message displayed

  SEARCH_007              Search with random text No results displayed

  SEARCH_008              Search with special     Proper validation or no
                          characters only         results

  SEARCH_009              Search with blank input System behaves as per
                                                  requirement

  SEARCH_010              Search with spaces only Validation or no
                                                  results
  -----------------------------------------------------------------------

### Login

#### Positive Scenarios

  -----------------------------------------------------------------------
  TC ID                   Test Case               Expected Result
  ----------------------- ----------------------- -----------------------
  LOGIN_001               Login with valid email  User logs in
                          and valid password      successfully

  LOGIN_002               Login using registered  User redirected to
                          user credentials        account/dashboard page

  LOGIN_003               Verify logout after     User logged out
                          successful login        successfully

  LOGIN_004               Verify Remember Me      User remains logged in
                          option                  after browser restart
  -----------------------------------------------------------------------

#### Negative Scenarios

  -----------------------------------------------------------------------
  TC ID                   Test Case               Expected Result
  ----------------------- ----------------------- -----------------------
  LOGIN_005               Valid email + invalid   Error message displayed
                          password                

  LOGIN_006               Invalid email + valid   Error message displayed
                          password                

  LOGIN_007               Invalid email + invalid Error message displayed
                          password                

  LOGIN_008               Empty email field       Validation message
                                                  displayed

  LOGIN_009               Empty password field    Validation message
                                                  displayed

  LOGIN_010               Empty email and         Validation message
                          password                displayed

  LOGIN_011               Unregistered email      Error message displayed

  LOGIN_012               Password case           Login should fail if
                          sensitivity check       password case is
                                                  incorrect
  -----------------------------------------------------------------------

## AI Generated Additional Test Cases

### Search

#### Functional (SEARCH_011--022)

-   Exact product name, partial keyword, uppercase, lowercase, mixed
    case, leading/trailing spaces, SKU, category keyword, Enter key,
    Search button, repeated searches.

#### Validation (SEARCH_023--030)

-   Empty input, single character, max length, over max length, numeric,
    alphanumeric, special characters, Unicode.

#### Result Accuracy (SEARCH_031--036)

-   Relevant results, irrelevant products excluded, result count,
    sorting, pagination, product details.

#### Security (SEARCH_037--041)

-   SQL Injection, UNION Injection, XSS, HTML injection, long malicious
    payload.

#### Performance (SEARCH_042--046)

-   Large catalog, concurrent users, repeated searches, slow network,
    SLA.

#### UI/UX (SEARCH_047--051)

-   Search box alignment, placeholder, search icon, clear input, layout.

#### Accessibility (SEARCH_052--054)

-   Keyboard navigation, screen reader, tab order.

### Login

#### Functional (LOGIN_013--019)

-   Leading/trailing spaces, password spaces, uppercase email, Enter
    key, copy-paste, refresh after login.

#### Validation (LOGIN_020--024)

-   Invalid email formats, email/password length, special characters.

#### Security (LOGIN_025--032)

-   SQL Injection, XSS, unauthorized URL access, back after logout,
    failed attempts, session timeout, password protection.

#### Session Management (LOGIN_033--036)

-   Multiple tabs, multiple browsers, browser close, logout
    synchronization.

#### Performance (LOGIN_037--040)

-   Slow network, concurrent logins, response time, high load.

#### Accessibility (LOGIN_041--043)

-   Tab navigation, screen reader, keyboard-only login.




==============================================================seassion2===========================================================================
# QA Test Case Generator Skill

## Role

Act as a Senior QA Automation Engineer.

## Objective

Generate comprehensive, automation-ready test cases for any given
requirement, user story, feature, API, or application module.

## Test Coverage

### Functional

-   Positive scenarios
-   Negative scenarios
-   End-to-end workflows
-   CRUD operations
-   Business rules
-   Workflow validation
-   State transition validation

### Field Validation

-   Mandatory fields
-   Optional fields
-   Empty values
-   Null values
-   Invalid values
-   Default values
-   Duplicate values
-   Numeric inputs
-   Alphanumeric inputs
-   Special characters
-   Unicode characters
-   Copy-paste
-   Leading/trailing spaces
-   Character restrictions

### Boundary Value Analysis

-   Minimum value
-   Maximum value
-   Just below minimum
-   Just above minimum
-   Minimum length
-   Maximum length
-   Just below maximum length
-   Just above maximum length

### Edge Cases

-   Empty data
-   Null data
-   Large inputs
-   Multiple rapid actions
-   Simultaneous users
-   Browser refresh
-   Browser back
-   Session interruption
-   Timeout
-   Network interruption

### Authentication & Authorization

-   Login required
-   Invalid credentials
-   Session timeout
-   Token expiration
-   Unauthorized access
-   Role-based access
-   Logout validation

### Error Handling

-   Proper error messages
-   Validation messages
-   Graceful failures
-   Retry behavior
-   Unexpected inputs

### Security Functional Checks

-   SQL Injection
-   XSS
-   HTML Injection
-   Script Injection
-   Direct URL access
-   Authorization validation
-   Session validation
-   Sensitive data exposure
-   Input sanitization

### API Checks

-   Status code
-   Response schema
-   Response body
-   Data types
-   Required/optional fields
-   Response headers
-   Content-Type
-   Response time
-   Authentication
-   Authorization
-   Pagination
-   Filtering
-   Sorting
-   Rate limiting
-   Idempotency
-   Error responses
-   JSON/XML output validation

### Non-Functional

-   Performance
-   Load
-   Stress
-   Scalability
-   Reliability
-   Recovery
-   Compatibility
-   Cross-browser
-   Responsive UI
-   Accessibility

### UI/UX

-   Alignment
-   Labels
-   Placeholder
-   Icons
-   Responsive layout
-   Mobile/Tablet/Desktop
-   Error message placement
-   User friendliness

### Accessibility

-   Keyboard navigation
-   Screen reader
-   Tab order
-   Focus visibility
-   WCAG compliance

## Automation Readiness

-   One validation per test case
-   Stable locators where applicable
-   Deterministic expected results
-   Reusable test data
-   Independent test cases
-   Suitable for Playwright, Selenium, Cypress, Appium, and API
    automation

## Output Format

Generate the output as a Markdown table using the following columns:

| Sl No \| Test Scenario ID \| Test Scenario Name \| Test Case ID \|
  Test Case Description \| Test Data \| Expected Result \| Actual Result
  \| Severity \| Priority \| Comments \|

Rules: - Generate unique Test Scenario IDs and Test Case IDs. - Avoid
duplicate or overlapping test cases. - Leave Actual Result blank. -
Severity: Critical, High, Medium, Low. - Priority: P0, P1, P2, P3. -
Comments should indicate Automation Candidate, Boundary Test, API
Validation, Security Test, Edge Case, Manual Verification, etc.

## Quality Guidelines

-   Follow ISTQB best practices.
-   Ensure complete requirement coverage.
-   Use concise, action-oriented language.
-   Include only meaningful scenarios.
-   Prioritize high-risk functionality.
-   Make every test case automation-ready.

## Coverage Summary

Provide: - Total Test Scenarios - Total Test Cases - Positive Test
Cases - Negative Test Cases - Functional Test Cases - Non-Functional
Test Cases - Boundary Value Test Cases - Edge Case Test Cases - Security
Test Cases - API Test Cases - UI/UX Test Cases - Accessibility Test
Cases - Automation-ready Test Cases - Requirement Coverage (%)

