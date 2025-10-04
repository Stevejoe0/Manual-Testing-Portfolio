# Test Cases – Ecommerce Application  

## 1. Introduction  
This document contains detailed test cases for the Ecommerce Web Application.  
It covers modules such as Registration, Login, Product Search, Cart, Checkout, Payment, and Notifications.  

---

## 2. Test Case Format  

| TC ID   | Test Case Description | Pre-Condition | Steps | Expected Result | Priority | Status |
|---------|-----------------------|---------------|-------|-----------------|----------|--------|

- **Priority:** High / Medium / Low  
- **Status:** Pass / Fail / Blocked (to be updated during execution)  

---

## 3. Test Cases  

### 3.1 Registration Module  

| TC ID   | Test Case Description | Pre-Condition | Steps | Expected Result | Priority | Status |
|---------|-----------------------|---------------|-------|-----------------|----------|--------|
| TC-001  | Verify user can register with valid details | App open | 1. Navigate to Register page <br> 2. Enter valid Name, Email, Password, Confirm Password <br> 3. Click Register | User registered successfully; redirected to login page | High | - |
| TC-002  | Verify error when registering with already used email | App open | Enter existing email and valid other details | Error message: "Email already exists" | High | - |
| TC-003  | Verify password mismatch validation | App open | Enter password and confirm password differently | Error message: "Passwords do not match" | High | - |
| TC-004  | Verify password complexity requirement | App open | Enter password with less than 8 characters | Error shown: "Password must be min 8 chars with uppercase, number, symbol" | High | - |

---

### 3.2 Login Module  

| TC ID   | Test Case Description | Pre-Condition | Steps | Expected Result | Priority | Status |
|---------|-----------------------|---------------|-------|-----------------|----------|--------|
| TC-005  | Verify login with valid credentials | User registered | Enter valid email & password | Login successful; user lands on dashboard | High | - |
| TC-006  | Verify login with invalid password | User registered | Enter valid email, invalid password | Error: "Invalid credentials" | High | - |
| TC-007  | Verify account lock after 5 failed attempts | User registered | Enter wrong password 5 times | Account locked; "Too many attempts" message | High | - |
| TC-008  | Verify password reset via email | User registered | Click "Forgot Password" → Enter email → Check mail | Password reset link sent to email | Medium | - |

---

### 3.3 Product Search & Filter  

| TC ID   | Test Case Description | Pre-Condition | Steps | Expected Result | Priority | Status |
|---------|-----------------------|---------------|-------|-----------------|----------|--------|
| TC-009  | Verify product search with valid product name | User logged in | Enter "Laptop" in search bar | List of laptops displayed | High | - |
| TC-010  | Verify search with invalid product name | User logged in | Search for "xyz123" | Message: "No products found" | Medium | - |
| TC-011  | Verify filter by category | User logged in | Select category "Mobiles" | Only mobiles displayed | Medium | - |
| TC-012  | Verify filter by price range | User logged in | Apply filter: 1000–5000 | Products within price range displayed | Medium | - |
| TC-013  | Verify filter by ratings | User logged in | Select filter: "4★ & above" | Only high-rated products displayed | Medium | - |

---

### 3.4 Cart Management  

| TC ID   | Test Case Description | Pre-Condition | Steps | Expected Result | Priority | Status |
|---------|-----------------------|---------------|-------|-----------------|----------|--------|
| TC-014  | Verify adding product to cart | User logged in | Click "Add to cart" on a product | Product added to cart | High | - |
| TC-015  | Verify updating product quantity in cart | Cart not empty | Increase quantity from 1 to 2 | Quantity updated; price recalculated | High | - |
| TC-016  | Verify removing item from cart | Cart not empty | Click "Remove" | Product removed from cart | Medium | - |
| TC-017  | Verify cart total updates dynamically | Cart not empty | Add multiple products | Total updates correctly | High | - |
| TC-018  | Verify empty cart message | Cart empty | Navigate to cart | Message: "Your cart is empty" | Medium | - |

---

### 3.5 Checkout  

| TC ID   | Test Case Description | Pre-Condition | Steps | Expected Result | Priority | Status |
|---------|-----------------------|---------------|-------|-----------------|----------|--------|
| TC-019  | Verify checkout with valid details | Cart not empty | Click Checkout → Enter Address → Proceed | User proceeds to payment page | High | - |
| TC-020  | Verify checkout with missing address | Cart not empty | Leave address blank → Proceed | Error: "Address required" | High | - |
| TC-021  | Verify checkout confirmation step | Cart not empty | Enter details → Review order → Confirm | Order review shown before payment | High | - |

---

### 3.6 Payment  

| TC ID   | Test Case Description | Pre-Condition | Steps | Expected Result | Priority | Status |
|---------|-----------------------|---------------|-------|-----------------|----------|--------|
| TC-022  | Verify payment with valid card details | Checkout initiated | Enter valid card details → Submit | Payment successful → Order confirmed | High | - |
| TC-023  | Verify payment with invalid card number | Checkout initiated | Enter invalid card | Error: "Invalid card details" | High | - |
| TC-024  | Verify UPI payment with valid UPI ID | Checkout initiated | Enter valid UPI ID | Payment successful → Order confirmed | High | - |
| TC-025  | Verify UPI payment with invalid UPI ID | Checkout initiated | Enter invalid UPI ID | Error message displayed | High | - |
| TC-026  | Verify payment with insufficient balance (mocked) | Checkout initiated | Simulate failed transaction | Payment declined; order not placed | High | - |

---

### 3.7 Notifications & Order History  

| TC ID   | Test Case Description | Pre-Condition | Steps | Expected Result | Priority | Status |
|---------|-----------------------|---------------|-------|-----------------|----------|--------|
| TC-027  | Verify confirmation email is sent post-purchase | Order placed | Place order → Check email | Confirmation email received | Medium | - |
| TC-028  | Verify order appears in user order history | Order placed | Navigate to My Orders | Order visible in history | Medium | - |
| TC-029  | Verify order details (products, amount, status) in history | Order placed | Open specific order | Order details displayed correctly | Medium | - |

---

## 4. Test Data  
- Valid user: `user1@test.com / Password@123`  
- Invalid user: `invalid@test.com / WrongPass`  
- Valid card: `4111 1111 1111 1111 / 12-26 / 123`  
- Invalid card: `1234 5678 9012 3456`  
- Valid UPI: `test@upi`  
- Invalid UPI: `fake@upi`  

---

## 5. Summary  
- **Total Test Cases:** 29  
- **High Priority:** 20  
- **Medium Priority:** 9  
- **Low Priority:** 0 (N/A)  
- Coverage: Registration → Payment → Notifications fully covered.  

---

## 6. Approval  
- **Prepared by:** Stephin Joe  
- **Reviewed by:** Test Lead  
- **Approved by:** QA Manager  
