# Bug Report: Registration API returns 500 instead of 400 for missing fields

**Bug ID:** BUG_API_REG_001  
**Title:** Registration API returns 500 Internal Server Error when required fields are missing  
**Module:** Registration API  
**Severity:** Major  
**Priority:** High  
**Environment:**  
- Base URL: https://www.saucedemo.com/api/register  
- Tool: Postman  
- DB: MySQL (users table)  

---

## Description
When sending a registration request with missing fields (username, email, password), the API responds with a `500 Internal Server Error`. The expected behavior is a `400 Bad Request` with a clear validation error message.

---

## Steps to Reproduce
1. Open Postman and create a `POST` request to `/api/register`.  
2. Set header: `Content-Type: application/json`.  
3. Provide the following JSON body:
   ```json
   {
     "username": "",
     "email": "",
     "password": ""
   }
- Send the request.

Expected Result
- Response code = 400 Bad Request
- Response body:
{
  "status": "error",
  "message": "Username, email, and password are required"
}



Actual Result
- Response code = 500 Internal Server Error
- Response body contains generic error or stack trace.
