# Test Strategy – RealWorld App (Conduit)

## 1. Introduction

This document explains how testing is carried out for the RealWorld (Conduit) application. It describes the general testing approach, the types of testing performed, and the tools used during the process. The goal is to ensure that the application behaves as expected, key user flows are reliable, and major quality risks are identified early.

## 2. Testing Objectives

The main goals of testing are to:

* Confirm that core features work correctly from a user perspective
* Detect defects that could negatively impact usability or data consistency
* Verify correct interaction between the UI and the API
* Minimize the risk of regressions after changes
* Provide clear and understandable information about the application’s quality

## 3. Test Levels

Testing is performed at the following levels:

* **Integration testing**
  Focused on validating communication between the frontend and backend services

* **System testing**
  End-to-end testing of complete user scenarios in a realistic environment

* **Regression testing**
  Re-testing of critical functionality after updates or fixes

(Unit testing is handled by developers and is not covered by this strategy.)

## 4. Test Types

The following types of testing are included:

* **Functional testing**
  Verification of UI and API behavior against expected results

* **Exploratory testing**
  Manual testing based on experience and intuition to uncover edge cases and unexpected issues

* **Regression testing**
  Ensuring that existing features remain stable after changes

* **Usability checks**
  Basic evaluation of forms, navigation, error messages, and overall user experience

* **API testing**
  Validation of endpoints, authentication, request/response structures, and error handling

## 5. Test Approach

### 5.1 UI Testing

* Manual testing of key user flows using documented test cases
* Automated UI tests implemented with Cypress and Playwright
* Primary focus on authentication, article management, comments, and navigation

### 5.2 API Testing

* API tests created and executed using Postman and Newman
* Coverage includes authentication, article operations, comments, and user profiles
* Both positive and negative scenarios are verified

### 5.3 Exploratory Testing

* Time-boxed exploratory sessions targeting high-risk or unstable areas
* Findings are documented as bug reports with clear reproduction steps and evidence

## 6. Test Automation Strategy

* Automation focuses on stable and repetitive scenarios
* Smoke and regression tests are prioritized for automation
* Highly unstable or exploratory scenarios are kept manual
* Automated tests are regularly reviewed and maintained to reduce flakiness

## 7. Test Data Strategy

* Use dedicated test accounts whenever possible
* Generate unique test data to avoid conflicts in the public demo environment
* Do not rely on shared or long-lived data
* Prefer API-created data for reliable automation

## 8. Defect Management

* Defects are reported with clear steps to reproduce and expected vs actual results
* Issues are categorized by severity: Critical, High, Medium, or Low
* Screenshots or recordings are attached when helpful

## 9. Entry and Exit Criteria

### Entry Criteria

* Test environment is available and accessible
* Test cases and test data are prepared
* Automation frameworks are ready for execution

### Exit Criteria

* All planned test cases have been executed
* No unresolved critical defects remain
* Test results and conclusions are documented

## 10. Risks and Mitigation

The main risks include authentication issues, problems with core functionality, and instability of the public demo environment. These risks are reduced by focusing testing efforts on critical areas, using automation where appropriate, and clearly documenting environment-related issues.

## 11. Deliverables

* Test Plan
* Test Strategy
* Manual Test Cases
* Automated Test Scripts
* Bug Reports
* Test Summary (if applicable)

## 12. Responsibilities

* QA Engineer: test design, execution, defect reporting, and test automation
* Developers: fixing reported defects and maintaining unit tests
* Stakeholders: review of testing progress and quality status
