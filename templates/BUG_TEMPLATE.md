# 🐞 Bug Report Template

---

##  Basic Information
**Bug ID:** BUG-YYYYMMDD-001  
**Reported By:** [Your Name]  
**Date Reported:** [YYYY-MM-DD]  
**Severity:** [Critical / High / Medium / Low]  
**Priority:** [P1 / P2 / P3 / P4]  
**Environment:** [Local / Test / Production]  
**Status:** [New / In Progress / Fixed / Retest / Closed]

---

##  Summary
**Short Description:**  
_A brief one-line summary of the issue._

---

##  Preconditions
_List all setup steps required before reproducing the issue (e.g. user logged in, database seeded, etc.)_

Example:
- Backend server running on `localhost:8080`
- Valid API token available
- Database contains at least one celestial object

---

##  Steps to Reproduce
1. Open Swagger UI or Postman
2. Send a `POST` request to `/api/celestialobjects` with invalid data
3. Observe the API response

---

##  Expected Result
_Describe what should happen if everything works correctly._
> Example: API should return `400 Bad Request` with validation message “Object name must not be empty.”

---

## Actual Result
_Describe what actually happens._
> Example: API returns `500 Internal Server Error` with no validation message.

---

##  Evidence
_Attach screenshots, console logs, or Postman responses (if applicable)._

Example:
- `img/bug_invalid_request.png`
- Postman console output
- Swagger response snippet

---

##  Retesting Notes
_If a fix has been deployed, describe how you verified it._

Example:
> Retested on `v1.2.1` build using Postman — issue no longer occurs.

---

##  Additional Context
_Add any notes that might help developers reproduce or understand the issue (e.g. stack trace, logs, DB data, etc.)._

Example:
```json
{
  "timestamp": "2025-11-10T10:35:21.843+00:00",
  "status": 500,
  "error": "Internal Server Error",
  "message": "Cannot invoke \"Object.getName()\" because object is null"
}