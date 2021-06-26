LittleBeasts

---
layout: default
title: SAD
nav_order: 3
parent: Project management
---
# Software Architecture Document 
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

# Revision History

| **Date**           | **Version**        | **Description**    | **Author**         |
|--------------------|--------------------|--------------------|--------------------|
| 22.11.2020         | 1.0                | Initial            | jatsqi             |
| 26.06.2021         |1.1                 |update quality paragraph|  Lawand Allo   |

Table of Contents

[1.Introduction](https://sce.uhcl.edu/helm/RationalUnifiedProcess/webtmpl/templates/a_and_d/rup_sad.htm#1.%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20Introduction)         

[1.1 Purpose](https://sce.uhcl.edu/helm/RationalUnifiedProcess/webtmpl/templates/a_and_d/rup_sad.htm#1.1%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20Purpose)     

[1.2 Scope](https://sce.uhcl.edu/helm/RationalUnifiedProcess/webtmpl/templates/a_and_d/rup_sad.htm#1.2%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20Scope)     

[1.3 Definitions, Acronyms and Abbreviations](https://sce.uhcl.edu/helm/RationalUnifiedProcess/webtmpl/templates/a_and_d/rup_sad.htm#1.3%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20Definitions,%20Acronyms%20and%20Abbreviations)     

[1.4 References](https://sce.uhcl.edu/helm/RationalUnifiedProcess/webtmpl/templates/a_and_d/rup_sad.htm#1.4%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20References)     

[1.5 Overview](https://sce.uhcl.edu/helm/RationalUnifiedProcess/webtmpl/templates/a_and_d/rup_sad.htm#1.5%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20Overview)     

[2. Architectural Representation](https://sce.uhcl.edu/helm/RationalUnifiedProcess/webtmpl/templates/a_and_d/rup_sad.htm#2.%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20Architectural%20Representation)

[3.       Architectural Goals and
Constraints](https://sce.uhcl.edu/helm/RationalUnifiedProcess/webtmpl/templates/a_and_d/rup_sad.htm#3.%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20Architectural%20Goals%20and%20Constraints)   

[4.       Use-Case
View](https://sce.uhcl.edu/helm/RationalUnifiedProcess/webtmpl/templates/a_and_d/rup_sad.htm#4.%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20Use-Case%20View)

[4.1 Use-Case Realizations](https://sce.uhcl.edu/helm/RationalUnifiedProcess/webtmpl/templates/a_and_d/rup_sad.htm#4.1%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20Use-Case%20Realizations)     

 

[5. Logical View](https://sce.uhcl.edu/helm/RationalUnifiedProcess/webtmpl/templates/a_and_d/rup_sad.htm#5.%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20Logical%20View)

[5.1 Overview](https://sce.uhcl.edu/helm/RationalUnifiedProcess/webtmpl/templates/a_and_d/rup_sad.htm#5.1%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20Overview)     

[5.2 Architecturally Significant Design Packages](https://sce.uhcl.edu/helm/RationalUnifiedProcess/webtmpl/templates/a_and_d/rup_sad.htm#5.2%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20Architecturally%20Significant%20Design%20Packages)     

[6. Process View](https://sce.uhcl.edu/helm/RationalUnifiedProcess/webtmpl/templates/a_and_d/rup_sad.htm#6.%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20Process%20View)

[7. Deployment View](https://sce.uhcl.edu/helm/RationalUnifiedProcess/webtmpl/templates/a_and_d/rup_sad.htm#7.%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20Deployment%20View)

[8. Implementation View](https://sce.uhcl.edu/helm/RationalUnifiedProcess/webtmpl/templates/a_and_d/rup_sad.htm#8.%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20Implementation%20View)

[8.1 Overview](https://sce.uhcl.edu/helm/RationalUnifiedProcess/webtmpl/templates/a_and_d/rup_sad.htm#8.1%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20Overview)     

[8.2 Layers](https://sce.uhcl.edu/helm/RationalUnifiedProcess/webtmpl/templates/a_and_d/rup_sad.htm#8.2%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20Layers)     

[9. Data View (optional) ](https://sce.uhcl.edu/helm/RationalUnifiedProcess/webtmpl/templates/a_and_d/rup_sad.htm#9.%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20Data%20View%20(optional))      

[10. Size and Performance](https://sce.uhcl.edu/helm/RationalUnifiedProcess/webtmpl/templates/a_and_d/rup_sad.htm#10.%20%20%20%20%20%20%20%20%20%20%20%20%20Size%20and%20Performance)               

[11. Quality](https://sce.uhcl.edu/helm/RationalUnifiedProcess/webtmpl/templates/a_and_d/rup_sad.htm#11.%20%20%20%20%20%20%20%20%20%20%20%20%20Quality)               

\
 Software Architecture Document

#### 1. Introduction
littleBeasts is a fantasy roleplay game in which you’re thrown into a bizarre world.
The game will include an interactive fighting system, an easy leveling mechanic and an explorable map. There will also be a story mode were the player can find NPCs and monsters to interact. In this world there will be safe-zones and battle-zones. In these battle-zones the player can engage in random encounters to find new beasts, gain EXP and loot.
The game will be designed in pixel-art-style with animations for movements and fights.

##### 1.1 Purpose

This document provides a comprehensive architectural overview of the
system, using a number of different architectural views to depict
different aspects of the system.  It is intended to capture and convey
the significant architectural decisions which have been made on the
system.

##### 1.2 Scope

This document describes the architecture of the littleBeast application, which consists of:
- GUI (implements LITIEngine Framework)
- Calculation Engine

##### 1.3 Definitions, Acronyms and Abbreviations


| Term     |                                     |
| -------- | ----------------------------------- |
| **SRS**  | Software Requirements Specification |
| **GUI**  | Graphical User Interface            |
| **CE**   | Calculation Engine                  |
| **JRE**  | JAVA Runtime Environment            |
| **tbd**  | to be determined                    |
| **n/a**  | not applicable                      |
| **UC**   | Use Case                            |
##### 1.4 References

All references can be found in our documentation Repo [here](https://github.com/LittleBeasts/documentation)

##### 1.5 Overview

In the following sections the aspects Architectural Representation, Architectural Goals and Constraints, class diagram of the project, overview of the use cases and quality assurance are described.

#### 2. Architectural Representation
[High level architecture](https://github.com/LittleBeasts/documentation/blob/master/ProjectStructure.pdf)

The backend consists of the CE which handles all logic processes. 
All GUI elements are created and rendered through the frontend which implements LITIEngine functionality. 
The controller receives the user inputs from the frontend and interacts with the backend.

#### 3. Architectural Goals and Constraints

##### 3.1 Off-the-shelf product
In the project most of graphical implementation is handled with LITIEngine. This includes but is not limited to: 
- Camera control
- Loading and displaying maps and other graphic assets (e.g. charater sprites)
- Animation control
- Menus

##### 3.2 Distribution
LITIEngine support distribution via Steam.

##### 3.3 Development Tools
- IntelliJ
- GitHub
- LITIEngine
- UtiLITI
- Tiled
- Maven
- Cucumber

#### 4. Use-Case View

<img src="https://raw.githubusercontent.com/LittleBeasts/documentation/master/useCases/diagrams/use_cases.png"/>

##### 4.1 Use-Case Realizations
This [catch use case](https://github.com/LittleBeasts/documentation/blob/master/useCases/useCaseCatch.md) gives users the possibility to catch littleBeasts. The actor can try to catch a beast, and the system checks if all preconditions are met and the give a chance of success. The preconditions include the actor being engaged in the battle and having the required item to catch a beast( e.g. a cage). After that the system checks if the player has a free slot for the caught beast. When there is a free slot, the new beast is added to it. If not, the player can choose to release a beast from one of the slot or discard the newly aquired beast.

#### 5. Logical View
Our Project is seperated into two parts:
* The Calculation Engine (CE): this part of the project handles all calculations needed for game actions(e. g. catch, attack, tame) in the background.
* LittleBeasts: this part handles the graphical representation and interaction of the player with the game.

##### 5.1 Overview

[This subsection describes the overall decomposition of the design model
in terms of its package hierarchy and layers.]

##### 5.2 Architecturally Significant Design Packages

[For each significant package, include a subsection with its name, its
brief description, and a diagram with all significant classes and
packages contained within the package.

For each significant class in the package, include its name, brief
description, and, optionally a description of some of its major
responsibilities, operations and attributes.]

#### 6. Process View

[This section describes the system's decomposition into lightweight
processes (single threads of control) and heavyweight processes
(groupings of lightweight processes). Organize the section by groups of
processes that communicate or interact. Describe the main modes of
communication between processes, such as message passing, interrupts,
and rendezvous.]

#### 7. Deployment View

[This section describes one or more physical network (hardware)
configurations on which the software is deployed and run. It is a view
of the Deployment Model. At a minimum for each configuration it should
indicate the physical nodes (computers, CPUs) that execute the software,
and their interconnections (bus, LAN, point-to-point, and so on.) Also
include a mapping of the processes of the **Process View** onto the
physical nodes.]

#### 8. Implementation View
![](https://github.com/LittleBeasts/documentation/blob/master/classDiagram.svg)

[This section describes the overall structure of the implementation
model, the decomposition of the software into layers and subsystems in
the implementation model, and any architecturally significant
components.]

##### 8.1 Overview

[This subsection names and defines the various layers and their
contents, the rules that govern the inclusion to a given layer, and the
boundaries between layers. Include a component diagram that shows the
relations between layers. ]

##### 8.2 Layers

[For each layer, include a subsection with its name, an enumeration of
the subsystems located in the layer, and a component diagram.]

#### 9. Data View (optional)

[A description of the persistent data storage perspective of the system.
This section is optional if there is little or no persistent data, or
the translation between the Design Model and the Data Model is trivial.]

#### 10. Size and Performance

[A description of the major dimensioning characteristics of the software
that impact the architecture, as well as the target performance
constraints.]

#### 11. Quality

Our architecture will provide a framework to easily implement the story of the game. All content can be altered and extended through JSON-Files and designwork in Tiled/UtiLITI so there is no need to code in JAVA.
In order to archive the best possible maintainability the application underlies a continous refactoring process.
##### 11.1 Pattern
Using pattern can be helpful to solve architectural problems in the code in a clean and maintainable way.
In this blog post we used the design pattern Composite and Strategy.
https://littlebeastsgame.wordpress.com/2021/05/17/week-2-6-design-pattern/
##### 11.2 Metrics 
In this blog post we describe how a metrics tool can help you to improve and maintain code quality 
https://littlebeastsgame.wordpress.com/2021/05/31/week-2-7-metrics/
