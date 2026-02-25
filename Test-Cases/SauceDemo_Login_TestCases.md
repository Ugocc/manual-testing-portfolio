# SauceDemo Login Module – Test Cases

**Test Case ID:** TC_LOGIN_001  
**Title:** Verify user can log in with valid credentials  
**Module:** Login  
**Priority:** High  
**Preconditions:** User account exists  

**Test Data:**  
- Username: `standard_user`  
- Password: `secret_sauce`  

**Test Steps:**  
1. Navigate to https://www.saucedemo.com/
2. Enter valid username  
3. Enter valid password  
4. Click **Login**  

**Expected Result:**  
- User is successfully redirected to the Inventory page  

**Actual Result:**  
- To be filled after execution -User is successfully redirected to the Inventory page  
 

**Status:**  
☑ Pass
☐ Fail

## Test Case ID: TC_LOGIN_002 
**Title:** Verify error message when password is incorrect  
**Module:** Login  
**Priority:** High  
**Preconditions:** User account exists  

**Test Data:**  
- Username: `standard_user`  
- Password: `wrong_passowrd`  

**Test Steps:**  
1. Navigate to https://www.saucedemo.com/
2. Enter valid username  
3. Enter invalid password  
4. Click **Login**  

**Expected Result:**  
- Error message displayed indicating invalid credentials 

**Actual Result:**  
- To be filled after execution  -Error message displayed indicating invalid credentials 

**Status:**  
-☑ Pass
 ☐ Fail

  ## Test Case ID: TC_LOGIN_003
**Title:** Verify error message when username is empty  
**Module:** Login  
**Priority:** Medium  
**Preconditions:** correct password is inputed  
**Test Data:** Password: `secret_sauce` 
               username: empty
**Test Steps:**  
1. Navigate to login page  
2. Leave username empty  
3. Enter valid password  
4. Click **Login**  
**Expected Result:** Error message displayed indicating username is required  
**Actual Result:** To be filled after execution  - Error message displayed indicating username is required  
**Status:** ☑ Pass
            ☐ Fail 
**Comments:** (Any additional observations)

---

## Test Case ID: TC_LOGIN_004
**Title:** Verify error message when password is empty  
**Module:** Login  
**Priority:** Medium  
**Preconditions:** User account exists, valid username is inputed 
**Test Data:** Username: `standard_user`
               Password:   empty
**Test Steps:**  
1. Navigate to login page  
2. Enter valid username  
3. Leave password empty  
4. Click **Login**  
**Expected Result:** Error message displayed indicating password is required  
**Actual Result:** To be filled after execution  -Error message displayed indicating password is required 
**Status:** ☑ Pass
            ☐ Fail 
**Comments:** (Any additional observations)

---

## Test Case ID: TC_LOGIN_005
**Title:** Verify error message for locked user  
**Module:** Login  
**Priority:** High  
**Preconditions:** User account is locked (`locked_out_user`)  
**Test Data:** Username: `locked_out_user`, Password: `secret_sauce`  
**Test Steps:**  
1. Navigate to login page  
2. Enter locked user username  
3. Enter password  
4. Click **Login**  
**Expected Result:** Error message displayed indicating the user is locked out  
**Actual Result:** To be filled after execution  -Error message displayed indicating the user is locked out  
**Status:**  ☑ Pass
             ☐ Fail 
**Comments:** (Any additional observations)

 ## Test Case ID: TC_LOGIN_006
**Title:** Verify error message when username is incorrect  
**Module:** Login  
**Priority:** High 
**Preconditions:** User is on login page
**Test Data:** Password: `secret_sauce` 
               username: invalid
**Test Steps:**  
1. Navigate to login page  
2. enter invalid user name  
3. Enter valid password  
4. Click **Login**  
**Expected Result:** Error message displayed indicating Username or password do not match any user in this service
**Actual Result:** To be filled after execution- Error message is displayed indicating that the username and password do not match any user in the service 
  
**Status:** ☑ Pass
            ☐ Fail 
**Comments:** (Any additional observations)

---
## Test Case ID: TC_LOGIN_007

**Title:** Verify login using Enter key instead of clicking Login button  

**Module:** Login  

**Priority:** Medium  

**Preconditions:**  
- Valid user account exists  

**Test Data:**  
- Username: `standard_user`  
- Password: `secret_sauce`  

**Test Steps:**  
1. Navigate to login page  
2. Enter valid username  
3. Enter valid password  
4. Press **Enter key** on keyboard  

**Expected Result:**  
- User is successfully logged in  
- User is redirected to Inventory page  

**Actual Result:**  
To be filled after execution
  - User is successfully logged in  
  - User is redirected to Inventory page  

**Status:**  
 ☑ Pass
 ☐ Fail  

**Comments:**  
(Any additional observations)

## Test Case ID: TC_LOGIN_008

**Title:** Verify login fails with invalid username/password formats

**Module:** Login  

**Priority:** High  

**Preconditions:**  
- Valid user account exists
- User is on login page  

**Test Data Variations:**  
SCENARIO	          USERNAME          	        PASSWORD
Leading Space	      standard_user	             secret_sauce
Trailing Space	     standard_user	           secret_sauce
Special Characters	 standard_user@@@	         secret_sauce


**Test Steps:**  
1. Navigate to login page  
2. Enter valid username  
3. Enter valid password  
4. Press **Enter key** on keyboard  

**Expected Result:**  
- Username and password do not match any user in this service  


**Actual Result:**  
To be filled after execution
 Username and password do not match any user in this service

**Status:**  
 ☑ Pass
 ☐ Fail  

**Comments:**  
(Any additional observations)
