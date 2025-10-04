# Requirements – Banking Web Application

## 1. Introduction
This document defines the functional requirements for the **Banking Web Application**, which allows users to securely register, log in, manage accounts, transfer funds, pay bills, and receive notifications.

---

## 2. Functional Requirements

| Req ID  | Requirement Description                                                | Priority | Module             |
|---------|------------------------------------------------------------------------|----------|------------------|
| REQ-001 | User should be able to register with Name, Email, Password             | High     | Registration      |
| REQ-002 | Password must meet complexity rules                                     | High     | Registration      |
| REQ-003 | User should be able to log in with valid email & password              | High     | Login             |
| REQ-004 | System must lock account after 5 failed login attempts                 | High     | Login             |
| REQ-005 | User should be able to reset password via registered email             | Medium   | Login             |
| REQ-006 | User should be able to view account balance                             | High     | Account Management|
| REQ-007 | User can update personal profile details                                | Medium   | Account Management|
| REQ-008 | User should be able to change password                                  | High     | Account Management|
| REQ-009 | User should be able to transfer funds internally                        | High     | Fund Transfer     |
| REQ-010 | User should be able to transfer funds via NEFT/IMPS                     | High     | Fund Transfer     |
| REQ-011 | System must validate sufficient balance before transfer                 | High     | Fund Transfer     |
| REQ-012 | User should be able to view transaction history                         | Medium   | Transaction History|
| REQ-013 | User should be able to download transaction statements                  | Medium   | Transaction History|
| REQ-014 | User can pay utility bills (Electricity, Water, Mobile)                 | High     | Bill Payments     |
| REQ-015 | Payment system should validate bill details before processing           | High     | Bill Payments     |
| REQ-016 | System should send notifications for successful transactions           | Medium   | Notifications     |
| REQ-017 | System should enforce OTP verification for critical actions             | High     | Security          |
| REQ-018 | Session should timeout after inactivity                                  | Medium   | Security          |
| REQ-019 | Application must work on latest Chrome and Firefox browsers            | High     | General           |
| REQ-020 | Application should handle basic concurrent users (~1000)               | Low      | Performance       |

---

## 3. Non-Functional Requirements

- **Usability:** Responsive UI, mobile-friendly.  
- **Reliability:** Transactions must be secure and persistent.  
- **Security:** Passwords stored encrypted; OTP verification for sensitive actions.  
- **Performance:** Page load time ≤ 3 seconds under normal load.  
- **Compatibility:** Windows 11, Ubuntu 22.04; Chrome & Firefox latest versions.

---

## 4. Assumptions

- Users have stable internet connectivity.  
- NEFT/IMPS & bill payment gateways are mocked for testing.  
- Email notifications are sent via a mock SMTP service.

---

## 5. Approval

- **Prepared by:** Stephin Joe  
- **Reviewed by:** Test Lead  
- **Approved by:** QA Manager
