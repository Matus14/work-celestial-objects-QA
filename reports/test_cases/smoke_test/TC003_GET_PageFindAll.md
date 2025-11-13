**Test Case ID:**  
TC003

**Title:**  
 Check if the page request is responsive.

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

- Exam Backend running at `http://localhost:8080`; database connected.

---

**Test Steps:**
1. pen Swagger → GET /api/celestialobjects/(pageable) → Try it out
2. Insert required data in JSON format
3. Execute

---

**Expected Result:**  

-  HTTP 200 OK with correct JSON structure and requested data.

---

**Actual Result:**  

- Received 200 OK with valid response body.

---

**Status:**
- [x] Passed
- [ ] Failed

---

**Comments / Notes:**  


---

**Saved Evidence:**
- Screenshot: `img/SmokeTest-TC003-PageFindAll.PNG`
- Response: `reports/test_cases/smoke_test/evidence/TC-API-003.response.json`