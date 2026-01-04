# Admin Module – Test Cases (OrangeHRM)

## Module Description
The Admin module allows authorized users to manage system users, roles, and access permissions.

---

### TC_ID: A01
**Title:** Verify Admin user can access Admin module  
**Precondition:** User is logged in as Admin  
**Steps:**
1. Login with valid admin credentials
2. Click on Admin module from the menu  
**Expected Result:**  
Admin module dashboard should be displayed successfully

---

### TC_ID: A02
**Title:** Verify Add User with valid details  
**Steps:**
1. Navigate to Admin → User Management
2. Click Add
3. Enter valid user details
4. Click Save  
**Expected Result:**  
User should be added successfully

---

### TC_ID: A03
**Title:** Verify Add User with existing username  
**Steps:**
1. Navigate to Admin → User Management
2. Click Add
3. Enter an already existing username
4. Click Save  
**Expected Result:**  
System should display an error message indicating username already exists

---

### TC_ID: A04
**Title:** Verify mandatory fields validation while adding user  
**Steps:**
1. Click Add User
2. Leave mandatory fields empty
3. Click Save  
**Expected Result:**  
Validation message should be displayed for required fields

---

### TC_ID: A05
**Title:** Verify search user by username  
**Steps:**
1. Navigate to Admin → User Management
2. Enter valid username in search field
3. Click Search  
**Expected Result:**  
Matching user record should be displayed

---

### TC_ID: A06
**Title:** Verify search with invalid username  
**Steps:**
1. Enter invalid username
2. Click Search  
**Expected Result:**  
No records found message should be displayed

---

### TC_ID: A07
**Title:** Verify edit user details  
**Steps:**
1. Search for an existing user
2. Click Edit
3. Modify user details
4. Click Save  
**Expected Result:**  
User details should be updated successfully

---

### TC_ID: A08
**Title:** Verify disable user account  
**Steps:**
1. Search for an active user
2. Edit user status to Disabled
3. Save changes  
**Expected Result:**  
User should be disabled and unable to login

---

### TC_ID: A09
**Title:** Verify delete user  
**Steps:**
1. Search for an existing user
2. Select user
3. Click Delete and confirm  
**Expected Result:**  
User should be deleted successfully

---

### TC_ID: A10
**Title:** Verify non-admin user cannot access Admin module  
**Precondition:** Login with non-admin user  
**Steps:**
1. Login as non-admin user
2. Attempt to access Admin module  
**Expected Result:**  
Access should be restricted or Admin module should not be visible
