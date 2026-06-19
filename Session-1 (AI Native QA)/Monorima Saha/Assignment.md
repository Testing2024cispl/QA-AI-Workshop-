# Automation Exercise QA Test Documentation

## Overview

This repository contains a complete QA testing documentation for the **Automation Exercise** website.

It includes:

* Manual test cases created through human-driven QA thinking
* AI-generated test cases
* Prompt engineering used to generate AI test cases
* Comparative analysis between manual and AI testing approaches
* Final optimized automation-ready test cases

---

## Reference Website

* https://automationexercise.com/

---

# Table of Contents

* [QA Manual Test Cases](#qa-manual-test-cases)

  * [Human Thinking Test Cases](#human-thinking-test-cases)

    * Test Case 001: User Registration
    * Test Case 002: User Login with Correct Credentials
    * Test Case 003: User Login with Incorrect Credentials
    * Test Case 004: Place Order After Registration
    * Test Case 005: Place Order – Register While Checkout

* [AI Manual Test Cases](#ai-manual-test-cases)

  * User Login
  * User Registration
  * Place Order After Registration
  * Place Order – Register While Checkout

* [Prompt](#prompt)

* [My Thoughts](#my-thoughts)

* [Final Test Cases (AI + Manual Combined) – Automation Ready](#final-test-cases-ai--manual-combined--automation-ready)

  * Suite 1: Registration
  * Suite 2: Session & Identity
  * Suite 3: E2E Checkout Flows

---

# QA Manual Test Cases

## Member Details

* **Member Name:** Monorima Saha

## Human Thinking Test Cases

### Test Case 001 — User Registration

Covers:

* New user signup
* Duplicate email validation
* Account creation workflow

### Test Case 002 — User Login with Correct Credentials

Covers:

* Successful login
* Authentication validation

### Test Case 003 — User Login with Incorrect Credentials

Covers:

* Failed login handling
* Error message validation

### Test Case 004 — Place Order After Registration

Covers:

* Registration
* Product selection
* Checkout
* Payment flow

### Test Case 005 — Place Order: Register While Checkout

Covers:

* Guest cart creation
* Mid-checkout registration
* Payment completion

---

# AI Manual Test Cases

This section contains AI-generated comprehensive QA test cases.

Coverage includes:

* Positive scenarios
* Negative scenarios
* Boundary testing
* UI/UX testing
* Security testing
* End-to-end testing

---

# Prompt

## Login Prompt

> Act as an expert Manual QA. Generate a comprehensive suite of test cases for the login functionality of Automation Exercise.

## Signup Prompt

> Act as a Senior Manual QA Engineer. Generate a robust suite of test cases for Signup functionality.

## E2E Workflow Prompt

> Act as a Senior QA Automation Engineer. Generate comprehensive test cases for Register and Place Order workflow.

## Checkout Workflow Prompt

> Act as a Senior Manual QA Engineer. Generate a detailed test suite for Place Order: Register while Checkout workflow.

---

# My Thoughts

## What Felt Suitable

The AI generated:

* Clean metadata outlines
* Explicit pre-conditions
* Distinct test data
* Clear expected results

Benefits:

* Organized repository structure
* Strong automation readiness
* Excellent edge-case coverage

### AI Test Cases Best For:

* Structured documentation
* Negative testing
* Automation preparation

Strength:

* Strong in coverage and structure

Weakness:

* Practical prioritization can be weaker

---

## What Felt Not Suitable

AI-generated test suites tend to create:

* Large volume of scenarios
* Document clutter
* Repetitive steps
* Duplicate flows

---

## Manual Test Cases Best For:

* Business flow validation
* Functional understanding
* Exploratory testing

Strength:

* Strong domain understanding

Weakness:

* Weak structure
* Limited edge-case coverage

---

# Final Test Cases (AI + Manual Combined) – Automation Ready

These final test cases combine:

* Human business logic understanding
* AI structured coverage
* Automation-friendly design

---

## Suite 1: Registration

### TC_REG_001 — New User Registration & Account Deletion Lifecycle

Covers:

* Signup flow
* Account creation
* Account deletion

### TC_REG_002 — Re-registration Block via Existing Email Validation

Covers:

* Duplicate email prevention

### TC_REG_003 — Step-2 Read-Only Data Attribute Verification

Covers:

* Email field validation
* UI security validation

---

## Suite 2: Session & Identity

### TC_AUTH_001 — Successful Account Login with Valid Credentials

### TC_AUTH_002 — Login Rejection Handling via Mismatched Credentials

### TC_AUTH_003 — Client-Side Input Masking & Security Property Verification

### TC_AUTH_004 — Post-Logout Session & Back-Buffer Termination

---

## Suite 3: E2E Checkout Flows

### TC_E2E_001 — Place Order - Post-Registration Workflow Path

Covers:

* Login
* Cart
* Checkout
* Payment

### TC_E2E_002 — Place Order - Mid-Checkout Gateway Registration Path

Covers:

* Guest cart
* Checkout registration
* Cart persistence
* Order placement

---

# Summary

This project demonstrates how combining:

* Manual QA expertise
* AI-assisted testing
* Automation thinking

can produce a highly effective QA strategy.

Final Outcome:

* Better test coverage
* Better maintainability
* Better automation readiness
