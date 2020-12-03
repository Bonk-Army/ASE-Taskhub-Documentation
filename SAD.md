# Software Architecture Document

# Table of Contents
- [Introduction](#1-introduction)
    - [Purpose](#11-purpose)
    - [Scope](#12-scope)
    - [Definitions, Acronyms and Abbreviations](#13-definitions-acronyms-and-abbreviations)
    - [References](#14-references)
    - [Overview](#15-overview)
- [Architectural Representation](#2-architectural-representation)
- [Architectural Goals and Constraints](#3-architectural-goals-and-constraints)
- [Use-Case View](#4-use-case-view)
- [Logical View](#5-logical-view)
    - [Overview](#51-overview)
    - [Architecturally Significant Design Packages](#52-architecturally-significant-design-packages)
- [Process View](#6-process-view)
- [Deployment View](#7-deployment-view)
- [Implementation View](#8-implementation-view)
- [Data View](#9-data-view)
- [Size and Performance](#10-size-and-performance)
- [Quality](#11-quality)

## 1. Introduction

### 1.1 Purpose
This document provides a comprehensive architectural overview of the system, using a number of different architectural views to depict different aspects of the system. It is intended to capture and convey the significant architectural decisions which have been made on the system.

### 1.2 Scope
This document describes the technical architecture of the TaskHub project, including the structure of classes, modules and dependencies.

### 1.3 Definitions, Acronyms and Abbreviations

| Abbrevation | Description                            |
| ----------- | -------------------------------------- |
| API         | Application programming interface      |
| REST        | Representational state transfer        |
| SRS         | Software Requirements Specification    |
| UC          | Use Case                               |
| VCS         | Version Control System                 |
| n/a         | not applicable                         |

### 1.4 References

| Title                                                                                                                               |     Date     | Publishing organization   |
| ------------------------------------------------------------------------------------------------------------------------------------|:------------:| ------------------------- |
| [TaskHub Blog](https://taskhub854228916.wordpress.com/)   	                                                                       	| 2020-12-03   | TaskHub Team              |
| [Repository on GitHub - Code ](https://github.com/Unk3wn/TaskHub---Codebase)	  	                                                  | 2020-12-03   | TaskHub Team              |
| [Repository on GitHub - Docu ](https://github.com/Unk3wn/TaskHub---Documentation)	                                                  | 2020-12-03   | TaskHub Team              |
| [UC Assign Student](https://github.com/Unk3wn/TaskHub---Documentation/blob/master/UC/UseCases/AssignStudent/AssignStudent.md)      | 2020-12-03   | TaskHub Team              |
| [UC Assign Teacher](https://github.com/Unk3wn/TaskHub---Documentation/blob/master/UC/UseCases/AssignTeacher/AssignTeacher.md)      | 2020-12-03   | TaskHub Team              |
| [UC CreateAClass](https://github.com/Unk3wn/TaskHub---Documentation/blob/master/UC/UseCases/CreateAClass/CreateAClass.md)        | 2020-12-03   | TaskHub Team              |
| [UC CreateTask](https://github.com/Unk3wn/TaskHub---Documentation/blob/master/UC/UseCases/CreateTask/CreateTask.md)            | 2020-12-03   | TaskHub Team              |
| [UC EditSolution](https://github.com/Unk3wn/TaskHub---Documentation/blob/master/UC/UseCases/EditSolution/EditSolution.md)        | 2020-12-03   | TaskHub Team              |
| [SRS](https://github.com/Unk3wn/TaskHub---Documentation/blob/master/README.md)                                                      | 2020-12-03   | TaskHub Team              |

### 1.5 Overview
This document contains the Architectural Representation, Goals and Constraints as well
as the Logical, Deployment, Implementation and Data Views.

## 2. Architectural Representation
![Architecture](https://github.com/Unk3wn/TaskHub---Documentation/blob/master/src/stack.png?raw=true)

## 3. Architectural Goals and Constraints
We are dividing the Frontend,Backend and Database. That we can swap each component very easily.

### Database
For the Database we use [Postgre](https://www.postgresql.org/), because we used that in the Past and are familiar with it.

### Backend
For the Backend we use a [Node.js](https://nodejs.org/en/) Server with [ExpressJS]() and [Sequelize](https://sequelize.org/) to generate an REST API.

###Frontend
For the Frontend we use [Angular](https://angular.io/) to build our Webapp and connect to the REST API to get our Data.

## 4. Use-Case View
![Use Case](https://github.com/Unk3wn/TaskHub---Documentation/blob/master/UML/TaskHubUML.png?raw=true)

## 5. Logical View
TODO

## 6. Process View
TODO

## 7. Deployment View
![Deployment View](https://github.com/Unk3wn/TaskHub---Documentation/blob/master/src/DeploymentView.png?raw=true)

## 9. Data View
![Database View](https://github.com/Unk3wn/TaskHub---Documentation/blob/master/src/database.png?raw=true))

## 10. Size and Performance
n/a

## 11. Quality/Metrics
We are planning to use Jenkins as an continuous integration tool to ensure a high quality of our development process. Whenever there is a new commit to a pull request or the master branch it automatically builds the project and executes all tests. The Jenkins build result will be displayed beside each commit on Github.
* Reducing the amount of Bugs/Issues/Code Smells raised by SonarQube.
