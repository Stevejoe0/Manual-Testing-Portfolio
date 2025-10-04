# Requirement Traceability Matrix (RTM) – Ecommerce Application  

## 1. Introduction  
The Requirement Traceability Matrix (RTM) ensures that all business requirements are covered by corresponding test cases. This provides visibility, completeness, and control over the testing process.  

---

## 2. RTM Table  

| Req ID  | Requirement Description                                               | Test Case IDs           | Status   |
|---------|-----------------------------------------------------------------------|-------------------------|----------|
| REQ-001 | User should be able to register with Name, Email, Password            | TC-001, TC-002, TC-003  | Covered  |
| REQ-002 | Password must meet complexity rules                                   | TC-004, TC-005          | Covered  |
| REQ-003 | User should be able to log in with valid email & password             | TC-006, TC-007          | Covered  |
| REQ-004 | Application must lock account after 5 failed attempts                 | TC-008                  | Covered  |
| REQ-005 | User should be able to reset password via email                       | TC-009, TC-010          | Covered  |
| REQ-006 | User should be able to search products by name                        | TC-011                  | Covered  |
| REQ-007 | User should be able to filter products by category, price, rating     | TC-012, TC-013          | Covered  |
| REQ-008 | User can add products to cart and update quantity                     | TC-014, TC-015          | Covered  |
| REQ-009 | User should be able to remove items from cart                         | TC-016                  | Covered  |
| REQ-010 | Cart must display total price dynamically                             | TC-017, TC-018          | Covered  |
| REQ-011 | User can checkout only if cart is not empty                           | TC-019                  | Covered  |
| REQ-012 | Checkout must include address, payment details, and confirmation step | TC-020, TC-021, TC-022  | Covered  |
| REQ-013 | User should be able to pay using Credit/Debit card, UPI, Net Banking  | TC-023, TC-024, TC-025  | Covered  |
| REQ-014 | Payment gateway must handle invalid details gracefully                | TC-026, TC-027          | Covered  |
| REQ-015 | User should receive confirmation email after successful order         | TC-028                  | Covered  |
| REQ-016 | System should maintain order history                                  | TC-029, TC-030          | Covered  |
| REQ-017 | Application must work on Chrome and Firefox (latest versions)         | TC-031, TC-032          | Covered  |
| REQ-018 | Application should handle 1000 concurrent users (basic performance)   | TC-033                  | Partially (Manual Test Load TBD) |

---

## 3. Notes  
- Status **Covered** means test cases are already mapped.  
- **Partially** indicates additional testing (e.g., performance/load) may require tools beyond manual scope.  
- RTM will be updated after every change in requirements or test cases.  

---

## 4. Approval  
- **Prepared by:** Stephin Joe  
- **Reviewed by:** Test Lead  
- **Approved by:** QA Manager  
