**Test Case ID:**  
TC004

**Title:**  
Test to check if the DELETE works as intended

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

-  Backend running at `http://localhost:8080`; database connected.

---

**Test Steps:**
1. Open Swagger → DELETE /api/celestialobjects/{id} → Try it out
2. Insert `id` of the object we want to test
3. Execute

---

**Expected Result:**  

- Response returns HTTP 200 OK - object will be deleted

---

**Actual Result:**  

- Received 200 OK DELETE completed 

---

**Status:**
- [x] Passed
- [ ] Failed

---

**Comments / Notes:**  


---

**Saved Evidence:**
- Screenshot: `img/SmokeTest-TC004-Delete.PNG`
- Response: `reports/test_cases/smoke_test/evidence/TC-API-004.response.json`