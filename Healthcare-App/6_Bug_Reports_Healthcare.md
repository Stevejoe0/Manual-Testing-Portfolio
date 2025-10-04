# Bug Reports – Healthcare Web Application

## 1. Introduction
This document captures the defects identified during testing of the **Healthcare Web Application**.  
Each bug is tracked with ID, title, description, severity, priority, and status.

---

## 2. Bug Report Format

| Bug ID  | Title | Module | Steps to Reproduce | Expected Result | Actual Result | Severity | Priority | Status |
|---------|-------|--------|------------------|----------------|---------------|----------|----------|--------|

- **Severity:** Critical / High / Medium / Low  
- **Priority:** High / Medium / Low  
- **Status:** Open / In Progress / Fixed / Retested / Closed  

---

## 3. Bug Reports

| Bug ID  | Title | Module | Steps to Reproduce | Expected Result | Actual Result | Severity | Priority | Status |
|---------|-------|--------|------------------|----------------|---------------|----------|----------|--------|
| BUG-001 | Registration allows blank email | Registration | 1. Go to Registration <br> 2. Leave Email blank <br> 3. Submit | Error: "Email required" | Registration succeeded | High | High | Open |
| BUG-002 | Appointment booking allows past date | Appointment Scheduling | 1. Schedule appointment <br> 2. Select past date <br> 3. Submit | Error: "Invalid date" | Appointment booked | Critical | High | Open |
| BUG-003 | Patient record update fails | Patient Records | 1. Navigate to Patient Records <br> 2. Update details <br> 3. Save | Record updated | Error: "Update failed" | High | High | Open |
| BUG-004 | Payment page accepts invalid card details | Billing & Payments | 1. Go to Billing <br> 2. Enter invalid card number <br> 3. Submit | Payment declined | Payment processed | Critical | High | Open |
| BUG-005 | Session does not timeout after inactivity | Security | 1. Log in <br> 2. Remain idle > 5 mins | User should be logged out | User still logged in | Medium | Medium | Open |

---

## 4. Defect Metrics Summary

- **Total Bugs Reported:** 5  
- **Critical:** 2  
- **High:** 2  
- **Medium:** 1  
- **Low:** 0  

**Defect Density by Module:**  
- Registration: 1  
- Appointment Scheduling: 1  
- Patient Records: 1  
- Billing & Payments: 1  
- Security: 1  

---

## 5. Approval

- **Prepared by:** Stephin Joe  
- **Reviewed by:** Test Lead  
- **Approved by:** QA Manager
