# SimpleSurvey - Software Requirements Specification

## Table of contents
- [1. Introduction](#1-introduction)
  * [1.1 Purpose](#11-purpose)
  * [1.2 Scope](#12-scope)
  * [1.3 Definitions, Acronyms and Abbreviations](#13-definitions--acronyms-and-abbreviations)
  * [1.4 References](#14-references)
  * [1.5 Overview](#15-overview)
- [2. Overall Description](#2-overall-description)
- [3. Specific Requirements](#3-specific-requirements)
  * [3.1 Functionality](#31-functionality)
  * [3.2 Usability](#32-usability)
  * [3.3 Reliability](#33-reliability)
  * [3.4 Performance](#34-performance)
  * [3.5 Supportability](#35-supportability)
  * [3.6 Design Constraints](#36-design-constraints)
  * [3.7 Online User Documentation and Help System Requirements](#37-on-line-user-documentation-and-help-system-requirements)
  * [3.8 Purchased Components](#38-purchased-components)
  * [3.9 Interfaces](#39-interfaces)
  * [3.10 Licensing Requirements](#310-licensing-requirements)
  * [3.11 Legal, Copyright, and Other Notices](#311-legal--copyright--and-other-notices)
  * [3.12 Applicable Standards](#312-applicable-standards)
- [4. Supporting Information](#4-supporting-information)


## 1. Introduction
### 1.1 Purpose
This Software Requirements Specification (SRS) describes all specifications for the application "SimpleSurvey". It includes an overview about this project and its vision, detailed information about the planned features and boundary conditions of the development process.

### 1.2 Scope
The following parts are planned:
* Dashboard
* Account settings
* Survey-System
	* create
	* edit
	* share
	* fill out
	* evaluate

### 1.3 Definitions, Acronyms and Abbreviations
| Abbrevation | Explanation                            |
| ----------- | -------------------------------------- |
| SRS         | Software Requirements Specification    |
| UC          | Use Case                               |
| n/a         | not applicable                         |
| tbd         | to be determined                       |
| UCD         | Use Case Diagram                       |
| FAQ         | Frequently asked Questions             |

### 1.4 References
| Title                                                              | Date       |
| -------------------------------------------------------------------|:----------:|
| [SimpleSurvey Blog](https://simplesurveyproject.wordpress.com)     | 13.10.2020 |
| [GitHub](https://github.com/SimpleSurveyProject)                   | 13.10.2020 |
| [WebApp](https://simplesurvey.de)                                  | 13.10.2020 |


### 1.5 Overview
The following chapter provides an overview of this project with vision and Overall Use Case Diagram. The third chapter (Requirements Specification) delivers more details about the specific requirements in terms of functionality, usability and design parameters. Finally there is a chapter with supporting information.
    
## 2. Overall Description
SimpleSurvey becomes a web application. The app should also be able to be used without a login.
Actors of this App can be guests, users, creators or administrators.
Users can create surveys and share them with the world. They can evaluate the results and draw conclusions on the platform.

## 3. Specific Requirements
### 3.1 Functionality
This section will explain the different use cases, you could see in the Use Case Diagram, and their functionality.  

![UCD](https://screen.simonlabs.de/img.php?id=2I0cisf)
- Green: Planned till end of december
- Orange: Planned till end of june
- White: Additional features

#### 3.1.1 Create survey
Every logged in user is able to create new surveys, which he can also share and evaluate.
[CLICK HERE](https://github.com/SimpleSurveyProject/SimpleSurvey-Documentation/blob/main/use-cases/use-case-createSurvey.md)  

#### 3.1.2 Fill out survey
Every logged in user is able to fill out exisiting surveys of other users. He needs to enter the unique ID of the survey he wants to answer.
[CLICK HERE](https://github.com/SimpleSurveyProject/SimpleSurvey-Documentation/blob/main/use-cases/use-case-fillsOutSurvey.md)  

#### 3.1.3 Edit survey
The users are able to edit their own surveys.
[CLICK HERE](https://github.com/SimpleSurveyProject/SimpleSurvey-Documentation/blob/main/use-cases/use-case-editSurvey.md)  

#### 3.1.4 Share Survey
The users are able to generate links for others to instantly access an exisiting survey.
[CLICK HERE](https://github.com/SimpleSurveyProject/SimpleSurvey-Documentation/blob/main/use-cases/use-case-sharesSurvey.md)  

#### 3.1.5 Evaluate Survey
The user has a dashboard which allows him to not only see the answers of the survey, but also shows general information about the questions (most skipped question, overall participants...)
[CLICK HERE](https://github.com/SimpleSurveyProject/SimpleSurvey-Documentation/blob/main/use-cases/use-case-evaluateSurvey.md)  

### 3.2 Usability
We plan on designing the user interface as intuitive and self-explanatory as possible to make the user feel as comfortable as possible using the app. Though an FAQ document will be available, it should not be necessary to use it.

#### 3.2.1 No training time needed
Our goal is that a user opens the Web-Application and is able to use all features without any explanation or help.

#### 3.2.2 Familiar Feeling
We want to implement a Web-Application with familiar designs and functions. This way the user is able to interact in familiar ways with the app without having to get to know new interfaces.

### 3.3 Reliability
#### 3.3.1 Availability
The server shall be available 95% of the time. This also means we have to figure out the "rush hours" of our application because the downtime of the server is only tolerable when as few as possible Users want to use the application.

#### 3.3.2 Defect Rate
Our goal is that we have no loss of any data. This is important so that the application can carry on, even after a downtime of the server.

### 3.4 Performance
#### 3.4.1 Capacity
The system should be able to manage thousands of requests. Also it should be possible to register as many users as necessary.

#### 3.4.2 Storage
We are aiming to keep the needed storage as small as possible.

#### 3.4.3 Performance / Response time
To provide the best  performance we aim to keep the response time as low as possible. This will make the user experience much better.

### 3.5 Supportability
#### 3.5.1 Coding Standards
We are going to write the code by using all of the most common clean code standards. For example we will name our variables and methods by their functionalities. This will keep the code easy to read by everyone and make further development much easier.

#### 3.5.2 Testing Strategy
The application will have a high test coverage and all important functionalities and edge cases should be tested. Further mistakes in the implementation will be discovered instantly and it will be easy to locate the error.

### 3.6 Design Constraints
The technology we use is:

Backend (Docker):  
* Spring Boot  
* MySQL Database (MariaDB)  

Frontend (Docker):  
* Angular  

IDE:  
* Microsoft Visual Studio Code  
* Eclipse  

Project Management:  
* YouTrack  
* GitHub  

Deployment:  
* Jenkins  

Testing:  
* Cucumber (Selenium)  


We are trying to provide a modern and easy to handle design for the UI as well as for the architecture of our application. To achieve that the functionalities will be kept as modular as possible.

Because we are programming a Web-Application we chose JavaScript  as our programming language. Also we are using the common MVC-architecture to keep the front end and back end separated. For a clean front end structure we use MVC.
To make the communication between the two parts easy, we will implement a RESTful-API between them which will provide the data in JSON-Format.
The supported Platforms will be:
* all modern Browsers

### 3.7 On-line User Documentation and Help System Requirements
The usage of the application should be as intuitive as possible so it won't need any further documentation. If the user needs some help we will implement a "Help"-Button which includes a FAQ and a formular to contact the development team.

### 3.8 Purchased Components
We have bought a domain for the web application and a Linux Server, where the applications run.

### 3.9 Interfaces
#### 3.9.1 User Interfaces
tbd

#### 3.9.2 Hardware Interfaces
We use a Linux server in a data center.

#### 3.9.3 Software Interfaces
Since it is a web application, it will run in any modern browser. The backend will be installed on a Linux server.

#### 3.9.4 Communication Interfaces
The frontend will communicate with the backend through the https protocol.

### 3.10 Licensing Requirements
### 3.11 Legal, Copyright, and Other Notices
Our logo is licensed to the SimpleSurvey Team and is only allowed to use for the application. Also, we do not take responsibilty for any incorrect data or errors in the application.

### 3.12 Applicable Standards
We try to follow all standards and use modern techniques.


## 4. Supporting Information
For further questions you can contact us on all platforms.
The Team Members are:
* Patrick Braje
* Simon Fischer
* (Dominik Seiler)
