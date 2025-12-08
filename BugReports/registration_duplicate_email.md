# Bug Report: Registration API returns 500 instead of 400 for duplicate email


**Bug ID:** BR_API_REG_002 
**Title:** Verify Registration API with duplicate email 
**Module:** Login -Registration  
**Severity:** Major  
**Priority:** High  
**Environment:**  
- Base URL: https://www.saucedemo.com/api/register 
- Tool: Postman 
- DB: MySQL (users table)

---

## Description
When sending a registration request with same existing emailed (username, email, password), the API responds with a `500 Internal Server Error`. The expected behaviour is a `400 Bad Request` with a clear validation error message.

---
## Steps to Reproduce
1. Send POST request to /api/register endpoint
2. Provide JSON body with:
   {
     "username": "newuser",
     "email": "existing@example.com",
     "password": "Password123"
   }
3. Observe the response
---

## Expected Result
- Response code = 409 Conflict
- Response body contains "status": "error"
- Message = "Email already registered"
---

## Actual Result
Response code =500  internal server error
Response body contains generic error or stack trace.


