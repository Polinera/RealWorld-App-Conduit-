Test Plan – RealWorld App
1. Purpose of the Document

This test plan defines the strategy, scope, and approach for testing the RealWorld Conduit application. Its purpose is to ensure that all core functionalities of the application are verified, defects are identified, and the application meets quality standards. This document will guide both manual and automated testing efforts, and serve as a reference for reporting and tracking issues.

2. Test Scope

In Scope:

UI Functional Tests:

User registration and login

Creating, editing, deleting articles

Commenting on articles

Viewing and editing user profiles

Navigation across the main pages (Home, Global Feed, Your Feed)

Error messages and form validations

API Tests:

Authentication endpoints (login, register)

CRUD operations on articles (create, read, update, delete)

Comment operations

User profile endpoints

Non-Functional Tests:

Usability of forms and navigation

Basic performance checks (page load times under normal conditions)

Responsive layout verification on desktop resolutions

Out of Scope:

Full load/performance testing under high traffic

Advanced security testing (e.g., penetration testing, XSS, SQL injection)

Cross-browser testing beyond Chrome and Firefox

Mobile device testing (focus on desktop web only)

3. Test Environment

Browsers: Chrome (v120), Firefox (v120)

Operating Systems: Windows 11, macOS Ventura

API Endpoint: https://demo.realworld.io/api

Test Data:

Pre-created user accounts: testuser1@example.com / Password123

Sample articles and comments for functional verification

Tools: Cypress, Playwright, Postman / Newman, GitHub for documentation and issue tracking

4. Tools

Cypress: UI automated tests (login, article creation, navigation)

Playwright: Cross-browser UI automation

Postman / Newman: API endpoint testing

GitHub: Version control, issue tracking, repository hosting

VSCode for code editing, Chrome DevTools for debugging

5. Entry / Exit Criteria

Entry Criteria:

Test environment is deployed and accessible

Test accounts and sample data created

Test cases documented and reviewed

Automation scripts scaffolded and ready for execution

Exit Criteria:

100% of planned manual test cases executed

All critical and high-severity defects resolved or documented

Automation scripts executed successfully with passing results

Test summary report completed and committed to GitHub repository

6. Risk Assessment

Medium Risk: Registration/login forms could have validation issues

Low Risk: Minor UI inconsistencies in article feed display

High Risk: API endpoints may fail under unexpected inputs or missing authentication tokens
