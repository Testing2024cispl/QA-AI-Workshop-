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

