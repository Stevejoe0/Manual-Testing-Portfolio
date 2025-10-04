# Requirements – Healthcare Web Application

## 1. Introduction
This document defines the functional requirements for the **Healthcare Web Application**, which allows patients and doctors to securely register, schedule appointments, manage medical records, create prescriptions, make payments, and receive notifications.

---

## 2. Functional Requirements

| Req ID  | Requirement Description                                               | Priority | Module                 |
|---------|-----------------------------------------------------------------------|----------|-----------------------|
| REQ-001 | User (patient/doctor) should be able to register with Name, Email, Password | High     | Registration          |
| REQ-002 | Password must meet complexity rules                                   | High     | Registration          |
| REQ-003 | User should be able to log in with valid email & password             | High     | Login                 |
| REQ-004 | System must lock account after 5 failed login attempts               | High     | Login                 |
| REQ-005 | User should be able to reset password via registered email           | Medium   | Login                 |
| REQ-006 | Patients should be able to schedule appointments                     | High     | Appointment Scheduling|
| REQ-007 | Patients should be able to reschedule or cancel appointments         | High     | Appointment Scheduling|
| REQ-008 | Doctors should be able to view scheduled appointments                | High     | Appointment Scheduling|
| REQ-009 | User should be able to view and update patient records               | High     | Patient Records       |
| REQ-010 | Doctors should be able to create prescriptions                        | High     | Prescription Management|
| REQ-011 | Patients should be able to view/download prescriptions               | High     | Prescription Management|
| REQ-012 | Users should be able to make payments for consultations              | High     | Billing & Payments    |
| REQ-013 | Users should be able to view invoice/payment history                 | Medium   | Billing & Payments    |
| REQ-014 | System should send notifications for appointments, prescriptions, and payments | Medium | Notifications         |
| REQ-015 | System should enforce OTP verification for sensitive actions         | High     | Security & Compliance |
| REQ-016 | Session should timeout after inactivity                                | Medium   | Security & Compliance |
| REQ-017 | Application must work on latest Chrome and Firefox browsers          | High     | General               |
| REQ-018 | Application should handle basic concurrent users (~500)              | Low      | Performance           |

---

## 3. Non-Functional Requirements

- **Usability:** Responsive UI, mobile-friendly.  
- **Reliability:** Data must be accurate and persistent.  
- **Security & Compliance:** HIPAA/GDPR compliant, secure data storage.  
- **Performance:** Page load time ≤ 3 seconds under normal load.  
- **Compatibility:** Windows 11, Ubuntu 22.04; Chrome & Firefox latest versions.

---

## 4. Assumptions

- Users have stable internet connectivity.  
- Appointment and billing gateways are mocked for testing.  
- Email/SMS notifications are sent via a mock service.  

---

## 5. Approval

- **Prepared by:** Stephin Joe  
- **Reviewed by:** Test Lead  
- **Approved by:** QA Manager
