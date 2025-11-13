# One-Page Test Plan - Celestial Objects API(v 1.0)

---

## 1. Project Overview
The purpose of the Celestial Objects project is to provide a REST API that manages data about astronomical objects such as planets, moons, and stars.  
The backend is implemented in Java (Spring Boot 3) and uses PostgreSQL as the database.  
This test plan defines the QA strategy, objectives, and scope of testing for this API.

---

## 2. Objectives
- Verify that all REST API endpoints function correctly and return valid responses.
- Validate database operations (data persistence, update, deletion).
- Ensure that invalid inputs return appropriate error messages.
- Confirm that the system meets functional and non-functional requirements.
- Identify and document any defects or inconsistencies.

---

## 3. Scope of Testing

### In Scope
- CRUD operations on Celestial Objects (Create, Read, Update, Delete)
- API validation using Swagger UI and Postman
- Input validation and error handling
- Database data integrity verification

### Out of Scope
- Frontend testing (no UI is part of this project)
- Performance and load testing
- Security and penetration testing

---

## 4. Test Approach
Testing will be performed manually using tools such as **Postman**, **Swagger UI**, and **DBeaver**.  
Each endpoint will be validated using positive and negative test cases.  
Testing will follow a structured process:

1. Verify API availability (smoke tests).
2. Execute CRUD operations with valid data.
3. Perform negative testing using invalid or missing parameters.
4. Cross-check data stored in the PostgreSQL database.
5. Log any defects and re-test after fixes.

---

## 5. Test Types
- Smoke Testing
- Functional Testing
- Negative Testing
- Regression Testing
- Database Testing

---

## 6. Test Environment
| Component | Description |
|------------|-------------|
| Application Type | REST API |
| Backend | Java 21, Spring Boot 3 |
| Database | PostgreSQL 16 |
| Tools | Postman, Swagger UI, DBeaver, IntelliJ IDEA |
| Test Environment URL | http://localhost:8080 |

---

## 7. Test Data
Test data will include valid and invalid values for object fields such as:
- objectName
- objectType
- objectDesignation
- discoveryYear
- distanceFromSunAu
- objectMassToEarth
- objectSpeedKmS

Test data will be created manually and managed using Postman collections.

---

## 8. Entry and Exit Criteria

### Entry Criteria
- Backend application is deployed and accessible on localhost.
- Database is configured and connected.
- Swagger documentation is available.
- Test data is prepared.

### Exit Criteria
- All planned test cases are executed.
- All critical defects are resolved or deferred with justification.
- Test summary report is completed.

---

## 9. Deliverables
- Test Plan (this document)
- Test Cases (Postman collection)
- Test Reports (in /reports folder)
- Defect Reports (in /reports/defects folder)
- Final QA Summary

---

## 10. Risks and Assumptions
| Risk | Mitigation |
|------|-------------|
| Environment configuration issues | Validate setup before testing |
| Database connection problems | Keep connection settings in config file |
| Limited test data | Use generated and boundary data sets |
| Time constraints | Prioritize smoke and functional tests first |

---

## 11. Approval
Prepared by: **Matúš Bučko**  
Role: QA Engineer / Java Developer  
Date: 10 November 2025  
Version: 1.0