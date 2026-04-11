# QA Portfolio

This repository is a portfolio showcasing my QA test cases and projects developed on the QAse platform.

I continuously update and expand this portfolio with new test cases and projects as I grow my skills.

---

# Test Suites

## Pet Shop

### TC-001: Verify the "Popular" sidebar on the "Jessie's Blog" page

**Steps:**
1. Scroll down to the "Popular" sidebar header  
   **Expected Result:** Sidebar is visible and correctly placed on the right side  

2. Scroll page  
   **Expected Result:** Sidebar remains visible and properly aligned  

**Actual Result:**  
Sidebar displayed incorrectly, rotated to the left side during scrolling.

**Status:** Failed  
**Bug Report:** Logged in Jira

---

### TC-002: Verify dropdown menu fields on the Shop page

**Steps:**
1. Check "Sorting" dropdown  
   **Expected Result:** No overlap, correct alignment  

2. Check "Manufacturer" dropdown  
   **Expected Result:** No overlap, correct alignment  

3. Check "Number" dropdown  
   **Expected Result:** No overlap, correct alignment  

**Actual Result:**  
All dropdown labels are misaligned and overlapping UI elements.

**Status:** Failed  
**Bug Report:** Logged in Jira

---

### TC-003: Tips page opens after clicking button

**Steps:**
1. Hover over "About Us"  
   **Expected Result:** Dropdown appears  

2. Click "Tips"  
   **Expected Result:** Tips page opens  

**Actual Result:**  
Actual result matches expected result.

**Status:** Passed

---

## Swagger / Starships

### TC-004: Create starship (POST / 201)

**Request URL:**  
https://qasandbox-production.up.railway.app/api/starships

**Request Body:**
{
  "id": "220",
  "name": "qwac",
  "capacity": 10000,
  "volume": 1000000,
  "range": 100,
  "status": "available"
}

**Expected Result:**
- Status code 201  
- Response contains all fields  
- Content-Type application/json  

**Actual Result:**  
Matches expected result

**Status:** Passed

---

### TC-005: Create new starship with existing ID (POST / 400 Unauthorized / Bad Request)

**Tool:** Postman  

**Request URL:**
https://qasandbox-production.up.railway.app/api/starships

**Request Body:**
{
  "id": "220",
  "name": "qwac",
  "capacity": 10000,
  "volume": 1000000,
  "range": 100,
  "status": "available"
}

---

**Precondition:**
A starship with ID "220" already exists in the system.

---

## Battle.net Login

### TC-006: Login flow

**Steps:**
1. Open https://eu.shop.battle.net/  
2. Open Account menu  
3. Click "Log in"  
4. Enter email and password  
5. Click "Log in"  

**Expected Result:**  
User successfully logs in and is redirected to homepage
