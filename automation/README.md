# Playwright UI Automation – RealWorld App

This folder is intended for UI automated tests for the RealWorld (Conduit) application using **Playwright**.

At the current stage, this is a **work in progress** area.  
The goal is to gradually build a small but meaningful set of automated tests focused on critical user flows.

---

## Purpose

The purpose of this automation is to:
- Practice UI test automation using Playwright
- Verify the most important user scenarios
- Support basic regression testing as test coverage grows
- Apply good automation practices in a realistic sample project

This project prioritizes learning, clarity, and maintainability over large test volume.

---

## Planned Automation Scope

The following areas are planned to be automated:

- User authentication via UI (login, logout)
- Article management (create, edit, delete)
- Basic navigation between main pages
- Smoke and simple regression scenarios

Scenarios that are highly dynamic or exploratory will remain manual.

---

## Planned Testing Approach

- Tests will be written from an end-user perspective
- Authentication will initially be handled through the **UI**, reflecting real user behavior
- API-based authentication may be added later to improve test speed and stability
- Emphasis will be placed on readable tests, clear assertions, and stable selectors
- Automation will focus on critical paths rather than full coverage

API endpoints, including login, are tested separately using Postman as part of API testing.

---

## Technology Stack (Planned)

- Playwright
- JavaScript / TypeScript
- Node.js
- npm

---

## Planned Project Structure

```text
playwright/
│
├── tests/
│   ├── auth/
│   │   └── login.spec.ts
│   ├── articles/
│   │   ├── create-article.spec.ts
│   │   └── edit-article.spec.ts
│   └── navigation.spec.ts
│
├── pages/                  # Page Object Model (optional)
│   ├── login.page.ts
│   └── article.page.ts
│
├── playwright.config.ts
└── README.md