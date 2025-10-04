# Test Plan – Ecommerce Application  

## 1. Introduction  
The purpose of this Test Plan is to validate the **Ecommerce Web Application** functionalities, ensuring that users can register, log in, search for products, add to cart, complete checkout, and receive order confirmation.  

---

## 2. Scope  

### In Scope  
- Functional Testing (Registration, Login, Search, Cart, Checkout, Payment, Order Confirmation)  
- UI/UX validation (labels, fields, buttons, alignment)  
- Negative & Boundary testing  
- Regression Testing after bug fixes  

### Out of Scope  
- Load & Performance Testing  
- Security Penetration Testing  
- Database performance tuning  

---

## 3. Objectives  
- Verify that all business requirements are implemented correctly.  
- Ensure end-to-end user flows work seamlessly.  
- Identify defects early and improve product quality.  

---

## 4. Assumptions  
- Requirements are baseline and approved.  
- Test environment is stable.  
- Test data will be prepared in advance.  

---

## 5. Risks  

| Risk Level | Description |
|------------|-------------|
| High       | Payment gateway integration issues may block test execution. |
| Medium     | Test environment downtime could delay schedule. |
| Low        | Ambiguous requirements may cause test case rework. |

---

## 6. Test Environment  

- **Browser:** Chrome 120+, Firefox 118+  
- **OS:** Windows 11, Ubuntu 22.04  
- **Database:** MySQL (mock)  
- **Tools:** Excel (test cases/RTM), Jira (defect management), Postman (API sanity, if needed)  

---

## 7. Deliverables  

- Test Plan  
- Requirements Document  
- Requirement Traceability Matrix (RTM)  
- Test Cases & Test Data  
- Bug Reports  
- Test Execution Report  

---

## 8. Entry & Exit Criteria  

### Entry Criteria  
- Requirements finalized and approved  
- Test environment ready  
- Test cases prepared and reviewed  

### Exit Criteria  
- All high-severity defects resolved  
- ≥95% of test cases passed  
- Test summary report published  

---

## 9. Roles & Responsibilities  

| Role         | Responsibility |
|--------------|----------------|
| Test Engineer | Prepare test cases, execute, report defects |
| Test Lead     | Review plan, manage execution & reporting |
| Developer     | Fix reported defects |
| Project Manager | Approve releases, track progress |

---

## 10. Schedule  

| Activity                | Start Date | End Date |
|--------------------------|------------|----------|
| Requirement Analysis     | Day 1      | Day 2    |
| Test Planning            | Day 3      | Day 4    |
| Test Case Design         | Day 5      | Day 8    |
| Test Execution (Cycle 1) | Day 9      | Day 12   |
| Defect Fix & Regression  | Day 13     | Day 15   |
| Test Closure             | Day 16     | Day 17   |

---

## 11. Approval  

- **Prepared by:** Stephin Joe  
- **Reviewed by:** Test Lead  
- **Approved by:** QA Manager  


📎 [Download Test Plan (Word Document)](./1_Test_Plan_Ecommerce.docx)
