# littleBeasts - Software Requirements Specification

## Table of Contents

-   [littleBeasts - Software Requirements Specification](#flashcard-community---software-requirements-specification)

    -   [Table of Contents](#table-of-contents)

    -   [1. Introduction](#1-introduction)

        -   [1.1 Purpose](#11-purpose)
        -   [1.2 Scope](#12-scope)
        -   [1.3 Definitions, Acronyms and Abbreviations](#13-definitions-acronyms-and-abbreviations)
        -   [1.4 References](#14-references)
        -   [1.5 Overview](#15-overview)

    -   [2. Overall Description](#2-overall-description)

        -   [2.1 Vision](#21-vision)
    -   [2.2 Use Case Diagram](#22-use-case-diagram)
    -   [2.3 Product perspective](#23-product-perspective)

        -   [2.4 User characteristics](#24-user-characteristics)
        -   [2.5 Dependencies](#25-dependencies)

    -   [3. Specific Requirements](#3-specific-requirements)

        -   [3.1 Functionality – Data Backend](#31-functionality--data-backend)

            -   [3.1.1 Read data given over API endpoints](#311-read-data-given-over-api-endpoints)
            -   [3.1.2 Parse data](#312-parse-data)
            -   [3.1.3 Provide data](#313-provide-data)

        -   [3.2 Functionality – User Interface](#32-functionality--user-interface)

            -   [3.2.1 User system](#321-user-system)
            -   [3.2.3 Flashcard boxes](#323-flashcard-boxes)
            -   [3.2.4 Flashcards](#324-flashcards)
            -   [3.2.5 Statistics](#325-statistics)

        -   [3.3 Usability](#33-usability)

        -   [3.4 Reliability](#34-reliability)

            -   [3.4.1 Availability](#341-availability)
            -   [3.4.2 MTBF, MTTR](#342-mtbf-mttr)
            -   [3.4.3 Accuracy](#343-accuracy)
            -   [3.4.4 Bug classes](#344-bug-classes)

        -   [3.5 Performance](#35-performance)

            -   [3.5.1 Response time](#351-response-time)
            -   [3.5.2 Throughput](#352-throughput)
            -   [3.5.3 Capacity](#353-capacity)
            -   [3.5.4 Resource utilization](#354-resource-utilization)

        -   [3.6 Supportability](#36-supportability)

        -   [3.7 Design Constraints](#37-design-constraints)

            -   [3.7.1 Development tools](#371-development-tools)
            -   [3.7.2 Spring Boot](#372-spring-boot)
            -   [3.7.3 ReactJS](#373-reactjs)
            -   [3.7.4 Supported Platforms](#374-supported-platforms)

        -   [3.8 Online User Documentation and Help System Requirements](#38-online-user-documentation-and-help-system-requirements)

        -   [3.9 Purchased Components](#39-purchased-components)

        -   [3.10 Interfaces](#310-interfaces)

            -   [3.10.1 User Interfaces](#3101-user-interfaces)
            -   [3.10.2 Hardware Interfaces](#3102-hardware-interfaces)
            -   [3.10.3 Software Interfaces](#3103-software-interfaces)
            -   [3.10.4 Communications Interfaces](#3104-communications-interfaces)

        -   [3.11 Licensing Requirements](#311-licensing-requirements)

        -   [3.12 Legal, Copyright and other Notices](#312-legal-copyright-and-other-notices)

        -   [3.13 Applicable Standards](#313-applicable-standards)

    -   [4. Supporting Information](#4-supporting-information)

## 1. Introduction
### 1.1 Purpose
The purpose of this document is to present a detailed description of the littleBeast project. It will explain the features of the application, what the application will do and the constraints under which it must operate and how the application will react to external actions. This document is intended for both the stakeholders and the developers of the application.

### 1.2 Scope
This SRS applies to the entire littleBeast project. 'littleBeast' is a roleplay game which brings the player into a world with so called littleBeast.
These can be tamed or cought and the player can engage in battles with the littleBeasts. It will be realized as an Java application. 
The overview of the features and subsystems are documented in the Use-Case model shown in Overall Description.

### 1.3 Definitions, Acronyms and Abbreviations

| Term     |                                     |
| -------- | ----------------------------------- |
| **SRS**  | Software Requirements Specification |
| **JSON** | JavaScript Object Notation          |
| **API**  | Application Programming Interface   |
| **FAQ**  | Frequently Asked Questions          |
| **REST** | Representational State Transfer     |

### 1.4 References

| Title                                                                                                 | Date       |
| ----------------------------------------------------------------------------------------------------- | ---------- |
| [Blog](https://littlebeastsgame.wordpress.com/)                                                       | 19/10/2020 |
| [GitHub](https://github.com/LittleBeasts)                                                             | 19/10/2020 |
| [Liti Engine](https://litiengine.com/)                                                                | 19/10/2020 |
| [Use Case Diagram](https://github.com/LittleBeasts/documentation/blob/master/use_cases.png)           | 19/10/2018 |

### 1.5 Overview
The following of this document gives overview over the functionality of the product and provides an more detailed description of the requirements.
## 2. Overall Description

### 2.1 Vision
littleBeasts is a fantasy roleplay game in which you’re thrown into a bizarre world. You will find friends in the beasts roaming the wild and cities, but you need to persuade them, to fight beside you. Find out, what mystery lies behind these littleBeasts.

The game will include an interactive fighting system, an easy leveling mechanic and an explorable map. There will also be a story mode were the player can find NPCs and monsters to interact. In this world there will be safe-zones and battle-zones. In these battle-zones the player can engage in random encounters to find new beasts, gain EXP and loot.

The game will be designed in pixel-art-style with small animations for movements and fights.

### 2.2 Use Case Diagram
<img src="https://github.com/LittleBeasts/documentation/blob/master/use_cases.png"/>

### 2.3 Product perspective
This game will stand out from it's competators by bringing you a unique and unforgetable experience. The fighting system is one of a kind and completely engineered from the ground up. You'll be able to play the game the way you want. Wether you want to fight and catch or find friends and tame. It's completely up to you. The story will blow you away and keep you up long at night. Are you able to find out what happened in the world of littleBeasts. Are you strong and brave enough to handle them? Available as early as next year!

### 2.4 User characteristics
The game is targeted at users who like the dark and interesting world of H.P.Lovecraft, who like story intense RPG-games and of course catching and collecting littleBeasts. The user won't need special background information in order to play and understand the game.

### 2.5 Dependencies
We have to support several operating-Systems: Linux and Windows. This will be achieved by using Java as our choice of implementation. For an easier and faster approach to game development we chose a new Java-game-engine, the Litiengine. It's espacially made for 2D-Tile-based games.

## 3. Specific Requirements
TBD.

### 3.1 Functionality - Calculation Engine

### 3.2 Functionality – User Interface

### 3.3 Usability

### 3.4 Reliability

### 3.5 Performance

#### 3.5.1 Response time

#### 3.5.4 Resource utilization

### 3.6 Supportability

### 3.7 Design Constraints

#### 3.7.1 Development tools

#### 3.7.2 Litiengine

#### 3.7.4 Supported Platforms

### 3.8 Online User Documentation and Help System Requirements

### 3.10 Interfaces

#### 3.10.1 User Interfaces

#### 3.10.2 Hardware Interfaces

#### 3.10.3 Software Interfaces

#### 3.10.4 Communications Interfaces

### 3.11 Licensing Requirements

### 3.12 Legal, Copyright and other Notices
