
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
This document describes the used tests (Unit tests and End-to-End tests).
### 1.3	Intended Audience
This document is meant for internal use primarily.
### 1.4	Document Terminology and Acronyms
- **SRS**	Software Requirements Specification
-  **UCD**	Use Case Diagram
- **n/a**	not applicable
- **tbd**	to be determined
### 1.5	 References
| Reference        | 
| ------------- |
| [SRS](https://github.com/SimpleSurveyProject/SimpleSurvey-Documentation/blob/main/Software%20Requirements%20Specification.md) |
| [SAD](https://github.com/SimpleSurveyProject/SimpleSurvey-Documentation/blob/main/Software%20Architecture%20Document.md) | 
| [UCD](https://ucd.simplesurvey.de) |

  
## 2.	Evaluation Mission and Test Motivation
### 2.1	Background
By testing source code, we ensure our application to run smoothly. The goal is to make sure, that our application does not run into any unexpected errors.
### 2.2	Evaluation Mission
The mission of this test plan is to prevent errors in production and ensure an outstanding software quality.
### 2.3	Test Motivators
Our testing is motivated by 
- quality risks 
- technical risks, 
- use cases 
- functional requirements
## 3.	Target Test Items
The listing below identifies those test items (software, hardware, and supporting product elements) that have been identified as targets for testing. 
This list represents what items will be tested. 
Items for Testing:
- SpringBoot Backend
- Angular Frontend
## 4.	Outline of Planned Tests
### 4.1	Outline of Test Inclusions
Testing the backend with unit tests. 
End2End testing the frontend application.
### 4.2	Outline of Other Candidates for Potential Inclusion
Stress Testing the application and its servers.
Findung security holes.
### 4.3 Outline of Test Exclusions
n/a
## 5.	Test Approach
### 5.1 Initital Test-Idea Catalogs and Other Reference Sources
**n/a**
### 5.2	Testing Techniques and Types
#### 5.2.1 SpringBoot Backend Testing
tbd
|| |
|---|---|
|Technique Objective  	|  |
|Technique 		|  |
|Oracles 		|  |
|Required Tools 	|  |
|Success Criteria	|  |
|Special Considerations	|  |
#### 5.2.2 Angular Frontend Testing
tbd
|| |
|---|---|
|Technique Objective  	|  |
|Technique 		|  |
|Oracles 		|  |
|Required Tools 	|  |
|Success Criteria	|  |
|Special Considerations	|  |
#### 5.2.3 Business Cycle Testing
**n/a**
#### 5.2.4 User Interface Testing
**n/a**
#### 5.2.5 Performance Profiling 
**n/a**
#### 5.2.6 Load Testing
**n/a**
#### 5.2.7 Stress Testing
**n/a**
#### 5.2.8	Volume Testing
**n/a**
#### 5.2.9	Security and Access Control Testing
**n/a**
#### 5.2.10	Failover and Recovery Testing
**n/a**
#### 5.2.11	Configuration Testing
**n/a**
#### 5.2.12	Installation Testing
**n/a**
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
The Jenkins pipeline provides the results via a web interface.
### 7.2	Reporting on Test Coverage
tbd
### 7.3	Perceived Quality Reports
n/a
### 7.4	Incident Logs and Change Requests
n/a
### 7.5	Smoke Test Suite and Supporting Test Scripts
n/a
### 7.6	Additional Work Products
#### 7.6.1	Detailed Test Results
tbd
#### 7.6.2	Additional Automated Functional Test Scripts
**n/a**
#### 7.6.3	Test Guidelines
tbd
#### 7.6.4	Traceability Matrices
**n/a**
## 8.	Testing Workflow
Developers should execute tests locally before pushing source code. When pushing to branches, the tests are executed automatically.
## 9.	Environmental Needs
This section presents the non-human resources required for the Test Plan.
### 9.1	Base System Hardware
tbd
### 9.2	Base Software Elements in the Test Environment
tbd
### 9.3	Productivity and Support Tools
tbd
### 9.4	Test Environment Configurations
n/a 
## 10.	Responsibilities, Staffing, and Training Needs
### 10.1	People and Roles
tbd
### 10.2	Staffing and Training Needs
**n/a**
## 11.	Iteration Milestones
| Milestone | Planned Start Date | Actual Start Date | Planned End Date | Actual End Date |
|---|---|---|---|---|
| Have Unit Tests | 27.04.2021 | 27.04.2021 | 03.05.2021 | - |
| 30% coverage | 27.04.2021 | 27.04.2021   | 27.05.2021   | - |
| Tests integrated in CI | 04.05.2021 | 04.05.2021 | 17.05.2021 | - |
## 12.	Risks, Dependencies, Assumptions, and Constraints
| Risk | Mitigation Strategy	| Contingency (Risk is realized) |
|---|---|---|
| Unexpected failures in production | Cover as much scenarios as possible, Logging | Look into logs and fix the bug, Roll back version if necessary |
## 13. Management Process and Procedures
**n/a**
