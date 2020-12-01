**Table of Contents**

1. Introduction

1.1 Purpose

1.2 Scope

1.3 Definitions, Acronyms, and Abbreviations

1.4 References

1.5 Overview

2. Architectural Representation

3. Architectural Goals and Constraints

4. Use-Case View

4.1 Use-Case Realizations

5. Logical View

5.1 Overview

5.2 Architecturally Significant Design Packages

6. Process View

7. Deployment View

8. Implementation View

8.1 Overview

8.2 Layers

9. Data View (optional)

10. Size and Performance

11. Quality


# 1. Introduction

The introduction of the **Software Architecture Document** provides an overview of the entire **Software Architecture Document**. It includes the purpose, scope, definitions, acronyms, abbreviations, references, and overview of the **Software Architecture Document**.

## 1.1 Purpose

This document provides a comprehensive architectural overview of the system, using a number of different architectural views to depict different aspects of the system. It is intended to capture and convey the significant architectural decisions which have been made on the system.

## 1.2 Scope

This document describes the way we write code and how we connect the components of the project.

## 1.3 Definitions, Acronyms, and Abbreviations

| Abbrevation | Description                            |
| ----------- | -------------------------------------- |
| n/a         | not applicable                         |

## 1.4 References

[Blog](https://simplesurveyproject.wordpress.com/)
[GitHub Repository](https://github.com/SimpleSurveyProject)
[Use Case Diagram](https://screen.simonlabs.de/img.php?id=2I0cisf)
[Fill out survey Use Case](https://github.com/SimpleSurveyProject/SimpleSurvey-Documentation/blob/main/use-case-fillsOutSurvey.md)
[Share survey Use Case](https://github.com/SimpleSurveyProject/SimpleSurvey-Documentation/blob/main/use-case-sharesSurvey.md)
[Database model](ressources/dbmodel.png)

## 1.5 Overview

This document contains the architectural representation, goals and constraints as well as the logical, deployment, implementation and data views.

# 2. Architectural Representation

We are implementing according to the MVC pattern:
![ucd](https://github.com/SimpleSurveyProject/SimpleSurvey-Documentation/blob/main/ressources/MVC.png)

# 3. Architectural Goals and Constraints

For the **frontend** we will use Angular. Angular is a JavaScript framework which was developed by Google. It aims at the development of web applications and attaches great importance to structure and quality. It was the first framework which was also suitable for large enterprise applications due to its focus on architecture, testing and isolated components in the JavaScript area.
Our **backend** is realized with Spring Boot. Spring Boot is a Java framework that aims to simplify programming with Java by avoiding repetitive code and encouraging good programming practices. With Spring Security we will implement authentication and login, with Spring Data we will connect to the database.

# 4. Use-Case View

![ucd](https://screen.simonlabs.de/img.php?id=2I0cisf)

## 4.1 Use-Case Realizations

A few use cases can be found here:
[Fill out survey](https://github.com/SimpleSurveyProject/SimpleSurvey-Documentation/blob/main/use-case-fillsOutSurvey.md)
[Share survey](https://github.com/SimpleSurveyProject/SimpleSurvey-Documentation/blob/main/use-case-sharesSurvey.md)

# 5. Logical View

_[This section describes the architecturally significant parts of the design model, such as its decomposition into subsystems and packages. And for each significant package, its decomposition into classes and class utilities. You should introduce architecturally significant classes and describe their responsibilities, as well as a few very important relationships, operations, and attributes.]_

## 5.1 Overview

_[This subsection describes the overall decomposition of the design model in terms of its package hierarchy and layers.]_

## 5.2 Architecturally Significant Design Packages

_[For each significant package, include a subsection with its name, its brief description, and a diagram with all significant classes and packages contained within the package._

_For each significant class in the package, include its name, brief description, and, optionally, a description of some of its major responsibilities, operations, and attributes.]_

# 6. Process View

n/a

# 7. Deployment View

_[This section describes one or more physical network (hardware) configurations on which the software is deployed and run. It is a view of the Deployment Model. At a minimum for each configuration it should indicate the physical nodes (computers, CPUs) that execute the software and their interconnections (bus, LAN, point-to-point, and so on.) Also include a mapping of the processes of the **Process View** onto the physical nodes.]_

# 8. Implementation View

n/a

## 8.1 Overview

n/a

## 8.2 Layers

n/a

# 9. Data View (optional)

![dbmodel](ressources/dbmodel.png)

# 10. Size and Performance

n/a

# 11. Quality

n/a