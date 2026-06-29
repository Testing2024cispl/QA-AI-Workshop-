Skill File

Skill Type:QA Manual Testing + AI-Assisted Test Design

Domain: E-Commerce Testing

Application:Grocery Store Demo

Website: https://grocerystoredemo.pcubeweb.com
Author: Sagarika Sahu

---
Name

End-to-End Manual Test Case Design for Grocery Store Demo Website**

---
Purpose

The purpose of this skill is to design complete, reusable, and automation-ready manual test cases for the Grocery Store Demo application.

This skill focuses on:

1.Login functionality

2. OTP verification
   
3.. WhatsApp OTP flow

4. Search functionality
 
5. Search Suggestions
 
6. Add to Cart
     
7. Cart Validation
  
8. Positive Testing
 
9.Negative Testing

10. AI-assisted Test Case Generation
    
11. Human validation and enhancement

---

Instructions

TestCases_001 – Login Flow

Create test cases that verify:

1. Homepage loading

2. Account icon functionality
 
3. Login popup

4. Country code (+91)

5. Mobile number validation

6. Send OTP button
 
7. OTP popup
 
8. OTP fields
 
9. OTP timer
 
10. Successful login
 
11. Session persistence
 
12. User account accessibility

---

TestCases_002 – WhatsApp OTP Flow

Verify:

1. OTP timer

2. WhatsApp OTP option

3. WhatsApp button availability
 
4. OTP verification
  
5. Successful login

---

TestCases_003 – Invalid Login

Verify:

1. Blank mobile number
  
2. Invalid mobile number

3. Less than 10 digits
 
4. Alphabet characters

5. Special characters
 
6. Invalid OTP

7. Expired OTP

8. Incomplete OTP

9. Multiple invalid OTP attempts

---

TestCases_004 – Search Suggestion & Add to Cart

Verify:

1. Search suggestion popup
* 
2. Bestseller categories
* 
3. Category image
 
4. Category name
 
5. Product listing

6. Product details
 
7. Add to Cart
 
8. Cart badge
 
9. Quantity update
 
10. Remove product

11. Cart total

---

TestCases_005 – Product Search

Verify:

1 Product search

2 Matching products

3 Product selection

4 Cart validation

5 Quantity update

6 Remove product

7 Total amount calculation


TestCases_006 – Invalid Search

Verify:

1.Invalid product search
 
2. No matching products
 
3. Appropriate message
 
4. Clear search
 
5. Product list restoration

---

AI Validation

1.Generate test cases using AI.

2.Review AI-generated scenarios.

3.Add missing validations manually.

4.Prepare a final automation-ready test case.

---

Input:

The skill requires:

1. Website URL
 
2. Functional requirement
 
3. Feature/module name

4. User workflow
 
5. Business rules
 
6. Validation rules

Example Input

Website:
https://grocerystoredemo.pcubeweb.com

Feature:
Login using Mobile Number & OTP

Feature:
Search Product

Feature:
Add Product to Cart

---

Output:

The skill produces:

1. Human-written manual test cases
 
2. Positive test scenarios
 
3. Negative test scenarios

4. Functional validation scenarios
 
5. UI validation scenarios
 
6. AI-generated test cases

7. Human-reviewed AI test cases

8. Final automation-ready test cases

Example Outputs

1. End-to-End Login Flow
 
2. WhatsApp OTP Flow
 
3. Invalid Login Flow
 
4. Search Suggestion Flow
 
5. Search Product Flow
 
6. Add to Cart Flow
 
7. Invalid Search Flow

---

Constraints

The skill follows these constraints:

1. Test cases must be step-by-step.
 
2. Every step should include a clear validation.

3. Cover both positive and negative scenarios.
 
4. Include UI and functional validations.
 
5. Test cases should be reusable.
 
6. Test cases should be automation-ready.
 
7. AI-generated cases must be reviewed before use.
 
8. Final output should combine AI suggestions with human validation.
 
9. Avoid duplicate scenarios.

10. Follow standard QA documentation practices.

---

Example

Feature

End-to-End Login Flow

Steps

1. Open Grocery Store Demo website.
  
2. Verify Homepage loads successfully.
   
3. Click Account icon.
 
4. Verify Login popup appears.
 
5. Verify +91 country code is displayed.
 
6. Enter a valid mobile number.
 
7. Click Send OTP.
   
8. Verify OTP popup appears.
 
9. Verify six OTP input fields are displayed.
 
10. Verify OTP timer is visible.
 
11. Verify WhatsApp OTP option is displayed.
 
12. Enter valid OTP.
 
13. Verify login is successful.
 
14. Verify popup closes automatically.
 
15. Verify Account section is accessible.
 
16. Refresh the page.
 
17. Verify logged-in session persists.

18. Capture screenshots and execution logs.
 
19. Mark the test case as Passed if all validations succeed.

---

Expected Result

1. User logs in successfully.
 
2. OTP is verified.
 
3. Session remains active after refresh.

4. Account page is accessible.
 
5. No validation or functional errors occur.

---

Skills Demonstrated

1. Manual Testing

2. Functional Testing
 
3. UI Testing

4. Positive Testing
 
5. Negative Testing

6. Validation Testing
 
7. End-to-End Testing
 
8. Requirement Analysis

9. AI Prompt Engineering

10. AI Test Case Review
  
11. Automation-Ready Test Design
  
12. QA Documentation

