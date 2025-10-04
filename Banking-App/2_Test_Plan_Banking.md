# Test Plan – Banking Web Application

## 1. Introduction
The purpose of this Test Plan is to validate the **Banking Web Application** functionalities, ensuring that users can securely register, log in, manage accounts, transfer funds, pay bills, and receive notifications.

---

## 2. Scope

### In Scope
- Functional Testing: Registration, Login, Account Management, Fund Transfer, Transaction History, Bill Payments, Notifications
- Security & Validation checks: OTP, password complexity, session timeout
- UI/UX validation
- Negative & boundary testing
- Regression testing after bug fixes

### Out of Scope
- Load/Performance Testing
- Penetration/Security testing beyond basic validation
- Database tuning

---

## 3. Objectives
- Verify all business requirements are implemented correctly.
- Ensure end-to-end banking flows work seamlessly.
- Identify defects early to improve product quality.

---

## 4. Assumptions
- Requirements are approved.
- Test environment is stable.
- Test data (accounts, transactions) is prepared in advance.

---

## 5. Risks

| Risk Level | Description |
|------------|-------------|
| High       | Payment/fund transfer failures could block test execution. |
| Medium     | Environment downtime may delay testing. |
| Low        | Ambiguous requirements may require test case rework. |

---

## 6. Test Environment
- **Browsers:** Chrome 120+, Firefox 118+  
- **OS:** Windows 11, Ubuntu 22.04  
- **Database:** MySQL / Mock DB  
- **Tools:** Excel (test cases/RTM), Jira (defect tracking), Postman (API sanity checks)

---

## 7. Deliverables
- Test Plan
- Requirements Document
- RTM
- Test Cases & Test Data
- Bug Reports
- Test Execution Report

---

## 8. Entry & Exit Criteria

### Entry Criteria
- Requirements finalized
- Environment ready
- Test cases reviewed

### Exit Criteria
- All high-severity defects resolved
- ≥95% test cases passed
- Test summary report published

---

## 9. Roles & Responsibilities

| Role          | Responsibility |
|---------------|----------------|
| Test Engineer | Prepare and execute test cases, report defects |
| Test Lead     | Review plan, manage execution & reporting |
| Developer     | Fix reported defects |
| Project Manager | Approve release, track progress |

---

## 10. Schedule

| Activity                 | Start Date | End Date |
|--------------------------|------------|----------|
| Requirement Analysis      | Day 1      | Day 2    |
| Test Planning             | Day 3      | Day 4    |
| Test Case Design          | Day 5      | Day 8    |
| Test Execution (Cycle 1)  | Day 9      | Day 12   |
| Defect Fix & Regression   | Day 13     | Day 15   |
| Test Closure              | Day 16     | Day 17   |

---

## 11. Approval
- **Prepared by:** Stephin Joe
- **Reviewed by:** Test Lead  
- **Approved by:** QA Manager
