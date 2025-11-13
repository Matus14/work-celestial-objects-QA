**Test Case ID:**  
TC005

**Title:**  
Test of the PUT-update works as intended

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
1. Open Swagger → PUT /api/celestialobjects/{id} → Try it out
2. Insert `id` of the object we want to test
3. Fill up the request body based on changes we want to make
4. Click Execute and observe the response.


---

**Expected Result:**  

- Response returns HTTP 200 OK with correct JSON structure.

---

**Actual Result:**  

-  Received 200 OK with valid response body, all changes successfully applied to the object

---

**Status:**
- [x] Passed
- [ ] Failed

---

**Comments / Notes:**  


---

**Saved Evidence:**
- Screenshot: `img/SmokeTest-TC005-Update.PNG`
- Response: `reports/test_cases/smoke_test/evidence/TC-API-005.response.json`