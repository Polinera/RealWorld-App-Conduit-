# Manual Test Cases – RealWorld App (Conduit)

## Overview
This document contains a selected set of manual test cases covering the most important user flows in the RealWorld (Conduit) application. The goal is to validate core functionality from an end-user perspective without excessive detail.

---

## Authentication

### TC-01 – User Login with Valid Credentials
**Preconditions:**  
- User account exists

**Steps:**  
1. Open the application homepage  
2. Click **Sign in**  
3. Enter valid email and password  
4. Click **Sign in**

**Expected Result:**  
- User is successfully logged in  
- **Your Feed** page is displayed

---

### TC-02 – Login with Invalid Password
**Preconditions:**  
- User account exists

**Steps:**  
1. Open **Sign in** page  
2. Enter valid email and invalid password  
3. Click **Sign in**

**Expected Result:**  
- Login fails  
- User receives an error message

---

## Article Management

### TC-03 – Create New Article
**Preconditions:**  
- User is logged in

**Steps:**  
1. Click **New Article**  
2. Enter article title, description, and body  
3. Click **Publish Article**

**Expected Result:**  
- Article is created successfully  
- User is redirected to the article page

---

### TC-04 – Edit Existing Article
**Preconditions:**  
- User is logged in  
- User has an existing article

**Steps:**  
1. Open own article  
2. Click **Edit Article**  
3. Modify article content  
4. Save changes

**Expected Result:**  
- Article is updated  
- Updated content is visible

---

### TC-05 – Delete Article
**Preconditions:**  
- User is logged in  
- User has an existing article

**Steps:**  
1. Open own article  
2. Click **Delete Article**

**Expected Result:**  
- Article is removed  
- User is redirected to **Your Feed**

---

## Comments

### TC-06 – Add Comment to Article
**Preconditions:**  
- User is logged in  
- Article exists

**Steps:**  
1. Open an article  
2. Enter comment text  
3. Click **Post Comment**

**Expected Result:**  
- Comment appears under the article

---

## User Profile

### TC-07 – View User Profile
**Preconditions:**  
- User is logged in

**Steps:**  
1. Click on a username  
2. Open profile page

**Expected Result:**  
- User profile page is displayed  
- Articles and bio are visible

---

## Navigation & Usability

### TC-08 – Navigate Between Main Pages
**Preconditions:**  
- Application is open

**Steps:**  
1. Navigate between **Home**, **Global Feed**, and **Your Feed**

**Expected Result:**  
- Pages load correctly  
- No broken links or errors appear

---

## Notes
- Test cases focus on critical paths and common user actions  
- Edge cases and negative scenarios are further explored through exploratory testing  
- Detailed results and evidence are documented in bug reports
