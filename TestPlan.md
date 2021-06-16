# Test plan

## 1.	Introduction
### 1.1	Purpose
The purpose of the Iteration Test Plan is to gather all of the information necessary to plan and control the test effort for a given iteration. 
It describes the approach to testing the software. This Test Plan for TaskHUB supports the following objectives:

- Identifies the items that should be targeted by the tests.
- Identifies the motivation for and ideas behind the test areas to be covered.
- Outlines the testing approach that will be used.
- Identifies the required resources and provides an estimate of the test efforts.

### 1.2	Scope
This document describes the functionality and usability of tests.

### 1.3	Intended Audience
This test plan is intended to help everyone that either wants to use our code and / or tests by giving a clearer structure about our testing strategies.

### 1.4	Document Terminology and Acronyms
- **SRS**	Software Requirements Specification
- **n/a**	not applicable
- **tbd**	to be determined

### 1.5	 References
| Reference        | 
| ------------- |
| [Blog](https://taskhub854228916.wordpress.com/) | 
| [GitHub Repository](https://github.com/Unk3wn/TaskHub---Codebase) | 
| [SRS](https://github.com/Unk3wn/TaskHub---Documentation/blob/master/README.md)|
| [SAD](https://github.com/Unk3wn/TaskHub---Documentation/blob/master/SAD.md)|

## 2.	Evaluation Mission and Test Motivation
The tests will mainly be written to ensure that any changes in the future don't break the application. As part of the tests will also be run as a part of our CI/CD system, any changes that cause a test to fail will not get merged until the issue is fixed.
### 2.1	Background
Testing serves to ensure that the written code does what it is intended to do. It also prevents future code changes to break existing functionality unnoticed. In the context of integration it can also prevent broken software states to be merged into secured VC branches.
### 2.2	Evaluation Mission
- find as many bugs as possible
- find important problems
- advise about product quality
- avoid merging breaking changes
### 2.3	Test Motivators
Our testing is motivated by 
- quality risks 
- technical risks 
- functional requirements

## 3.	Target Test Items
The listing below identifies those test items software, hardware, and supporting product elements that have been identified as targets for testing. As we don't have the infrastructure to perform hardware and operating system tests, our tests will focus on the code we write.

## 4.	Outline of Planned Tests
### 4.1	Outline of Test Inclusions
||type of tests|
|---|---|
|Frontend: Angular|UI testing of views/fragments|
||Unit testing|
|Backend: Node and Express| API testing |

The tests themself will not be tested and will not account into code coverage.

### 4.2	Outline of Other Candidates for Potential Inclusion
n/a
### 4.3 Outline of Test Exclusions
Hardware and operating systems will not be tested as we don't have the infrastructure to do this.

## 5.	Test Approach
### 5.1	Testing Techniques and Types
n/a
#### 5.1.1	Function and Database Integrity Testing
||Description|
|---|---|
|Technique Objective|Every endpoint should be accessible and return the correct data if the correct input parameters are supplied|
|Technique|The endpoints are accessed via postman and the answers from the server are checked for correctness|
|Oracles|The HTTP status code and the body type of the response are checked|
|Required Tools|Postman|
|Success Criteria|All endpoints return the expected data|
|Special Consideration|-|

#### 5.1.2	Unit Testing
||Description|
|---|---|
|Technique Objective|Every request to the backend shall be done correctly. Possible exceptions are caught correctly.|
|Technique|Unit testing the endpoints|
|Oracles|user enter valid data, for example a valid username and a valid password|
|Required Tools|Jasmine, Karma|
|Success Criteria|successful scenarios, all tests will pass|
|Special Consideration|-|

#### 5.1.3	Business Cycle Testing
n/a

#### 5.1.4	User Interface Testing (Cucumber)
||Description|
|---|---|
|Technique Objective  	| Every possible UI scenario should work flawless  |
|Technique 		| Cucumber testing by integrating a special JS plugin into IntelliJ and running earlier specified .feature files  |
|Oracles 		| The site looks as expected after performing a scenario |
|Required Tools 	| Cucumber JS plugin |
|Success Criteria	| All tests passed |
|Special Considerations	|     -          |

#### 5.1.5	Performance Profiling 
n/a

#### 5.1.6	Load Testing
n/a

#### 5.1.7	Stress Testing
n/a
 
#### 5.1.8	Volume Testing
n/a

#### 5.1.9	Security and Access Control Testing
n/a

#### 5.1.10	Failover and Recovery Testing
n/a

#### 5.1.11	Configuration Testing
n/a

#### 5.1.12	Installation Testing

## 6.	Entry and Exit Criteria
### 6.1	Test Plan
**n/a**
#### 6.1.1	Test Plan Entry Criteria
**n/a**
#### 6.1.2	Test Plan Exit Criteria
All tests pass successfully.
#### 6.1.3 Suspension and Resumption Criteria
n/a

## 7.	Deliverables
### 7.1	Test Evaluation Summaries
n/a

### 7.2	Reporting on Test Coverage
Karma creates a detailed code coverage report every time the frontend is tested. It provides overall coverage which is also reflected in our GitHub README as well as detailed coverage per file.

### 7.3	Perceived Quality Reports
n/a

### 7.4	Incident Logs and Change Requests
Incidents and Change Requests are handled via our project management tool YouTrack.

### 7.5	Smoke Test Suite and Supporting Test Scripts
n/a

### 7.6	Additional Work Products
n/a

#### 7.6.1	Detailed Test Results
n/a

#### 7.6.2	Additional Automated Functional Test Scripts
- [API Tests](https://github.com/Unk3wn/TaskHub---Codebase/blob/master/Backend/0_Postman/TaskHub.postman_collection.json)
- [Unit Tests](https://github.com/Unk3wn/TaskHub---Codebase/tree/master/Frontend/src) (in each component)
- [Functional Tests](https://github.com/Unk3wn/TaskHub---Codebase/tree/master/CucumberTests/src/test)

#### 7.6.3	Test Guidelines
n/a

#### 7.6.4	Traceability Matrices
n/a

## 8.	Testing Workflow
Tests should be written and (if required) adjusted alongside the development.

## 9.	Environmental Needs
### 9.1	Base System Hardware
n/a

### 9.2	Base Software Elements in the Test Environment
The following base software elements are required in the test environment for this Test Plan.

|---|---|
|Software Element Name	|Type and Other Notes|
|IntelliJ|	Test Runner / IDE|
|Jasime / Karma|	Unit testing library|
|Cucumber	|human readable test definitions|

### 9.3	Productivity and Support Tools
The following tools will be employed to support the test process for this Test Plan.
|Tool |Category or Type|	Tool Brand Name	|Vendor or In-house|	Version|
|Test Management|	Karma.js	|Open-Source|	6.3.2|
|Test Coverage Monitor or Profiler|	Karma.js	|Open-Source	|6.3.2|
|Project Management|	YouTrack	|JetBrains|	N/A|
|DBMS tools	|IntelliJ|	JetBrains|2021.1|

### 9.4	Test Environment Configurations
n/a

## 10.	Responsibilities, Staffing, and Training Needs
### 10.1	People and Roles
This table shows the staffing assumptions for the test effort.
|Role|Minimum Resources Recommended(number of full-time roles allocated)|Specific Responsibilities or Comments|
|---|---|---|
|Test Manager|1|Provides management oversight.  Responsibilities include:  planning and logistics  agree mission  identify motivators acquire appropriate resources present management reporting advocate the interests of testevaluate effectiveness of test effort|
|Test Designer|1|Defines the technical approach to the implementation of the test effort.  Responsibilities include: define test approach define test automation architecture verify test techniques define testability elements structure test implementation|
|Tester|1|Implements and executes the tests. Responsibilities include: implement tests and test suites execute test suites log results analyze and recover from test failures document incidents|
|Test System Administrator|1|Ensures test environment and assets are managed and maintained. Responsibilities include: 	administer test management system install and support access to, and recovery of, test environment configurations and test labs|
|Implementer|1|Implements and unit tests the test classes and test packages. Responsibilities include: creates the test components required to support testability requirements as defined by the designer|

### 10.2	Staffing and Training Needs
n/a
## 11.	Iteration Milestones

| Milestone | Planned Start Date | Actual Start Date | Planned End Date | Actual End Date |
|---|---|---|---|---|
| Have Unit Tests | 29.04.2021 | 05.05.2021 | 15.06.2021 | 04.06.2021 |
| Have Cucumber Tests | 29.10.2021 | 30.10.2021 | 15.06.2021 | 16.06.2021 |
| Have API Tests | 29.04.2021 | 03.05.2021 | 15.06.2021 | 26.05.2021 |
| 50% coverage | 29.04.2021 | 05.05.2021 | 15.06.2021 | 16.06.2021 |
| Tests integrated in CI | - | - | - | - |


## 12.	Risks, Dependencies, Assumptions, and Constraints
| Risk | Mitigation Strategy	| Contingency (Risk is realized) |
|---|---|---|
| Testing scenario is not <br/>covered | Aim for high coverage | Add scenario | 
## 13. Management Process and Procedures
n/a
