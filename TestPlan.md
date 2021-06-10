# Test plan

## 1.	Introduction
### 1.1	Purpose
The purpose of the Iteration Test Plan is to gather all of the information necessary to plan and control the test effort for a given iteration. 
It describes the approach to testing the software.

### 1.2	Scope
This document describes the used tests.

### 1.3	Intended Audience
n/a

### 1.4	Document Terminology and Acronyms
- **SRS**	Software Requirements Specification
- **n/a**	not applicable
- **tbd**	to be determined

### 1.5	 References
| Reference        | 
| ------------- |
| [Blog](https://taskhub854228916.wordpress.com/) | 
| [SRS](https://github.com/Unk3wn/TaskHub---Documentation/blob/master/README.md)|
| [SAD](https://github.com/Unk3wn/TaskHub---Documentation/blob/master/SAD.md)|

## 2.	Evaluation Mission and Test Motivation
### 2.1	Background
By testing our project, we try to ensure that feature changes to our source code don't break functionality.
### 2.2	Evaluation Mission
n/a
### 2.3	Test Motivators
Our testing is motivated by 
- quality risks 
- technical risks 
- functional requirements

## 3.	Target Test Items

## 4.	Outline of Planned Tests
### 4.1	Outline of Test Inclusions
n/a
### 4.2	Outline of Other Candidates for Potential Inclusion
n/a
### 4.3 Outline of Test Exclusions
n/a

## 5.	Test Approach
### 5.1	Testing Techniques and Types
n/a
#### 5.1.1	Function and Database Integrity Testing
n/a
#### 5.1.2	Unit Testing
|||
|---|---|
|Technique Objective|Every request to the backend shall be done correctly. Possible exceptions are caught correctly.|
|Technique|Unit testing the endpoints|
|Oracles|user enter valid data, for example a valid username and a valid password|
|Required Tools|Jasmine|
|Success Criteria|successful scenarios, all tests will pass|
|Special Consideration|-|

#### 5.1.3	Business Cycle Testing
n/a

#### 5.1.4	User Interface Testing (Cucumber)
|| |
|---|---|
|Technique Objective  	| Every possible UI scenario should work flawless  |
|Technique 		| Cucumber testing by integrating a special JS plugin into IntelliJ and running earlier specified .feature files  |
|Oracles 		| The site looks as expected after performing a scenario |
|Required Tools 	| Cucumber JS plugin |
|Success Criteria	| All tests passed |
|Special Considerations	|     -          |
|| |

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
tbd

### 7.3	Perceived Quality Reports
n/a

### 7.4	Incident Logs and Change Requests
n/a

### 7.5	Smoke Test Suite and Supporting Test Scripts
n/a

### 7.6	Additional Work Products
n/a

#### 7.6.1	Detailed Test Results
n/a

#### 7.6.2	Additional Automated Functional Test Scripts
n/a

#### 7.6.3	Test Guidelines
n/a

#### 7.6.4	Traceability Matrices
n/a

## 8.	Testing Workflow

## 9.	Environmental Needs
### 9.1	Base System Hardware
n/a

### 9.2	Base Software Elements in the Test Environment
n/a

### 9.3	Productivity and Support Tools
n/a

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
| Have Cucumber Tests | 29.10.2021 | 30.10.2021 | 15.06.2021 | tbd |
| Have API Tests | 29.04.2021 | 03.05.2021 | 15.06.2021 | 26.05.2021 |
| 5% coverage | 29.10.2021 |  | 15.06.2021 |  |
| Tests integrated in CI | - | - | - | - |


## 12.	Risks, Dependencies, Assumptions, and Constraints
| Risk | Mitigation Strategy	| Contingency (Risk is realized) |
|---|---|---|
| Testing scenario is not <br/>covered | Aim for high coverage | Add scenario | 
## 13. Management Process and Procedures
n/a
