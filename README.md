# Airbnb Web Platform — Enterprise Manual QA Portfolio

> **End-to-End Manual Testing | Functional Quality Engineering | Defect Analysis | Test Evidence**

## Overview

This repository presents a structured, evidence-driven manual testing portfolio for selected user-facing workflows of the Airbnb web platform.

The project is designed to demonstrate how a QA Engineer approaches the validation of a modern, highly dynamic consumer web application — from test planning and test-case design through execution, defect reporting, retesting, regression testing, and final quality assessment.

The emphasis is not simply on finding whether a feature "works", but on systematically evaluating:

- Functional correctness
- Business-rule behaviour
- Boundary conditions
- Invalid and unexpected inputs
- User-interface consistency
- Responsive behaviour
- Cross-browser compatibility
- Defect impact and risk
- Reproducibility and test evidence

---

## Quality Engineering Objective

The primary objective of this project is to evaluate critical user journeys and identify conditions that could negatively affect:

- User experience
- Search accuracy
- Booking discovery
- Data integrity
- Functional reliability
- Accessibility of important controls
- Responsive usability

Testing decisions are based on risk, user impact, observable system behaviour, and reproducible evidence.

---

# System Under Test

**Application:** Airbnb Web Platform  
**Testing Approach:** Manual Black-Box Testing  
**Application Type:** Consumer Web Application  
**Primary Focus:** Search and discovery workflows

### Core Workflow

```text
User
 │
 ├── Destination
 │
 ├── Dates
 │
 ├── Guests
 │
 ├── Filters
 │
 └── Search
       │
       ▼
   Search Results
       │
       ▼
   Listing Discovery
```

---

# Testing Scope

## In Scope

### 1. Search & Discovery

- Destination input
- Destination suggestions
- Search execution
- Search result rendering
- Search criteria persistence

### 2. Date Selection

- Check-in selection
- Check-out selection
- Date boundaries
- Invalid date combinations
- Calendar navigation
- Disabled-date behaviour

### 3. Guest Selection

- Adult counter
- Child counter
- Infant counter
- Increment/decrement controls
- Boundary conditions
- Invalid guest combinations

### 4. Search Filters

- Price-related filters
- Property-related filters
- Availability-related filters
- Multiple filter combinations
- Filter application and removal

### 5. Responsive UI

- Desktop layout
- Mobile viewport behaviour
- Navigation accessibility
- Element visibility
- Text wrapping
- Interactive control accessibility

---

# Out of Scope

The following areas are intentionally excluded from this portfolio:

- Payment processing
- Real financial transactions
- Private APIs
- Internal services
- Private databases
- Source-code analysis
- Security penetration testing
- Authentication bypass testing
- Host administration systems
- Destructive testing

---

# Testing Methodology

The project combines multiple complementary testing techniques.

## Functional Testing

Validates whether features behave according to their observable intended functionality.

## Negative Testing

Attempts invalid or unexpected user inputs to evaluate how the application handles them.

## Boundary Value Analysis

Tests values around important boundaries and limits.

Example:

```text
Below boundary
At boundary
Above boundary
```

## Equivalence Partitioning

Groups similar input conditions into representative test classes to reduce redundant testing while maintaining meaningful coverage.

## Exploratory Testing

Uses structured exploration to identify unexpected behaviour that may not be covered by predefined test cases.

## Compatibility Testing

Evaluates behaviour across supported browsers and viewport configurations.

## Regression Testing

Re-executes previously validated scenarios after changes or fixes to determine whether existing functionality remains stable.

---

# Test Design Strategy

Test cases are designed around realistic user journeys and risk-based scenarios.

Each test case contains:

- Unique Test Case ID
- Feature / Module
- Test Objective
- Preconditions
- Test Steps
- Test Data
- Expected Result
- Actual Result
- Execution Status
- Severity
- Evidence

The project progressively expands from core positive scenarios into negative, boundary, edge-case, exploratory, and compatibility scenarios.

---

# Defect Management

Potential defects are documented using a reproducible defect-reporting structure.

Each defect report includes:

- Defect ID
- Title
- Environment
- Preconditions
- Steps to Reproduce
- Expected Result
- Actual Result
- Severity
- Priority
- Reproducibility
- Evidence
- Current Status

### Defect Classification

**Severity** describes the impact of the defect.

**Priority** describes how urgently the defect should be addressed.

These attributes are evaluated independently rather than treating them as interchangeable values.

---

# Test Evidence

Testing evidence is maintained alongside the test documentation.

```text
evidence/
├── screenshots/
└── recordings/
```

Evidence may include:

- Test execution screenshots
- Defect screenshots
- Responsive viewport evidence
- Before/after verification
- Reproduction recordings where appropriate

Only evidence produced during actual test execution is reported as test evidence.

---

# Test Execution

Test execution results are recorded using the following states:

| Status | Meaning |
|---|---|
| PASS | Actual behaviour matches the expected result |
| FAIL | Actual behaviour differs from the expected result |
| BLOCKED | Test cannot be completed because of an external blocker |
| NOT EXECUTED | Test has not yet been executed |
| RETEST | Defect fix is being verified |

Execution metrics are reported only after the corresponding test cases have actually been executed.

---

# Traceability

The project maintains traceability between testing objectives, test cases, execution results, and identified defects.

```text
Testing Objective
       │
       ▼
Test Scenario
       │
       ▼
Test Case
       │
       ▼
Test Execution
       │
       ├── PASS
       │
       └── FAIL
              │
              ▼
         Defect Report
              │
              ▼
            Retest
              │
              ▼
          Regression
```

This structure allows testing decisions and defect findings to be traced back to the original validation objective.

---

# Repository Structure

```text
airbnb-manual-testing-portfolio/
│
├── README.md
├── TEST_PLAN.md
├── TEST_CASES.xlsx
├── BUG_REPORTS.md
├── TEST_EXECUTION_REPORT.md
├── TRACEABILITY_MATRIX.md
│
└── evidence/
    ├── screenshots/
    └── recordings/
```

---

# Test Environment

The environment used during execution is documented with each test cycle.

Typical environment information includes:

```text
Operating System
Browser
Browser Version
Viewport / Device
Test Date
Build / Website State
```

Exact environment details are recorded from the actual execution environment rather than assumed in advance.

---

# Quality Metrics

After execution, the project may report metrics such as:

```text
Total Test Cases
Executed
Passed
Failed
Blocked
Pass Rate
Defects Identified
Critical Defects
High Severity Defects
Retested Defects
Regression Results
```

No metric is reported until it has been supported by actual test execution data.

---

# Professional QA Principles Applied

This portfolio follows several core quality-engineering principles:

- Test the product from the user's perspective
- Prioritize high-risk workflows
- Separate expected behaviour from observed behaviour
- Never assume a defect without reproducible evidence
- Record actual results rather than predicted results
- Distinguish severity from priority
- Maintain traceability
- Preserve objective test evidence
- Retest fixes
- Perform regression testing after relevant changes
- Avoid overstating test coverage or defect findings

---

# Educational Disclaimer

This project is an independent educational QA portfolio.

Testing is restricted to normal, non-destructive interaction with publicly accessible functionality of the Airbnb web platform.

No private systems, internal infrastructure, private APIs, databases, authentication mechanisms, or security-sensitive components are intentionally accessed or tested.

Airbnb and related trademarks belong to their respective owners. This repository is not affiliated with, endorsed by, or sponsored by Airbnb.

---

# Author

**Manual QA / Software Testing Portfolio**

This repository demonstrates practical application of software quality-assurance principles through structured test design, execution, evidence collection, defect analysis, and reporting.
