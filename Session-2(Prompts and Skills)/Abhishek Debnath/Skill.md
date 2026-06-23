# EventHub Testing Skill

## 1. App Context

| Item | Details |
|------|---------|
| **App Name** | EventHub |
| **URL** | https://eventhub.rahulshettyacademy.com |
| **Auth** | Email + Password (register/login) |
| **Pages** | Login, Register, Dashboard, Events, Event Detail, My Bookings, Booking Detail |
| **Test Data** | Dynamic — agent generates unique emails with timestamps |

---

## 2. Page Inventory

| Page | URL | Key Elements |
|------|-----|--------------|
| Login | /login | Email, Password, Sign In, Register link |
| Register | /register | Email, Password, Confirm Password, Create Account, 4 password rules |
| Dashboard | / | Featured Events, nav links (Home, Events, My Bookings, API Docs, Admin, Logout) |
| Events | /events | Search bar, Category dropdown, City dropdown, event cards with Book Now |
| Event Detail | /events/{id} | Event info, ticket counter (+/-), Full Name, Email, Phone, Confirm Booking |
| My Bookings | /bookings | Booking cards with status, View Details, Cancel Booking, Clear all |
| Booking Detail | /bookings/{id} | Booking info, Cancel Booking, Check refund eligibility, Back button |

---

## 3. Test Case Format (Manual — for QA Team)

| TC ID | Module | Scenario | Steps | Expected Result | Priority |
|-------|--------|----------|-------|-----------------|----------|
| TC_001 | Registration | Happy path | 1. Navigate to /register<br>2. Enter email<br>3. Enter password<br>4. Click Create Account | User redirected to Dashboard | High |

**Columns:**
- **TC ID:** Unique identifier (TC_001, TC_002, etc.)
- **Module:** Feature area (Registration, Login, Events, Booking, etc.)
- **Scenario:** Brief description of the test case
- **Steps:** Numbered steps to execute
- **Expected Result:** What should happen
- **Priority:** High, Medium, Low

---

## 4. Test Case Format (Automation-Ready)

| TC ID | Module | Scenario | Precondition | Steps | Expected Result | Selectors | Priority |
|-------|--------|----------|--------------|-------|-----------------|-----------|----------|
| TC_001 | Registration | Happy path | User not logged in | 1. Navigate to /register<br>2. Enter dynamic email<br>3. Enter password "Test@1234"<br>4. Click Create Account | Redirect to Dashboard, email in navbar | `#email`, `button:has-text("Create Account")` | High |

**Additional Columns (vs Manual):**
- **Precondition:** What must be true before execution
- **Selectors:** Element selectors for automation

---

## 5. Selector Reference

| Page | Element | Selector |
|------|---------|----------|
| Login | Email | `input[type="email"]` |
| Login | Password | `input[type="password"]` |
| Login | Sign In | `button:has-text("Sign In")` |
| Register | Email | `#email` |
| Register | Password | `#password` |
| Register | Confirm Password | `#confirmPassword` |
| Register | Create Account | `button:has-text("Create Account")` |
| Register | Password rules | `.password-rule` (4 items) |
| Dashboard | User email | `.user-email` or navbar text |
| Dashboard | Logout | `button:has-text("Logout")` |
| Events | Search | `input[placeholder*="Search"]` |
| Events | Category | `select` or custom dropdown |
| Events | City | `select` or custom dropdown |
| Events | Book Now | `button:has-text("Book Now")` |
| Event Detail | Ticket + | `button:has-text("+")` |
| Event Detail | Ticket - | `button:has-text("−")` |
| Event Detail | Full Name | `#fullName` |
| Event Detail | Email | `#email` |
| Event Detail | Phone | `#phone` |
| Event Detail | Confirm Booking | `button:has-text("Confirm Booking")` |
| Bookings | Cancel Booking | `button:has-text("Cancel Booking")` |
| Bookings | View Details | `button:has-text("View Details")` |
| Bookings | Clear all | `button:has-text("Clear all bookings")` |
| Cancel Modal | Confirm | `button:has-text("Yes, cancel it")` |
| Cancel Modal | Dismiss | `button:has-text("Cancel")` |

---

## 6. Test Case Inventory

| TC Group | Feature | Coverage |
|----------|---------|----------|
| TC_001 | Registration | Happy path, validation, duplicate email |
| TC_002 | Login | Happy path, invalid credentials, empty fields |
| TC_003 | Browse Events | Search, filter, category, city |
| TC_004 | Event Detail | Page verification, breadcrumbs, featured badge |
| TC_005 | Event Booking | Happy path, multiple tickets, max/min limits, validation |
| TC_006 | My Bookings | View list, view details, booking card verification |
| TC_007 | Cancel Booking | Happy path, decline confirmation, clear all |
| TC_008 | Logout | Happy path, session invalidation, protected routes |
| TC_009 | Navigation | All links, breadcrumbs, back navigation |
| TC_010 | E2E Flow | Register → Book → Cancel → Logout |

---

## 7. Example Test Cases

### Example 1: Manual Test Case (for QA Team)

| TC ID | Module | Scenario | Steps | Expected Result | Priority |
|-------|--------|----------|-------|-----------------|----------|
| TC_001 | Registration | Happy path | 1. Navigate to /register<br>2. Enter email "test_{timestamp}@yopmail.com"<br>3. Enter password "Test@1234"<br>4. Confirm password "Test@1234"<br>5. Click Create Account | User redirected to Dashboard, email displayed in navbar | High |

### Example 2: Automation-Ready Test Case

| TC ID | Module | Scenario | Precondition | Steps | Expected Result | Selectors | Priority |
|-------|--------|----------|--------------|-------|-----------------|-----------|----------|
| TC_001 | Registration | Happy path | User not logged in | 1. Navigate to /register<br>2. Enter dynamic email<br>3. Enter password "Test@1234"<br>4. Confirm password "Test@1234"<br>5. Click Create Account | Redirect to Dashboard, email in navbar | `#email`, `#password`, `#confirmPassword`, `button:has-text("Create Account")` | High |

---

## 8. Prompting Guide

**To write a new test case, specify:**
1. Feature (Registration, Login, Events, Booking, etc.)
2. Scenario type (happy path, negative, boundary, E2E)
3. Expected behavior
4. Any specific data or conditions

**Example prompts:**
- "Write a test case for event booking with 5 tickets"
- "Write a negative test case for login with locked account"
- "Write an E2E test case for register → book → cancel → logout"

---

## 9. Key Decisions

| Decision | Choice |
|----------|--------|
| **Test data** | Dynamic — agent generates unique emails with timestamps |
| **Selectors** | Verified correct, included as-is |
| **Scope** | UI test cases only |
| **Format** | Tabular (not Gherkin) |

