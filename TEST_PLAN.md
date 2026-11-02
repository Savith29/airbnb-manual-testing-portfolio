# Software Test Plan — Airbnb Web Platform

## 1. Purpose

This test plan defines the strategy, scope, objectives, test approach, environment, and quality criteria for the manual testing of selected user-facing workflows of the Airbnb web platform.

The purpose is to identify functional, usability, validation, and compatibility issues through structured and evidence-driven manual testing.

---

## 2. Test Objectives

The main objectives of this testing activity are to:

- Verify critical user-facing workflows.
- Validate search and discovery functionality.
- Verify date and guest selection behaviour.
- Evaluate filter functionality.
- Identify invalid and unexpected input behaviour.
- Validate important UI interactions.
- Evaluate responsive behaviour across selected viewport sizes.
- Document reproducible defects with supporting evidence.
- Verify fixes through retesting where applicable.
- Perform regression testing on affected functionality.

---

## 3. Scope

### 3.1 In Scope

The following areas are included in this testing project:

#### Search & Discovery

- Destination input
- Destination suggestions
- Search execution
- Search results
- Search criteria behaviour

#### Date Selection

- Check-in date
- Check-out date
- Calendar navigation
- Date boundaries
- Invalid date combinations

#### Guest Selection

- Adults
- Children
- Infants
- Increment controls
- Decrement controls
- Boundary conditions

#### Filters

- Price-related filtering
- Property-related filtering
- Multiple filter combinations
- Applying filters
- Removing filters

#### Responsive UI

- Desktop viewport
- Mobile viewport
- Navigation
- Search controls
- Text visibility
- Interactive elements

---

## 4. Out of Scope

The following areas are excluded:

- Payment transactions
- Real financial transactions
- Private APIs
- Internal databases
- Source-code testing
- Security penetration testing
- Authentication bypass testing
- Host administration functionality
- Destructive testing
- Access to private or restricted systems

---

## 5. Testing Types

The following testing techniques will be applied where appropriate.

### 5.1 Functional Testing

Verifies that features behave according to their observable intended functionality.

### 5.2 Negative Testing

Validates application behaviour when invalid, unexpected, or incomplete inputs are provided.

### 5.3 Boundary Value Analysis

Tests values at, below, and above relevant boundaries.

### 5.4 Equivalence Partitioning

Groups similar input conditions into representative test scenarios.

### 5.5 Exploratory Testing

Uses structured exploration to discover unexpected behaviour that may not be identified through predefined test cases.

### 5.6 UI Testing

Validates the visibility, usability, consistency, and interaction of important interface elements.

### 5.7 Compatibility Testing

Evaluates behaviour across selected browsers and viewport configurations.

### 5.8 Regression Testing

Re-executes relevant test cases after changes or defect fixes to identify unintended regressions.

---

## 6. Test Environment

The exact environment used for each execution cycle will be recorded.

### Environment Information

- Operating System
- Browser
- Browser Version
- Screen Resolution
- Viewport Size
- Test Date
- Application State

Example:

```text
Operating System: Windows
Browser: Google Chrome
Browser Version: Recorded during execution
Viewport: Desktop / Mobile
Testing Type: Manual Black-Box Testing
```

---

## 7. Test Data

Test data will use non-sensitive and non-production personal information.

Examples include:

- Public destinations
- Valid calendar dates
- Guest counts
- Filter combinations
- Boundary values
- Invalid input combinations

No real payment information or sensitive personal information will be used.

---

## 8. Entry Criteria

Testing may begin when:

- The publicly accessible application is available.
- Required browser tools are available.
- Test cases have been prepared.
- The test environment has been identified.
- Required test data is available.

---

## 9. Exit Criteria

The test cycle may be considered complete when:

- Planned test cases have been executed.
- Results have been recorded.
- Failed tests have been investigated.
- Reproducible defects have been documented.
- Relevant retesting has been completed.
- Regression testing has been performed where applicable.
- Final test results have been summarized.

---

## 10. Defect Management

Potential defects will be documented using a standard defect-reporting structure.

Each defect should contain:

- Defect ID
- Summary
- Environment
- Preconditions
- Steps to Reproduce
- Expected Result
- Actual Result
- Severity
- Priority
- Reproducibility
- Evidence
- Status

Defects will only be reported as confirmed defects when they can be reproduced and supported by evidence.

---

## 11. Severity Classification

| Severity | Description |
|---|---|
| Critical | Prevents a critical user journey or causes severe system impact |
| High | Major functionality is significantly affected |
| Medium | Important functionality is affected but a workaround may exist |
| Low | Minor functional or UI issue with limited impact |

---

## 12. Priority Classification

| Priority | Description |
|---|---|
| P0 | Immediate attention required |
| P1 | High priority |
| P2 | Normal priority |
| P3 | Low priority |

Severity and priority will be assessed independently.

---

## 13. Test Execution

Each test case will be assigned an execution status.

| Status | Meaning |
|---|---|
| PASS | Actual result matches expected result |
| FAIL | Actual result differs from expected result |
| BLOCKED | Test cannot be completed because of an external blocker |
| NOT EXECUTED | Test has not yet been executed |
| RETEST | Previously failed scenario is being verified again |

---

## 14. Test Evidence

Evidence will be collected during actual test execution.

Evidence may include:

- Screenshots
- Screen recordings
- Browser information
- Responsive viewport evidence
- Defect reproduction evidence

Evidence will be stored in the repository under:

```text
evidence/
├── screenshots/
└── recordings/
```

---

## 15. Traceability

Testing activities will maintain traceability between:

```text
Test Objective
      ↓
Test Scenario
      ↓
Test Case
      ↓
Test Execution
      ↓
Defect
      ↓
Retest
      ↓
Regression
```

This provides visibility into what was tested and how identified issues were validated.

---

## 16. Risks and Limitations

Testing a publicly accessible production web platform introduces limitations.

These may include:

- UI changes during the testing period
- Dynamic content
- Location-dependent results
- Availability-dependent behaviour
- Browser differences
- Network conditions
- Features changing without notice

Therefore, test observations are recorded together with the execution environment and date.

---

## 17. Testing Ethics

Testing will be performed using normal, non-destructive user interactions.

The project will not intentionally:

- Attack the application
- Attempt unauthorized access
- Circumvent authentication
- Access private information
- Exploit security vulnerabilities
- Perform denial-of-service activities
- Modify or damage application data

---

## 18. Deliverables

The final project is expected to contain:

- Test Plan
- Test Cases
- Test Execution Results
- Defect Reports
- Test Evidence
- Traceability Matrix
- Final Test Summary

---

## 19. Approval

This document defines the planned manual testing approach for the project.

Actual results, defect counts, execution metrics, and coverage statistics will be added only after testing has been performed.
