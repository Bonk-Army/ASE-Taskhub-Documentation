Project - TaskHub | Software Requirements Specification
======
Version <1.0>
======

- [#Revision History](#-revision-history)
- [1. Introduction](#1-introduction)
  * [1.1 Purpose](#11-purpose)
  * [1.2 Scope](#12-scope)
  * [1.3 Definitions, Acronyms and Abbreviations](#13-definitions--acronyms-and-abbreviations)
  * [1.4 References](#14-references)
  * [1.5 Overview](#15-overview)
- [2. Overall Description](#2-overall-description)
  * [2.1 Vision](#21-vision)
  * [2.2 Use Case Diagram](#22-use-case-diagram)
  * [2.3 Technology Stack](#23-technology-stack)
- [3. Specific Requirements](#3-specific-requirements)
  * [3.1 Functionality](#31-functionality)
    + [3.1.1 User Registration](#311-user-registration)
    + [3.1.2 Classes](#312-classes)
    + [3.1.3 Teams](#313-teams)
    + [3.1.4 Colloborative Work](#314-colloborative-work)
  * [3.2 Usability](#32-usability)
    + [3.2.1 Easy to understand](#321-easy-to-understand)
    + [3.2.2 No Overloaded features](#322-no-overloaded-features)
  * [3.3 Reliability](#33-reliability)
    + [3.3.1 Backup feature of Solutions](#331-backup-feature-of-solutions)
  * [3.4 Perfomance](#34-perfomance)
    + [3.4.1 Speed](#341-speed)
  * [3.5 Supportability](#35-supportability)
    + [3.5.1 Supportability Requirement One](#351-supportability-requirement-one)
  * [3.6 Design Constraints](#36-design-constraints)
    + [3.6.1 Lightway](#361-lightway)
    + [3.6.1 Minimalistic](#361-minimalistic)
  * [3.7 On-line User Documentation and Help System Requirements](#37-on-line-user-documentation-and-help-system-requirements)
  * [3.8 Purchased Components](#38-purchased-components)
  * [3.9 Interfaces](#39-interfaces)
    + [3.9.1 User Interfaces](#391-user-interfaces)
    + [3.9.2 Hardware Interfaces](#392-hardware-interfaces)
    + [3.9.3 Software Interfaces](#393-software-interfaces)
    + [3.9.4 Communications Interfaces](#394-communications-interfaces)
  * [3.10 Licensing Requirements](#310-licensing-requirements)
  * [3.11 Legal, Copyright, and Other Notices](#311-legal--copyright--and-other-notices)
  * [3.12 Applicable Standards](#312-applicable-standards)
- [4. Supporting Information](#4-supporting-information)


#Revision History
-----
|    Date    | Version |    Description    | Author |
|------------|---------|-------------------|--------|
| 15.10.2020 |   1.0   |  initial Release  |  Nico  |

## 1. Introduction

### 1.1 Purpose
This Software Requirements Specification (SRS) describes all specifications for the application "TaskHub". It includes an overview about this project and its vision, detailed information about the planned features and boundary conditions of the development process.

### 1.2 Scope
The project is going to be realized as an Web-Application.
to be determined (tbd)

### 1.3 Definitions, Acronyms and Abbreviations

|     Abbrevation      |                            Explanation                                   |
| -------------------- | ------------------------------------------------------------------------ |
| SRS                  | Software Requirements Specification                                      |
| n/a                  | not applicable                                                           |
| tbd                  | to be determined                                                         |
| not applicable (n/a) | Items that are not relevant have been maintained but contain the comment |

### 1.4 References
| Title                                                                                    | Date       | Publishing organization   |
| -----------------------------------------------------------------------------------------|:----------:| ------------------------- |
| [TaskHub Blog](https://taskhub854228916.wordpress.com/)                                  | 15.10.2020 | TaskHub Team              |
| [GitHub Repo for Code](https://github.com/Unk3wn/TaskHub---Documentation/)               | 15.10.2020 | TaskHub Team              |
| [GitHub Repo for Documentation](https://github.com/Unk3wn/TaskHub---Documentation/)      | 15.10.2020 | TaskHub Team              |


### 1.5 Overview
The following chapter provides an overview of this project with vision and Overall Use Case Diagram. The third chapter (Requirements Specification) delivers more details about the specific requirements in terms of functionality, usability and design parameters. Finally there is a chapter with supporting information.

## 2. Overall Description
[This section of the SRS should describe the general factors that affect the product and its requirements.  This section does not state specific requirements.  
Instead, it provides a background for those requirements, which are defined in detail in Section 3, and makes them easier to understand. Include such items as:
 - product perspective
 - product functions
 - user characteristics
 - constraints
 - assumptions and dependencies
 - requirements subsets]

### 2.1 Vision
The main functions of our webapp are the collaborative features. In our vision many users can write simultaneously into shared documents to solve problems or tasks as a living group. As a team member you can write your discoveries about the task or your finished solution approach into this document to share with your team.

We got inspired by an CTF Tool, which many teams use in their workflow. In this tool you can create tasks with notes on specific topics. Also you can set deadlines or assign a specific member, an expert, to a task.

### 2.2 Use Case Diagram
[<img src="https://raw.githubusercontent.com/Unk3wn/TaskHub---Documentation/main/UML/TaskHubUML.png">](UML)

### 2.3 Technology Stack
- L inux
- A pache
- M ySql
- A ngular


## 3. Specific Requirements


### 3.1 Functionality
This section will explain the different use cases, you could see in the Use Case Diagram, and their functionality.
Until December we plan to implement: 
- User Registration
- User Login
- Class Functions
- Team Functions
Until June, we want to implement:
- Colloborative Work
- Grading
- Notifications

#### 3.1.1 Create a Class
The Use Case "Create a Class" describes how an admin can create a new class.
[Link to our UC](./UC/UCD/AddUserToClass/UCS_CreateClass.md)

#### 3.1.2. Assign Teacher
[Link to our UC](./UC/UCD/AddUserToClass/UCS_AssignTeacher.md)

#### 3.1.3. Add User to Class
[Link to our UC](./UC/UCD/AddUserToClass/UCS_AddUserToClass.md)

#### 3.1.4. Create new Task
[Link to our UC](./UC/UCD/AddUserToClass/UCS_CreateNewTask.md)

#### 3.1.5. Edit Solution
[Link to our UC](./UC/UCD/AddUserToClass/UCS_EditSolution.md)

### 3.2 Usability
We want to create an lightway easy to use Webapp for working together colloborative.

#### 3.2.1 Easy to understand
An easy to understand overlay with all necessary informations and functions

#### 3.2.2 No Overloaded features
We want to stay in an lightway app. Not many function noone ever will use.

### 3.3 Reliability
The webapp should be online at any time.

#### 3.3.1 Backup feature of Solutions
Backup the Solutions on a private space, to negate the possibility of Data loss

### 3.4 Perfomance
Should be quite quick, noone likes long loading apps

#### 3.4.1 Speed
Qick Loading Speed

### 3.5 Supportability
to be determined (tbd)

#### 3.5.1 Supportability Requirement One
[The requirement description goes here.]

### 3.6 Design Constraints
Lightway, minimalistic Design

#### 3.6.1 Lightway
Only frequently used features get included. Not to much functions!

#### 3.6.1 Minimalistic
Easy to use and minimimalistic interface without many graphics etc.

### 3.7 On-line User Documentation and Help System Requirements
Documentation gets published on the Mentioned Repo on Point 1.4. But we also want to comment the Code to get an easy access for everyone, who is interested in our Project!

### 3.8 Purchased Components
n/a

### 3.9 Interfaces
to be determined (tbd)

#### 3.9.1 User Interfaces
We want to interact with the user in an Webapp.

#### 3.9.2 Hardware Interfaces
n/a

#### 3.9.3 Software Interfaces
We want to use RestAPI's for the most Part to connect the Frontend to the Backend

#### 3.9.4 Communications Interfaces
n/a

### 3.10 Licensing Requirements
to be determined (tbd)

### 3.11 Legal, Copyright, and Other Notices
The logo is licensed to the TaskHub Team and is only allowed to use for the application. We do not take responsibilty for any incorrect data or errors in the application.

### 3.12 Applicable Standards
The development will follow the common clean code standards and naming conventions. Also we will create a definition of d which will be added here as soon as its complete.

## 4. Supporting Information
For any further information you can contact the TaskHub Team or check our (TaskHub Blog)[https://taskhub854228916.wordpress.com/]. The Team Members are:
- Nico
- Kristin
- Danny
