**Test Case ID:**  
TC001

**Title:**  
Create Celestial Object with valid payload

**Test Type:**  
 Smoke

**Priority:**  
 Low

**Tested By:**  
Matus Bucko

**Execution Date:**  
2025-11-13

---

**Preconditions:**  

- Backend running at http://localhost:8080; DB connected.

---

**Test Steps:**
1. Open Swagger → POST /api/celestialobjects → Try it out
2. Paste valid JSON payload
3. Click Execute

---

**Expected Result:**  

- HTTP 201 (or 200) and response body contains created object with non-null `id`; fields match request.

---

**Actual Result:**  

- Response matched expected result

---

**Status:**
- [x] Passed
- [ ] Failed

---

**Comments / Notes:**  


---

**Saved Evidence:**
- Screenshot: `img/SmokeTest-TC001-Create.PNG`
- Response: `reports/test_cases/smoke_test/evidence/TC-API-001.response.json`