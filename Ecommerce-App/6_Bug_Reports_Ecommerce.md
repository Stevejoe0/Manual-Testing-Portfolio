# Bug Reports – Ecommerce Application  

## 1. Introduction  
This document captures the defects identified during testing of the Ecommerce Web Application.  
Each bug is tracked with ID, title, description, severity, priority, and status.  

---

## 2. Bug Report Format  

| Bug ID  | Title | Module | Steps to Reproduce | Expected Result | Actual Result | Severity | Priority | Status |
|---------|-------|--------|--------------------|----------------|---------------|----------|----------|--------|

- **Severity:** Critical / High / Medium / Low  
- **Priority:** High / Medium / Low  
- **Status:** Open / In Progress / Fixed / Retested / Closed  

---

## 3. Bug Reports  

| Bug ID  | Title | Module | Steps to Reproduce | Expected Result | Actual Result | Severity | Priority | Status |
|---------|-------|--------|--------------------|----------------|---------------|----------|----------|--------|
| BUG-001 | Login allows blank password | Login | 1. Go to Login page <br> 2. Enter valid email but leave password blank <br> 3. Click Login | Error message: "Password required" | User logged in without password | High | High | Open |
| BUG-002 | Cart not updating quantity correctly | Cart | 1. Add same product twice <br> 2. Check cart | Quantity should update to 2 | Cart still shows quantity = 1 | Medium | Medium | Open |
| BUG-003 | Invalid UPI accepted as payment | Payment | 1. Go to checkout <br> 2. Select UPI <br> 3. Enter invalid UPI ID (e.g., abc@123) | Payment should be declined | Payment accepted; order placed | Critical | High | Open |
| BUG-004 | Confirmation email not sent after purchase | Notifications | 1. Place order successfully <br> 2. Check registered email | Confirmation email should be sent | No email received | High | Medium | Open |
| BUG-005 | Filter by rating not working | Search | 1. Search "Mobiles" <br> 2. Apply "4★ & above" filter | Only 4★+ products shown | All products displayed regardless of rating | Medium | Low | Open |

---

## 4. Defect Metrics Summary  

- **Total Bugs Reported:** 5  
- **Critical:** 1  
- **High:** 2  
- **Medium:** 2  
- **Low:** 0  

**Defect Density:**  
- Registration: 0  
- Login: 1  
- Search: 1  
- Cart: 1  
- Checkout/Payment: 1  
- Notifications: 1  

---

## 5. Approval  

- **Prepared by:** Stephin Joe 
- **Reviewed by:** Test Lead  
- **Approved by:** QA Manager  

