
# Celestial Objects – QA & Testing Repository

This repository contains all QA and manual testing documentation for the Celestial Objects API project, a Spring Boot backend connected to a PostgreSQL database.  
The goal of this repository is to demonstrate the full testing workflow that a QA engineer would follow in a real project.

---

## Project Overview
The tested application is a REST API called Celestial Objects, which manages data about planets, stars, and other astronomical entities.  
The backend is developed in Java 21 (Spring Boot 3) and integrated with PostgreSQL 16.

Main repository under test:  
[work-celestial-objects-BE](https://github.com/Matus14/work-celestial-objects-BE)

---

## Repository Structure
/docs/ → Exported Swagger or API documentation
/postman/ → Postman collections and environment files
/reports/ → Test results and QA reports
/reports/defects/ → Logged defects and bug reports
TestPlan_OnePage.md → High-level QA test plan
README.md → Repository overview

---

## Tools and Technologies Used
| Tool | Purpose |
|------|----------|
| Postman | Manual API testing |
| Swagger UI | API documentation and endpoint verification |
| DBeaver / pgAdmin | Database validation |
| IntelliJ IDEA | Backend execution and code review |
| Git / GitHub | Version control and documentation storage |

---

## Test Types Covered
- Smoke testing – checking API availability and basic functionality
- Functional testing – verifying CRUD operations (Create, Read, Update, Delete)
- Negative testing – validating error responses and incorrect inputs
- Database testing – ensuring data is stored and updated correctly
- Regression testing – verifying stability after code updates

---

## Defect Management
All discovered defects are documented under:
/reports/defects/

Each defect follows this structure:
D:
Title:
Environment:
Steps to Reproduce:
Expected Result:
Actual Result:
Severity:
Status:

File naming convention:
BUG-001_DuplicateNameConflict.md
BUG-002_MissingValidationCheck.md

---

## Reporting
Each test session or day of testing is summarized in a report file located in the `/reports/` directory.  
Example:
2025-11-10_SmokeResults.md

Reports include:
- Executed test cases
- Test environment details
- Pass/Fail summary
- Notes and observations

---

## API Documentation
Swagger UI is available when the backend application is running:
http://localhost:8080/swagger-ui/index.html


## Author
Matúš Bučko  
QA Engineer / Java Developer  
Slovakia  
[LinkedIn Profile](https://www.linkedin.com/in/matus-bucko-771b73313)

---

This repository demonstrates a realistic QA workflow, including test planning, execution, defect management, and structured reporting for a REST API application.