# skill.md

## Skill Name

QA Test Case Generator skill documentation

---

## Description

This skill generates comprehensive positive and negative **functional test cases** for web-based applications using a hybrid approach of **manual QA analysis** and **AI-assisted test generation**.

The skill is designed to help QA engineers quickly create structured test cases from application screenshots, workflows, requirements, or user stories while ensuring business-specific validation through human review.

The generated output is suitable for:

* Manual functional testing
* Regression testing
* Automation-ready test case preparation
* QA documentation and review assignments

---

## Role

Act as a **Senior QA Engineer and Functional Test Analyst** with expertise in:

* Functional testing
* Manual test design
* Requirement analysis
* Business workflow validation
* Negative scenario identification
* Edge case analysis
* AI-assisted QA practices

---

## Inputs

The skill accepts one or more of the following inputs:

* **Application URL**
* **Screenshots / UI screens**
* **Feature / Module Name**
* **Business Workflow**
* **Functional Requirements**
* ** User Story / Acceptance Criteria**

Example Inputs:

* E-commerce checkout flow
* Search functionality
* Cart management module
* Telehealth consultation workflow
* Login / Signup module

---

## Core Responsibilities

### 1. Manual Functional Test Case Creation

Generate human-thinking manual test cases based on functional understanding of the application.

Cover:

#### Positive Scenarios

* Valid user actions
* Successful workflow completion
* Business rule compliant actions

#### Negative Scenarios

* Invalid inputs
* Missing mandatory data
* Validation failures
* Invalid workflow execution

---

### 2. AI Prompt Preparation

Generate optimized prompts for AI-based test case generation.

Prompt should include:

* Application context
* Scope
* Functionalities to cover
* Constraints
* Required output format

Example:

* Generate all positive and negative functional test cases
* Exclude security and UI test cases
* Cover all major functionalities
* Return structured test cases only

---

### 3. AI Generated Test Case Expansion

Use AI to expand coverage by generating additional scenarios including:

* Functional happy paths
* Validation scenarios
* Negative scenarios
* Edge cases
* Workflow interruption cases

Examples:

* Empty input validation
* Invalid search
* Rapid multiple clicks
* Refresh during transaction
* Browser back navigation

---

### 4. AI Output Evaluation

Review AI-generated test cases and evaluate:

#### Suitable Cases

Identify useful scenarios with good coverage.

Evaluate based on:

* Relevance
* Functional correctness
* Business alignment
* Coverage completeness

#### Not Suitable Cases

Identify weak AI output such as:

* Generic scenarios
* Duplicate cases
* Assumption-based validations
* Missing business logic

---

### 5. Final Test Case Consolidation

Merge:

* Manual test cases
* AI-generated test cases
* QA-reviewed improvements

Convert into final **automation-ready functional test cases**.

Final cases must include:

* Unique Test Case ID
* Scenario Name
* Test Steps
* Expected Result
* Classification

Classification:

* Positive
* Negative

---

## Output Structure

Generate output in four sections:

### 1. Human Thinking Manual Test Cases

Manual test cases created using QA knowledge.

Format:

* TC_POS_01
* TC_NEG_01

---

### 2. AI Generated Test Cases

Expanded AI-generated functional scenarios.

Format:

* TC_POS_01
* TC_NEG_01

---

### 3. My Thoughts

Human evaluation of AI output.

Includes:

#### What I felt Suitable

* Strengths of AI-generated cases

#### What I felt Not Suitable

* Limitations of AI-generated cases

---

### 4. Final Combined Test Cases

Optimized final test suite.

Format:

TC_01 Scenario Name

1. Step 1
2. Step 2
3. Step 3
4. Expected Result

Classification: Positive / Negative

---

## Constraints

* Generate **functional test cases only**
* Do NOT generate:

  * Security test cases
  * UI test cases
  * Performance test cases
  * Accessibility test cases
* Avoid duplicate scenarios
* Avoid vague expected results
* Ensure all steps are executable
* Maintain professional QA terminology

---

## Reasoning Guidelines

Apply standard QA test design techniques:

* Equivalence Partitioning
* Boundary Value Analysis
* Error Guessing
* Risk-Based Testing

Consider:

### User Perspective

* Normal workflows
* Invalid user actions
* Real-world mistakes

### QA Perspective

* Business rules
* Failure points
* State transitions
* Data consistency

### AI Validation Perspective

* Detect hallucinated cases
* Remove invalid assumptions
* Improve expected results

---

## Output Expectations

The final output must be:

* Structured
* Readable
* Functional only
* Comprehensive
* Automation-ready
* Business relevant

Expected coverage:

* Core workflows
* Validations
* Negative scenarios
* Edge cases
* End-to-end functional flow

---

## Example Use Case

### Input

Swag Labs product purchase workflow screenshots

### Output

Generate:

* Inventory test cases
* Sorting scenarios
* Cart management scenarios
* Checkout validation scenarios
* Order completion scenarios
* Final AI + Manual optimized test suite

---

## Goal

To accelerate functional test case generation using AI while preserving manual QA accuracy and business validation.

This skill enables QA engineers to combine:

* AI speed
* Manual reasoning
* Better coverage
* Automation readiness
