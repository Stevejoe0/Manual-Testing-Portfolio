# Test Cases – Healthcare Web Application

## 1. Introduction
This document contains detailed test cases for the **Healthcare Web Application**, covering modules such as Registration, Login, Appointment Scheduling, Patient Records, Prescription Management, Billing, Notifications, and Security.

---

## 2. Test Case Format

| TC ID   | Test Case Description | Pre-Condition | Steps | Expected Result | Priority | Status |
|---------|----------------------|---------------|-------|-----------------|----------|--------|

- **Priority:** High / Medium / Low  
- **Status:** Pass / Fail / Blocked (to be updated during execution)  

---

## 3. Test Cases

### 3.1 Registration Module

| TC ID   | Test Case Description | Pre-Condition | Steps | Expected Result | Priority | Status |
|---------|----------------------|---------------|-------|-----------------|----------|--------|
| TC-001  | Verify patient registration with valid details | App open | Navigate to Registration → Enter Name, Email, Password → Submit | Registration successful; redirected to login page | High | - |
| TC-002  | Verify doctor registration with valid details | App open | Navigate to Registration → Enter Name, Email, Specialization, Password → Submit | Registration successful; redirected to login page | High | - |
| TC-003  | Verify password complexity validation | App open | Enter invalid password → Submit | Error message displayed | High | - |
| TC-004  | Verify duplicate email registration | App open | Enter already registered email → Submit | Error: "Email already exists" | High | - |

---

### 3.2 Login Module

| TC ID   | Test Case Description | Pre-Condition | Steps | Expected Result | Priority | Status |
|---------|----------------------|---------------|-------|-----------------|----------|--------|
| TC-005  | Verify login with valid credentials | User registered | Enter valid email & password → Login | Login successful; dashboard displayed | High | - |
| TC-006  | Verify login with invalid password | User registered | Enter valid email, invalid password → Login | Error: "Invalid credentials" | High | - |
| TC-007  | Verify account lock after 5 failed attempts | User registered | Enter wrong password 5 times → Login | Account locked; "Too many attempts" message | High | - |
| TC-008  | Verify password reset via email | User registered | Click "Forgot Password" → Enter email → Check email | Password reset link received | Medium | - |

---

### 3.3 Appointment Scheduling

| TC ID   | Test Case Description | Pre-Condition | Steps | Expected Result | Priority | Status |
|---------|----------------------|---------------|-------|-----------------|----------|--------|
| TC-009  | Verify booking a new appointment | Patient logged in | Navigate to Appointments → Select Doctor → Choose Date & Time → Submit | Appointment confirmed | High | - |
| TC-010  | Verify rescheduling an appointment | Patient logged in | Navigate to Appointments → Select existing appointment → Change Date/Time → Submit | Appointment updated successfully | High | - |
| TC-011  | Verify cancelling an appointment | Patient logged in | Navigate to Appointments → Cancel existing appointment | Appointment cancelled successfully | High | - |
| TC-012  | Verify doctor views scheduled appointments | Doctor logged in | Navigate to Doctor Dashboard → View Appointments | List of upcoming appointments displayed | High | - |

---

### 3.4 Patient Records Management

| TC ID   | Test Case Description | Pre-Condition | Steps | Expected Result | Priority | Status |
|---------|----------------------|---------------|-------|-----------------|----------|--------|
| TC-013  | Verify patient views medical history | Patient logged in | Navigate to Patient Records | Medical history displayed | High | - |
| TC-014  | Verify doctor updates patient record | Doctor logged in | Navigate to Patient Records → Update → Save | Record updated successfully | High | - |

---

### 3.5 Prescription Management

| TC ID   | Test Case Description | Pre-Condition | Steps | Expected Result | Priority | Status |
|---------|----------------------|---------------|-------|-----------------|----------|--------|
| TC-015  | Verify doctor creates prescription | Doctor logged in | Navigate to Patient → Add Prescription → Save | Prescription created successfully | High | - |
| TC-016  | Verify patient views/downloads prescription | Patient logged in | Navigate to Prescription → View/Download | Prescription displayed/downloaded | High | - |

---

### 3.6 Billing & Payments

| TC ID   | Test Case Description | Pre-Condition | Steps | Expected Result | Priority | Status |
|---------|----------------------|---------------|-------|-----------------|----------|--------|
| TC-017  | Verify payment for consultation | Patient logged in | Navigate to Billing → Select Appointment → Pay → Submit | Payment successful; receipt generated | High | - |
| TC-018  | Verify viewing invoice history | Patient logged in | Navigate to Billing → View History | List of invoices displayed | Medium | - |

---

### 3.7 Notifications & Security

| TC ID   | Test Case Description | Pre-Condition | Steps | Expected Result | Priority | Status |
|---------|----------------------|---------------|-------|-----------------|----------|--------|
| TC-019  | Verify appointment reminder notification | Appointment scheduled | Check email/SMS | Reminder notification received | Medium | - |
| TC-020  | Verify prescription notification | Prescription created | Check email/SMS | Notification received | Medium | - |
| TC-021  | Verify OTP verification for sensitive actions | Patient/Doctor logged in | Initiate sensitive action | OTP received and must be validated | High | - |
| TC-022  | Verify session timeout after inactivity | User logged in | Remain idle > 5 mins | User logged out automatically | Medium | - |

---

## 4. Test Data

- **Patients:** patient1@health.com / Password@123  
- **Doctors:** doctor1@health.com / Password@123  
- **Appointments:** Valid dates/times for testing  
- **Billing:** Consultation fee = 500  

---

## 5. Summary

- **Total Test Cases:** 22  
- **High Priority:** 12  
- **Medium Priority:** 10  
- **Coverage:** All modules from Registration → Billing → Notifications → Security covered  

---

## 6. Approval

- **Prepared by:** Stephin Joe  
- **Reviewed by:** Test Lead  
- **Approved by:** QA Manager
