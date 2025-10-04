# Requirement Traceability Matrix (RTM) – Healthcare Web Application

## 1. Introduction
The Requirement Traceability Matrix (RTM) ensures that all functional requirements of the **Healthcare Web Application** are mapped to corresponding test cases, providing visibility, completeness, and control over the testing process.

---

## 2. RTM Table

| Req ID  | Requirement Description                                               | Test Case IDs           | Status   |
|---------|-----------------------------------------------------------------------|------------------------|----------|
| REQ-001 | User (patient/doctor) should be able to register with Name, Email, Password | TC-001, TC-002         | Covered  |
| REQ-002 | Password must meet complexity rules                                   | TC-003, TC-004         | Covered  |
| REQ-003 | User should be able to log in with valid email & password             | TC-005, TC-006         | Covered  |
| REQ-004 | System must lock account after 5 failed login attempts               | TC-007                  | Covered  |
| REQ-005 | User should be able to reset password via registered email           | TC-008, TC-009         | Covered  |
| REQ-006 | Patients should be able to schedule appointments                     | TC-010, TC-011         | Covered  |
| REQ-007 | Patients should be able to reschedule or cancel appointments         | TC-012, TC-013         | Covered  |
| REQ-008 | Doctors should be able to view scheduled appointments                | TC-014                  | Covered  |
| REQ-009 | User should be able to view and update patient records               | TC-015, TC-016         | Covered  |
| REQ-010 | Doctors should be able to create prescriptions                        | TC-017, TC-018         | Covered  |
| REQ-011 | Patients should be able to view/download prescriptions               | TC-019, TC-020         | Covered  |
| REQ-012 | Users should be able to make payments for consultations              | TC-021, TC-022         | Covered  |
| REQ-013 | Users should be able to view invoice/payment history                 | TC-023                  | Covered  |
| REQ-014 | System should send notifications for appointments, prescriptions, and payments | TC-024, TC-025         | Covered  |
| REQ-015 | System should enforce OTP verification for sensitive actions         | TC-026, TC-027         | Covered  |
| REQ-016 | Session should timeout after inactivity                                | TC-028                  | Covered  |
| REQ-017 | Application must work on latest Chrome and Firefox browsers          | TC-029, TC-030         | Covered  |
| REQ-018 | Application should handle basic concurrent users (~500)              | TC-031                  | Partially |

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
