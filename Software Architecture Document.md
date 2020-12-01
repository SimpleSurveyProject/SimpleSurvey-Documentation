\&lt;Company Name\&gt;

\&lt;Project Name\&gt;

Software Architecture Document

**Version \&lt;1.0\&gt;**

_[Note: The following template is provided for use with the Rational Unified Process. Text enclosed in square brackets and displayed in blue italics (style=InfoBlue) is included to provide guidance to the author and should be deleted before publishing the document. A paragraph entered following this style will automatically be set to normal (style=Body Text).]_

_[To customize automatic fields in Microsoft Word (which display a gray background when selected), select File\&gt;Properties and replace the Title, Subject and Company fields with the appropriate information for this document. After closing the dialog, automatic fields may be updated throughout the document by selecting Edit\&gt;Select All (or Ctrl-A) and pressing F9, or simply click on the field and press F9. This must be done separately for Headers and Footers. Alt-F9 will toggle between displaying the field names and the field contents. See Word help for more information on working with fields.]_

**Revision History**

| **Date** | **Version** | **Description** | **Author** |
| --- | --- | --- | --- |
| \&lt;dd/mmm/yy\&gt; | \&lt;x.x\&gt; | \&lt;details\&gt; | \&lt;name\&gt; |
|
 |
 |
 |
 |
|
 |
 |
 |
 |
|
 |
 |
 |
 |

**Table of Contents**

1.Introduction 2

1.1Purpose 2

1.2Scope 2

1.3Definitions, Acronyms, and Abbreviations 2

1.4References 2

1.5Overview 2

2.Architectural Representation 2

3.Architectural Goals and Constraints 2

4.Use-Case View 2

4.1Use-Case Realizations 2

5.Logical View 2

5.1Overview 2

5.2Architecturally Significant Design Packages 2

6.Process View 2

7.Deployment View 2

8.Implementation View 2

8.1Overview 2

8.2Layers 2

9.Data View (optional) 2

10.Size and Performance 2

11.Quality 2

Software Architecture Document

1.
# Introduction

_[The introduction of the **Software Architecture Document** provides an overview of the entire **Software Architecture Document**. It includes the purpose, scope, definitions, acronyms, abbreviations, references, and overview of the **Software Architecture Document**.]_

  1.
## Purpose

This document provides a comprehensive architectural overview of the system, using a number of different architectural views to depict different aspects of the system. It is intended to capture and convey the significant architectural decisions which have been made on the system.

_[This section defines the role or purpose of the **Software Architecture Document** , in the overall project documentation, and briefly describes the structure of the document. The specific audiences for the document is identified, with an indication of how they are expected to use the document.]_

  1.
## Scope

_[A brief description of what the Software Architecture Document applies to; what is affected or influenced by this document.]_

  1.
## Definitions, Acronyms, and Abbreviations

_[This subsection provides the definitions of all terms, acronyms, and abbreviations required to properly interpret the **Software Architecture Document**.  This information may be provided by reference to the project&#39;s Glossary.]_

  1.
## References

_[This subsection provides a complete list of all documents referenced elsewhere in the **Software Architecture Document**. Identify each document by title, report number (if applicable), date, and publishing organization. Specify the sources from which the references can be obtained. This information may be provided by reference to an appendix or to another document.]_

  1.
## Overview

_[This subsection describes what the rest of the **Software Architecture Document** contains and explains how the **Software Architecture Document** is organized.]_

1.
# Architectural Representation

_[This section describes what software architecture is for the current system, and how it is represented. Of the **Use-Case** , **Logical** , **Process** , **Deployment** , and **Implementation Views** , it enumerates the views that are necessary, and for each view, explains what types of model elements it contains.]_

1.
# Architectural Goals and Constraints

_[This section describes the software requirements and objectives that have some significant impact on the architecture; for example, safety, security, privacy, use of an off-the-shelf product, portability, distribution, and reuse. It also captures the special constraints that may apply: design and implementation strategy, development tools, team structure, schedule, legacy code, and so on.]_

1.
# Use-Case View

_[This section lists use cases or scenarios from the use-case model if they represent some significant, central functionality of the final system, or if they have a large architectural coverage—they exercise many architectural elements or if they stress or illustrate a specific, delicate point of the architecture.]_

  1.
## Use-Case Realizations

_[This section illustrates how the software actually works by giving a few selected use-case (or scenario) realizations, and explains how the various design model elements contribute to their functionality.]_

1.
# Logical View

_[This section describes the architecturally significant parts of the design model, such as its decomposition into subsystems and packages. And for each significant package, its decomposition into classes and class utilities. You should introduce architecturally significant classes and describe their responsibilities, as well as a few very important relationships, operations, and attributes.]_

  1.
## Overview

_[This subsection describes the overall decomposition of the design model in terms of its package hierarchy and layers.]_

  1.
## Architecturally Significant Design Packages

_[For each significant package, include a subsection with its name, its brief description, and a diagram with all significant classes and packages contained within the package._

_For each significant class in the package, include its name, brief description, and, optionally, a description of some of its major responsibilities, operations, and attributes.]_

1.
# Process View

_[This section describes the system&#39;s decomposition into lightweight processes (single threads of control) and heavyweight processes (groupings of lightweight processes). Organize the section by groups of processes that communicate or interact. Describe the main modes of communication between processes, such as message passing, interrupts, and rendezvous.]_

1.
# Deployment View

_[This section describes one or more physical network (hardware) configurations on which the software is deployed and run. It is a view of the Deployment Model. At a minimum for each configuration it should indicate the physical nodes (computers, CPUs) that execute the software and their interconnections (bus, LAN, point-to-point, and so on.) Also include a mapping of the processes of the **Process View** onto the physical nodes.]_

1.
# Implementation View

_[This section describes the overall structure of the implementation model, the decomposition of the software into layers and subsystems in the implementation model, and any architecturally significant components.]_

  1.
## Overview

_[This subsection names and defines the various layers and their contents, the rules that govern the inclusion to a given layer, and the boundaries between layers. Include a component diagram that shows the relations between layers.]_

  1.
## Layers

_[For each layer, include a subsection with its name, an enumeration of the subsystems located in the layer, and a component diagram.]_

1.
# Data View (optional)

_[A description of the persistent data storage perspective of the system. This section is optional if there is little or no persistent data, or the translation between the Design Model and the Data Model is trivial.]_

1.
# Size and Performance

_[A description of the major dimensioning characteristics of the software that impact the architecture, as well as the target performance constraints.]_

1.
# Quality

_[A description of how the software architecture contributes to all capabilities (other than functionality) of the system: extensibility, reliability, portability, and so on. If these characteristics have special significance, such as safety, security or privacy implications, they must be clearly delineated.]_
