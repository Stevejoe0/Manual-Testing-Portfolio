# Requirement Traceability Matrix (RTM) – Banking Web Application

## 1. Introduction
The Requirement Traceability Matrix (RTM) ensures that all functional requirements of the **Banking Web Application** are mapped to corresponding test cases, providing visibility, completeness, and control over the testing process.

---

## 2. RTM Table

| Req ID  | Requirement Description                                               | Test Case IDs           | Status   |
|---------|-----------------------------------------------------------------------|------------------------|----------|
| REQ-001 | User should be able to register with Name, Email, Password            | TC-001, TC-002         | Covered  |
| REQ-002 | Password must meet complexity rules                                   | TC-003, TC-004         | Covered  |
| REQ-003 | User should be able to log in with valid email & password             | TC-005, TC-006         | Covered  |
| REQ-004 | System must lock account after 5 failed login attempts               | TC-007                  | Covered  |
| REQ-005 | User should be able to reset password via registered email           | TC-008, TC-009         | Covered  |
| REQ-006 | User should be able to view account balance                           | TC-010                  | Covered  |
| REQ-007 | User can update personal profile details                               | TC-011                  | Covered  |
| REQ-008 | User should be able to change password                                 | TC-012                  | Covered  |
| REQ-009 | User should be able to transfer funds internally                       | TC-013, TC-014         | Covered  |
| REQ-010 | User should be able to transfer funds via NEFT/IMPS                    | TC-015, TC-016         | Covered  |
| REQ-011 | System must validate sufficient balance before transfer               | TC-017                  | Covered  |
| REQ-012 | User should be able to view transaction history                        | TC-018, TC-019         | Covered  |
| REQ-013 | User should be able to download transaction statements                 | TC-020                  | Covered  |
| REQ-014 | User can pay utility bills (Electricity, Water, Mobile)                | TC-021, TC-022         | Covered  |
| REQ-015 | Payment system should validate bill details before processing          | TC-023                  | Covered  |
| REQ-016 | System should send notifications for successful transactions          | TC-024, TC-025         | Covered  |
| REQ-017 | System should enforce OTP verification for critical actions            | TC-026, TC-027         | Covered  |
| REQ-018 | Session should timeout after inactivity                                 | TC-028                  | Covered  |
| REQ-019 | Application must work on latest Chrome and Firefox browsers           | TC-029, TC-030         | Covered  |
| REQ-020 | Application should handle basic concurrent users (~1000)              | TC-031                  | Partially |

---

## 3. Notes
- Status **Covered** means test cases are mapped and ready for execution.  
- Status **Partially** indicates additional testing (e.g., performance/load testing) may be required beyond manual scope.  
- RTM will be updated after changes in requirements or test cases.

---

## 4. Approval
- **Prepared by:** Stephin Joe  
- **Reviewed by:** Test Lead  
- **Approved by:** QA Manager
