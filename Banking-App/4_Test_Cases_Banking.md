# Test Cases – Banking Web Application

## 1. Introduction
This document contains detailed test cases for the **Banking Web Application**, covering modules such as Registration, Login, Account Management, Fund Transfer, Transaction History, Bill Payments, Notifications, and Security.

---

## 2. Test Case Format

| TC ID   | Test Case Description | Pre-Condition | Steps | Expected Result | Priority | Status |
|---------|-----------------------|---------------|-------|-----------------|----------|--------|

- **Priority:** High / Medium / Low  
- **Status:** Pass / Fail / Blocked (to be updated during execution)  

---

## 3. Test Cases

### 3.1 Registration Module

| TC ID   | Test Case Description | Pre-Condition | Steps | Expected Result | Priority | Status |
|---------|----------------------|---------------|-------|-----------------|----------|--------|
| TC-001  | Verify user can register with valid details | App open | 1. Navigate to Registration page <br> 2. Enter valid Name, Email, Password, Confirm Password <br> 3. Click Register | User registered successfully; redirected to login page | High | - |
| TC-002  | Verify error when registering with already used email | App open | Enter existing email and valid other details | Error: "Email already exists" | High | - |
| TC-003  | Verify password mismatch validation | App open | Enter different Password and Confirm Password | Error: "Passwords do not match" | High | - |
| TC-004  | Verify password complexity requirement | App open | Enter password < 8 chars or missing uppercase/number/symbol | Error message displayed | High | - |

---

### 3.2 Login Module

| TC ID   | Test Case Description | Pre-Condition | Steps | Expected Result | Priority | Status |
|---------|----------------------|---------------|-------|-----------------|----------|--------|
| TC-005  | Verify login with valid credentials | User registered | Enter valid email & password | Login successful; dashboard displayed | High | - |
| TC-006  | Verify login with invalid password | User registered | Enter valid email, invalid password | Error: "Invalid credentials" | High | - |
| TC-007  | Verify account lock after 5 failed attempts | User registered | Enter wrong password 5 times | Account locked; "Too many attempts" message | High | - |
| TC-008  | Verify password reset via email | User registered | Click "Forgot Password" → Enter email → Check email | Password reset link sent | Medium | - |

---

### 3.3 Account Management

| TC ID   | Test Case Description | Pre-Condition | Steps | Expected Result | Priority | Status |
|---------|----------------------|---------------|-------|-----------------|----------|--------|
| TC-009  | Verify user can view account balance | User logged in | Navigate to Account Summary | Account balance displayed correctly | High | - |
| TC-010  | Verify user can update personal profile | User logged in | Update profile fields → Save | Profile updated successfully | Medium | - |
| TC-011  | Verify user can change password | User logged in | Enter old password → New password → Confirm | Password changed successfully | High | - |

---

### 3.4 Fund Transfer

| TC ID   | Test Case Description | Pre-Condition | Steps | Expected Result | Priority | Status |
|---------|----------------------|---------------|-------|-----------------|----------|--------|
| TC-012  | Verify internal fund transfer | User logged in, sufficient balance | Navigate to Fund Transfer → Enter details → Submit | Transfer successful | High | - |
| TC-013  | Verify NEFT/IMPS transfer | User logged in, sufficient balance | Enter beneficiary details → Submit | Transfer successful; confirmation displayed | High | - |
| TC-014  | Verify transfer with insufficient balance | User logged in | Enter amount > balance | Error: "Insufficient funds" | High | - |
| TC-015  | Verify transfer to invalid account | User logged in | Enter invalid account number | Error: "Invalid account number" | High | - |

---

### 3.5 Transaction History

| TC ID   | Test Case Description | Pre-Condition | Steps | Expected Result | Priority | Status |
|---------|----------------------|---------------|-------|-----------------|----------|--------|
| TC-016  | Verify viewing transaction history | User logged in | Navigate to Transactions | List of transactions displayed | Medium | - |
| TC-017  | Verify downloading transaction statements | User logged in | Click "Download Statement" | Statement downloaded correctly | Medium | - |

---

### 3.6 Bill Payments

| TC ID   | Test Case Description | Pre-Condition | Steps | Expected Result | Priority | Status |
|---------|----------------------|---------------|-------|-----------------|----------|--------|
| TC-018  | Verify paying utility bills | User logged in, sufficient balance | Navigate to Bill Payments → Select utility → Enter details → Submit | Payment successful; confirmation displayed | High | - |
| TC-019  | Verify bill payment with invalid details | User logged in | Enter invalid bill account | Error: "Invalid bill details" | High | - |

---

### 3.7 Notifications & Security

| TC ID   | Test Case Description | Pre-Condition | Steps | Expected Result | Priority | Status |
|---------|----------------------|---------------|-------|-----------------|----------|--------|
| TC-020  | Verify transaction notification email | Transaction completed | Check registered email | Confirmation email received | Medium | - |
| TC-021  | Verify OTP verification for sensitive actions | User logged in | Initiate fund transfer | OTP sent; must be validated | High | - |
| TC-022  | Verify session timeout after inactivity | User logged in | Remain idle > 5 mins | User logged out automatically | Medium | - |

---

## 4. Test Data

- **Valid user:** user1@bank.com / Password@123  
- **Invalid user:** fake@bank.com / WrongPass  
- **Internal transfer:** Amount = 5000  
- **Bill Payment:** Bill ID = 123456  

---

## 5. Summary

- **Total Test Cases:** 22  
- **High Priority:** 13  
- **Medium Priority:** 9  
- **Coverage:** All modules from Registration → Payment → Notifications → Security covered  

---

## 6. Approval

- **Prepared by:** Stephin Joe 
- **Reviewed by:** Test Lead  
- **Approved by:** QA Manager
