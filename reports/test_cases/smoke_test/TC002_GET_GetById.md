**Test Case ID:**  
TC002

**Title:**  
Get celestial object by ID.

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
1. Open Swagger → GET /api/celestialobjects/{id} → Try it out
2. Enter an existing `id` from previous POST test.
3. Click Execute and observe the response.

---

**Expected Result:**  

- HTTP 200 OK.

---

**Actual Result:**  

- HTTP 200 OK.
- Response matches expected data.
- JSON body returned

---

**Status:**
- [x] Passed
- [ ] Failed

---

**Comments / Notes:**  


---

**Saved Evidence:**
- Screenshot: `img/SmokeTest-TC002-GetById.PNG`
- Response: `reports/test_cases/smoke_test/evidence/TC-API-002.response.json`