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


1.
# Introduction

_[The introduction of the **Software Architecture Document** provides an overview of the entire **Software Architecture Document**. It includes the purpose, scope, definitions, acronyms, abbreviations, references, and overview of the **Software Architecture Document**.]_

  1.1
## Purpose

This document provides a comprehensive architectural overview of the system, using a number of different architectural views to depict different aspects of the system. It is intended to capture and convey the significant architectural decisions which have been made on the system.

  1.2
## Scope

_[A brief description of what the Software Architecture Document applies to; what is affected or influenced by this document.]_

  1.3
## Definitions, Acronyms, and Abbreviations

n/a: not applicable

  1.4
## References

_[This subsection provides a complete list of all documents referenced elsewhere in the **Software Architecture Document**. Identify each document by title, report number (if applicable), date, and publishing organization. Specify the sources from which the references can be obtained. This information may be provided by reference to an appendix or to another document.]_

  1.5
## Overview

_[This subsection describes what the rest of the **Software Architecture Document** contains and explains how the **Software Architecture Document** is organized.]_

2.
# Architectural Representation

_[This section describes what software architecture is for the current system, and how it is represented. Of the **Use-Case** , **Logical** , **Process** , **Deployment** , and **Implementation Views** , it enumerates the views that are necessary, and for each view, explains what types of model elements it contains.]_

3.
# Architectural Goals and Constraints

_[This section describes the software requirements and objectives that have some significant impact on the architecture; for example, safety, security, privacy, use of an off-the-shelf product, portability, distribution, and reuse. It also captures the special constraints that may apply: design and implementation strategy, development tools, team structure, schedule, legacy code, and so on.]_

4.
# Use-Case View

_[This section lists use cases or scenarios from the use-case model if they represent some significant, central functionality of the final system, or if they have a large architectural coverage—they exercise many architectural elements or if they stress or illustrate a specific, delicate point of the architecture.]_

  4.1
## Use-Case Realizations

_[This section illustrates how the software actually works by giving a few selected use-case (or scenario) realizations, and explains how the various design model elements contribute to their functionality.]_

5.
# Logical View

_[This section describes the architecturally significant parts of the design model, such as its decomposition into subsystems and packages. And for each significant package, its decomposition into classes and class utilities. You should introduce architecturally significant classes and describe their responsibilities, as well as a few very important relationships, operations, and attributes.]_

  5.1
## Overview

_[This subsection describes the overall decomposition of the design model in terms of its package hierarchy and layers.]_

  5.2
## Architecturally Significant Design Packages

_[For each significant package, include a subsection with its name, its brief description, and a diagram with all significant classes and packages contained within the package._

_For each significant class in the package, include its name, brief description, and, optionally, a description of some of its major responsibilities, operations, and attributes.]_

6.
# Process View

n/a

7.
# Deployment View

_[This section describes one or more physical network (hardware) configurations on which the software is deployed and run. It is a view of the Deployment Model. At a minimum for each configuration it should indicate the physical nodes (computers, CPUs) that execute the software and their interconnections (bus, LAN, point-to-point, and so on.) Also include a mapping of the processes of the **Process View** onto the physical nodes.]_

8.
# Implementation View

n/a

  8.1
## Overview

n/a

  8.2
## Layers

n/a

9.
# Data View (optional)

![dbmodel](ressources/dbmodel.png)

10.
# Size and Performance

n/a

11.
# Quality

n/a
