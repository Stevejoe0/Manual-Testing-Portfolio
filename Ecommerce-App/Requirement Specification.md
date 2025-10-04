# Requirements – Ecommerce Application

## 1. Introduction
This document defines the functional requirements for the **Ecommerce Web Application**, which allows users to register, log in, search products, add them to a cart, checkout, and make payments.

---

## 2. Functional Requirements

| Req ID  | Requirement Description                                                                 | Priority | Module        |
|---------|-----------------------------------------------------------------------------------------|----------|---------------|
| REQ-001 | User should be able to register with Name, Email, Password, and Confirm Password        | High     | Registration  |
| REQ-002 | Password must be minimum 8 characters, include uppercase, lowercase, number, and symbol | High     | Registration  |
| REQ-003 | User should be able to log in with valid email & password                               | High     | Login         |
| REQ-004 | Application must validate incorrect login attempts (lock after 5 failed attempts)       | High     | Login         |
| REQ-005 | User should be able to reset password via email                                         | Medium   | Login         |
| REQ-006 | User should be able to search products by name                                          | High     | Search        |
| REQ-007 | User should be able to filter products by category, price range, and rating             | Medium   | Search        |
| REQ-008 | User can add products to cart and update quantity                                       | High     | Cart          |
| REQ-009 | User should be able to remove items from cart                                           | Medium   | Cart          |
| REQ-010 | Cart must display total price dynamically                                               | High     | Cart          |
| REQ-011 | User can proceed to checkout only if the cart is not empty                              | High     | Checkout      |
| REQ-012 | Checkout process must include delivery address, payment details, and confirmation step  | High     | Checkout      |
| REQ-013 | User should be able to pay using Credit/Debit card, UPI, and Net Banking                | High     | Payment       |
| REQ-014 | Payment gateway must handle invalid card/UPI details gracefully                         | High     | Payment       |
| REQ-015 | User should receive a confirmation email after successful order placement               | Medium   | Notifications |
| REQ-016 | System should maintain order history for logged-in users                                | Medium   | Orders        |
| REQ-017 | Application must be accessible via Chrome and Firefox (latest versions)                 | High     | General       |
| REQ-018 | Application should handle up to 1000 concurrent users (basic performance requirement)   | Low      | General       |

---

## 3. Non-Functional Requirements

- **Usability:** UI must be responsive and mobile-friendly.  
- **Reliability:** Application must ensure that transactions are not lost during server failures.  
- **Security:** Passwords must be stored encrypted (SHA-256 or better).  
- **Performance:** Average page load time should be ≤ 3 seconds.  
- **Compatibility:** Should work on Windows 11 and Ubuntu 22.04.  

---

## 4. Assumptions

- Users have stable internet connectivity.  
- Payment gateway is simulated for testing purposes.  
- Emails are sent using a mock SMTP service in the test environment.  

---

## 5. Approval

- **Prepared by:** Stephin Joe  
- **Reviewed by:** Test Lead  
- **Approved by:** QA Manager  
