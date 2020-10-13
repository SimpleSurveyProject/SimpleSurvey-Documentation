# Common Playground - Software Requirements Specification

## Table of contents
- [Table of contents](#table-of-contents)
- [Introduction](#1-introduction)
    - [Purpose](#11-purpose)
    - [Scope](#12-scope)
    - [Definitions, Acronyms and Abbreviations](#13-definitions-acronyms-and-abbreviations)
    - [References](#14-references)
    - [Overview](#15-overview)
- [Overall Description](#2-overall-description)
    - [Vision](#21-vision)
    - [Use Case Diagram](#22-use-case-diagram)
    - [Technology Stack](#23-technology-stack)
- [Specific Requirements](#3-specific-requirements)
    - [Functionality](#31-functionality)
    - [Usability](#32-usability)
    - [Reliability](#33-reliability)
    - [Performance](#34-performance)
    - [Supportability](#35-supportability)
    - [Design Constraints](#36-design-constraints)
    - [Online User Documentation and Help System Requirements](#37-on-line-user-documentation-and-help-system-requirements)
    - [Purchased Components](#purchased-components)
    - [Interfaces](#39-interfaces)
    - [Licensing Requirements](#310-licensing-requirements)
    - [Legal, Copyright And Other Notices](#311-legal-copyright-and-other-notices)
    - [Applicable Standards](#312-applicable-standards)
- [Supporting Information](#4-supporting-information)

## 1. Introduction

### 1.1 Purpose
This Software Requirements Specification (SRS) describes all specifications for the application "SimpleSurvey". It includes an overview about this project and its vision, detailed information about the planned features and boundary conditions of the development process.


### 1.2 Scope
The project is going to be realized as a Web-Application.  
 
Actors of this App can be guests, users, creators or administrators.  
 
Planned Subsystems are:
* Notice Board:  
* Account System:  
Users can create accounts so Surveys can be created as well as to join requests. User data must be stored.
* Survey Creation:  
* Survey Sharing:  
* Storing Data:  
User data for accounts and possibly profiles has to be stored. Also the surveys have to be stored as datasets containing the form contents. The data storage will form the foundation for the visualization.

### 1.3 Definitions, Acronyms and Abbreviations
| Abbrevation | Explanation                            |
| ----------- | -------------------------------------- |
| SRS         | Software Requirements Specification    |
| UC          | Use Case                               |
| n/a         | not applicable                         |
| tbd         | to be determined                       |
| UCD         | overall Use Case Diagram               |
| FAQ         | Frequently asked Questions             |

### 1.4 References

| Title                                                              | Date       | Publishing organization   |
| -------------------------------------------------------------------|:----------:| ------------------------- |
| [SimpleSurvey Blog](https://simplesurveyproject.wordpress.com/)    | 13.10.2020 | SimpleSurvey Team    |
| [GitHub]https://github.com/SimpleSurveyProject               | 13.10.2020 | SimpleSurvey Team    |


### 1.5 Overview
The following chapter provides an overview of this project with vision and Overall Use Case Diagram. The third chapter (Requirements Specification) delivers more details about the specific requirements in terms of functionality, usability and design parameters. Finally there is a chapter with supporting information.
    
## 2. Overall Description

### 2.1 Vision

### 2.2 Use Case Diagram

- Green: Planned till end of december
- Orange: Planned till end of june
- White: Additional features

### 2.3 Technology Stack
The technology we use is:

Backend:
-Spring Boot
-MySQL Database

Frontend:
-Angular

IDE:
-Microsoft Visual Studio Code

Project Management:
-YouTrack
-GitHub

Deployment:
-tbd

Testing:
-tbd

## 3. Specific Requirements

### 3.1 Functionality
This section will explain the different use cases, you could see in the Use Case Diagram, and their functionality.  
Until December we plan to implement:
- 3.1.1 Creating an account
- 3.1.2 Logging in
- 3.1.3 Logging out
- 3.1.4 Create survey
- 3.1.5 Fill out survey

Until June, we want to implement:
- 3.1.6 Edit survey
- 3.1.7 Share Survey
- 3.1.8 Evaluate Survey

If we still have time:
-3.1.9 Admin can manage users
-3.1.10 Admin can manage surveys

#### 3.1.1 Creating an account
To identify all users we need an account system. This account system enables us to build important functions such as creating,editing and evaluating a survey.

#### 3.1.2 Logging in
The app will provide the possibility to register and log in. This will also make the usability easier when a user wants to manage his surveys.

#### 3.1.3 Logging out
In case you share your phone, have multiple accounts or just want to be cautious about your privacy you should be able to manually log out.

#### 3.1.4 Create survey
tbd

#### 3.1.5 Fill out survey
tbd

#### 3.1.6 Edit survey
tbd

#### 3.1.7 Share Survey
tbd

#### 3.1.8 Evaluate Survey
tbd

#### 3.1.9 Admin can manage users
tbd

#### 3.1.10 Admin can manage surveys
tbd

#### 3.1.11 Presenting yourself and checking out others
With the possibility to log in there comes another functionality, the profile. Every user will have their own profile where they can write some informations about themselves. Because of the privacy policy in Europe, the user has the possibility to only write the information they want other people to see. Using the profile, users can also check out results of other surveys.


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
We are trying to provide a modern and easy to handle design for the UI as well as for the architecture of our application. To achieve that the functionalities will be kept as modular as possible.

Because we are programming a Web-Application we chose JavaScript  as our programming language. Also we are using the common MVC-architecture to keep the front end and back end separated. For a clean front end structure we use MVC.
To make the communication between the two parts easy, we will implement a RESTful-API between them which will provide the data in JSON-Format.
The supported Platforms will be:
- all modern Browsers

### 3.7 On-line User Documentation and Help System Requirements
The usage of the application should be as intuitive as possible so it won't need any further documentation. If the user needs some help we will implement a "Help"-Button which includes a FAQ and a formular to contact the development team.

### 3.8 Purchased Components
We have bought a domain for the web application and a Linux Server, where the backend runs.

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
- Patrick Braje
- Dominik Seiler
- Simon Fischer
