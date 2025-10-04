# Bug Reports – Banking Web Application

## 1. Introduction
This document captures the defects identified during testing of the **Banking Web Application**.  
Each bug is tracked with ID, title, description, severity, priority, and status.

---

## 2. Bug Report Format

| Bug ID  | Title | Module | Steps to Reproduce | Expected Result | Actual Result | Severity | Priority | Status |
|---------|-------|--------|-------------------|----------------|---------------|----------|----------|--------|

- **Severity:** Critical / High / Medium / Low  
- **Priority:** High / Medium / Low  
- **Status:** Open / In Progress / Fixed / Retested / Closed  

---

## 3. Bug Reports

| Bug ID  | Title | Module | Steps to Reproduce | Expected Result | Actual Result | Severity | Priority | Status |
|---------|-------|--------|------------------|----------------|---------------|----------|----------|--------|
| BUG-001 | Login allows blank password | Login | 1. Go to Login page <br> 2. Leave password blank <br> 3. Click Login | Error message: "Password required" | User logged in without password | High | High | Open |
| BUG-002 | Account balance not updated after transfer | Account Management/Fund Transfer | 1. Transfer funds to another account <br> 2. Check account balance | Balance should reduce correctly | Balance remains same | Critical | High | Open |
| BUG-003 | OTP not sent during fund transfer | Fund Transfer/Security | 1. Initiate transfer requiring OTP <br> 2. Check registered mobile/email | OTP received | No OTP received | Critical | High | Open |
| BUG-004 | Bill payment succeeds with invalid bill ID | Bill Payments | 1. Enter invalid bill account <br> 2. Submit | Error: "Invalid bill details" | Payment processed successfully | High | Medium | Open |
| BUG-005 | Session does not timeout after inactivity | Security | 1. Log in <br> 2. Remain idle > 5 mins | User should be logged out automatically | User still logged in | Medium | Medium | Open |

---

## 4. Defect Metrics Summary

- **Total Bugs Reported:** 5  
- **Critical:** 2  
- **High:** 2  
- **Medium:** 1  
- **Low:** 0  

**Defect Density by Module:**  
- Registration: 0  
- Login: 1  
- Account Management: 1  
- Fund Transfer: 2  
- Bill Payments: 1  
- Security: 1  

---

## 5. Approval

- **Prepared by:** Stephin Joe  
- **Reviewed by:** Test Lead  
- **Approved by:** QA Manager
