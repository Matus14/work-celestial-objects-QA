# 🛰 Smoke Test Results
**Project:** Space Catalog API  
**Date:** 2025-11-13  
**Tester:** Matus Bucko  
**Environment:** Localhost (DEV)  
**Backend Version:** v1.0  
**Database:** PostgreSQL – local

---

##  Summary
All defined smoke test cases were executed to verify the critical functionality of the Space Catalog API.  
The purpose of the smoke suite is to confirm that the API is stable enough to continue with deeper functional, negative, and regression testing.

**Overall Result:** ✅ **PASS**  
**Total Tests:** 5  
**Passed:** 5  
**Failed:** 0

---

##  Executed Test Cases

| TC ID | Test Name | Description | Status | Evidence |
|------|------------|-------------|--------|----------|
| **TC001** | POST – Create Valid Object | Valid creation of a celestial object | ✅ PASS | [TC001_POST_CreateValid.md](../test_cases/smoke/TC001_POST_CreateValid.md) |
| **TC002** | GET – Find Object By ID | Retrieve created object using ID | ✅ PASS | [TC002_GET_GetById.md](../test_cases/smoke/TC002_GET_GetById.md) |
| **TC003** | GET – Page & Sort | Retrieve paginated list with sorting | ✅ PASS | [TC003_GET_PageFindAll.md](../test_cases/smoke/TC003_GET_PageFindAll.md) |
| **TC004** | DELETE – Delete Existing Object | Delete object created during the process | ✅ PASS | [TC004_DELETE_deleteObject.md](../test_cases/smoke/TC004_DELETE_deleteObject.md) |
| **TC005** | PUT – Update Existing Object | Update + verify updated values | ✅ PASS | [TC005_PUT_update.md](../test_cases/smoke/TC005_PUT_update.md) |

---

##  Notes & Observations
- API behaved correctly for all critical endpoints.
- Pagination & sorting returned valid structure (`page`, `size`, `sort`).
- DELETE endpoint returned **200 OK**, no content (expected behavior).
- No unexpected errors or delays observed.
- System is ready for deeper testing.

---

##  Conclusion
The build is **stable** and ready for:

### ✔ Functional Testing
### ✔ Negative Testing
### ✔ Regression Testing
### ✔ Integration Testing
