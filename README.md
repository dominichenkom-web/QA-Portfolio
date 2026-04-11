# QA Portfolio

This repository is a portfolio showcasing my QA test cases and projects developed on the QAse platform.

I continuously update and expand this portfolio with new test cases and projects as I grow my skills.

---

# Test Suites

## Pet Shop

### TC-001: Verify the "Popular" sidebar on the "Jessie's Blog" page

**Steps:**
1. Scroll down to the header of the "Popular" sidebar  
   **Expected Result:** Sidebar is visible and correctly displayed on the right side

2. Scroll until the sidebar disappears from view  
   **Expected Result:** Sidebar remains visible and properly aligned during scrolling

**Actual Result:**  
Sidebar displayed incorrectly, rotated to the left side.  
When page is scrolled, sidebar starts to rotate to the other side.

**Status:** Failed  
**Bug:** Logged in bug tracker

---

### TC-002: Verify dropdown menu fields on the Shop page

**Steps:**
1. Observe the "Sorting" dropdown menu  
   **Expected Result:** Fully visible, no overlap

2. Observe the "Manufacturer" dropdown menu  
   **Expected Result:** Fully visible, no overlap

3. Observe the "Number" dropdown menu  
   **Expected Result:** Fully visible, no overlap

**Actual Result:**  
Labels are misaligned and text overlaps with other UI elements.

**Status:** Failed  
**Bug:** Logged in bug tracker

---

## Swagger / Starships

### TC-003: Create new starship with valid data (POST / 201)

**Tool:** Postman

**Request Body:**
```json
{
  "id": "220",
  "name": "qwac",
  "capacity": 10000,
  "volume": 1000000,
  "range": 100,
  "status": "available"
} 
