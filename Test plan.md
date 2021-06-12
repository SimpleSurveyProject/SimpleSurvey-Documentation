
# Test plan
## 1.	Introduction
### 1.1	Purpose
The purpose of the Iteration Test Plan is to gather all of the information necessary to plan and control the test effort for a given iteration. 
It describes the approach to testing the software.
This Test Plan for **SimpleSurvey** supports the following objectives:
-	Identifies the items that should be targeted by the tests.
-	Identifies the motivation for and ideas behind the test areas to be covered.
-	Outlines the testing approach that will be used.
-	Identifies the required resources and provides an estimate of the test efforts.
### 1.2	Scope
This document describes the used tests (Unit tests, End-to-End tests, Swagger UI).
### 1.3	Intended Audience
This document is meant for internal use primarily.
### 1.4	Document Terminology and Acronyms
| Abbrevation | Explanation                            |
| ----------- | -------------------------------------- |
| MVC         | Model View Controller |
| UC          | Use Case                               |
| UCD         | Use Case Diagram                       |
| n/a         | not applicable                         |
| tbd         | to be determined                       |

### 1.5	 References
| Title                                                              |
| -------------------------------------------------------------------|
| [SimpleSurvey Blog](https://simplesurveyproject.wordpress.com)     |
| [GitHub](https://github.com/SimpleSurveyProject)                   |
| [WebApp](https://simplesurvey.de)                                  |
| [SRS](https://github.com/SimpleSurveyProject/SimpleSurvey-Documentation/blob/main/Software%20Requirements%20Specification.md)|
| [MVC Diagram](https://github.com/SimpleSurveyProject/SimpleSurvey-Documentation/blob/main/ressources/MVC.png)  |
| [Use Case Diagram](https://screen.simonlabs.de/img.php?id=2I0cisf)  |
| [Fill out survey Use Case](https://github.com/SimpleSurveyProject/SimpleSurvey-Documentation/blob/main/use-cases/use-case-fillsOutSurvey.md)  |
| [Share survey Use Case](https://github.com/SimpleSurveyProject/SimpleSurvey-Documentation/blob/main/use-cases/use-case-sharesSurvey.md)  |
| [Create survey Use Case](https://github.com/SimpleSurveyProject/SimpleSurvey-Documentation/blob/main/use-cases/use-case-createSurvey.md)  |
| [Edit survey Use Case](https://github.com/SimpleSurveyProject/SimpleSurvey-Documentation/blob/main/use-cases/use-case-editSurvey.md)  |
| [Evaluate survey Use Case](https://github.com/SimpleSurveyProject/SimpleSurvey-Documentation/blob/main/use-cases/use-case-evaluateSurvey.md)  |
| [Architecture](https://puu.sh/HO32X/997aef87b5.png)  |
| [Deployment](https://screen.simonlabs.de/img.php?id=2HVXfjn)  |
| [Database model](ressources/dbmodel.png)  |

  
## 2.	Evaluation Mission and Test Motivation
### 2.1	Background
By testing source code, we ensure our application to run smoothly. The goal is to make sure, that our application does not run into any unexpected errors.
### 2.2	Evaluation Mission
The mission of this test plan is to prevent errors in production and ensure an outstanding software quality.
### 2.3	Test Motivators
Our testing is motivated by 
- quality risks 
- technical risks
- use cases 
- functional requirements
## 3.	Target Test Items
The listing below identifies those test items (software, hardware, and supporting product elements) that have been identified as targets for testing. 
This list represents what items will be tested. 
Items for Testing:
- Spring Boot Backend
- Angular Frontend
- Connection between both components
## 4.	Outline of Planned Tests
### 4.1	Outline of Test Inclusions
- Testing the backend with unit tests. 
- End2End testing the frontend application.
- Documentation and Testing of the API with Swagger UI
### 4.2	Outline of Other Candidates for Potential Inclusion
- Stress Testing the application and its servers
- Searching security holes
### 4.3 Outline of Test Exclusions
- Angular Framework
- Spring Boot Services
## 5.	Test Approach
### 5.1 Initital Test-Idea Catalogs and Other Reference Sources
n/a
### 5.2	Testing Techniques and Types
#### 5.2.1 Spring Boot Backend Testing (Unit)
|Technique Objective  	| The backend is to be tested directly via the existing interface. We will write a small test framework for this. |
|Technique 		| Most editing tools are tested with mocked data. There is an extra test user for this. |
|Oracles 		| The test user has all rights to perform all tests. |
|Required Tools 	| Java, JUnit |
|Success Criteria	| all tests pass, no unexpected behaviors, all possible cases and inputs are getting tested |
|Special Considerations	| - |
#### 5.2.2 Angular Frontend Testing (Cucumber)
|Technique Objective  	| The frontend is tested by simulating a web browser. This makes the tests very close to the user. |
|Technique 		| Nothing is mocked up, as all layers are to be checked for correctness. |
|Oracles 		| The user input, for example a valid username and password. |
|Required Tools 	| Java, Cucumber, Selenium |
|Success Criteria	| all tests pass, no unexpected behaviors, all possible cases and inputs are getting tested  |
|Special Considerations	| - |
#### 5.2.3 Business Cycle Testing
n/a
#### 5.2.4 User Interface Testing
Tested with Selenium
- [Angular Frontend Testing (Cucumber)](#5-2-2-angular-frontend-testing-\(Cucumber\))
#### 5.2.5 Performance Profiling 
n/a
#### 5.2.6 Load Testing
n/a
#### 5.2.7 Stress Testing
n/a
#### 5.2.8	Volume Testing
n/a
#### 5.2.9	Security and Access Control Testing
Login tests with Java Unit tests
- [Spring Boot Backend Testing (Unit)](#5-2-1-spring-boot-backend-testing-\(Unit\))
#### 5.2.10	Failover and Recovery Testing
n/a
#### 5.2.11	Configuration Testing
n/a
#### 5.2.12	Installation Testing
n/a
## 6.	Entry and Exit Criteria
### 6.1	Test Plan
#### 6.1.1	Test Plan Entry Criteria
Pushing new commits to Github will trigger the Jenkins CI/CD pipeline.
#### 6.1.2	Test Plan Exit Criteria
When all tests pass without throwing an exception.
#### 6.1.3 Suspension and Resumption Criteria
n/a
## 7.	Deliverables
### 7.1	Test Evaluation Summaries
The Jenkins pipeline provides the results via a web interface and reports the results to Github.
### 7.2	Reporting on Test Coverage
tbd
### 7.3	Perceived Quality Reports
Codacy checks the code and provides a metrics report.
Additional, we use the Eclipse Metrics plugin to keep track of the code quality.
### 7.4	Incident Logs and Change Requests
n/a
### 7.5	Smoke Test Suite and Supporting Test Scripts
n/a
### 7.6	Additional Work Products
#### 7.6.1	Detailed Test Results
Jenkins collects the logs of the tests and provides them clearly in the interface.
#### 7.6.2	Additional Automated Functional Test Scripts
n/a
#### 7.6.3	Test Guidelines
All code that is testable should be tested. Due to the technologies used, a target coverage in percent does not make sense. We will test all important components at our own discretion.
#### 7.6.4	Traceability Matrices
n/a
## 8.	Testing Workflow
Developers should execute tests locally before pushing source code. When pushing to branches, the tests are executed automatically.
## 9.	Environmental Needs
This section presents the non-human resources required for the Test Plan.
### 9.1	Base System Hardware
| Resource | Quantity                            |Name and Type |
| ----------- | -------------------------------------- |-----|
| Frontend Server | 1 | Linux Server |
| Backend Server | 1 | Linux Server |
| Database         | 1 | MariaDB (MySQL) |
### 9.2	Base Software Elements in the Test Environment
| Software Element Name | Version                            |Type and Other Notes|
| ----------- | -------------------------------------- |-----|
| Windows | 10 | Operating System |
| Chrome | 91 | Internet Browser |
| Firefox | 89 | Internet Browser |
| Java | 11 | Runtime Environment |
### 9.3	Productivity and Support Tools
|Tool Category or Type | Tool Brand Name                            |
| ----------- | -------------------------------------- |
| Code Hoster | Github |
| CI/CD Service | Jenkins |
| Metrics Tool | Codacy |
| Deployment Tool | Docker |
### 9.4	Test Environment Configurations
n/a 
## 10.	Responsibilities, Staffing, and Training Needs
### 10.1	People and Roles
| Role | Minimum Resources Recommended (number of full-time roles allocated)      |Specific Responsibilities or Comments |
| ----------- | -------------------------------------- |-----|
| Test Manager | 1 | Provides management oversight|
| Test Designer | 1 | Defines the technical approach to the implementation of the test effort.|
|Tester|1|Implements and executes the tests. |
|Test System Administrator|1|Ensures test environment and assets are managed and maintained.|
|Database Administrator, Database Manager|1|Ensures test data (database) environment and assets are managed and maintained.|
|Implementer|3|Implements and unit tests the test classes and test packages.|
### 10.2	Staffing and Training Needs
n/a
## 11.	Iteration Milestones
| Milestone | Planned Start Date | Actual Start Date | Planned End Date | Actual End Date |
|---|---|---|---|---|
| Have .feature Files | 27.10.2020 | 27.10.2020 | 31.12.2020 | 01.12.2020 |
| Have Unit Tests | 20.04.2021 | 20.04.2021 | 27.04.2021 | 27.04.2021 |
## 12.	Risks, Dependencies, Assumptions, and Constraints
[Risk Management](https://docs.google.com/spreadsheets/d/19gUf3bzLuj642SzhrBE9ir6mFPK2t47UzX7Xnn0cUHU/edit?usp=sharing)
## 13. Management Process and Procedures
n/a
