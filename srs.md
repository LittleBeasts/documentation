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

        -   [3.1 Functionality](#31-functionality)
            -   [3.1.1 Menus](#311-menus)
            -   [3.1.2 Player Controls](#312-player-controls)
            -   [3.1.3 Map Interactions](#313-map-interactions)
            -   [3.1.4 Battle](#314-battle)
        -   [3.2 Usability](#32-usability)
            -   [3.2.1 Intuitive control-pattern](#321-intuitive-control-pattern)
            -   [3.2.2 Control Mapping](#322-control-mapping)
            -   [3.2.3 In-Game tutorial](#323-in-game-tutorial)

        -   [3.3 Reliability](#33-reliability)

            -   [3.3.1 JAVA](#331-java)
            -   [3.3.2 Local Application](#332-local-application)

        -   [3.4 Performance](#34-performance)

            -   [3.4.1 GUI](#351-gui)
            -   [3.4.2 Calculation Engine](#342-calculation-engine)
            -   [3.4.3 Loading Times](#353-loading-times)

        -   [3.5 Supportability](#35-supportability)

        -   [3.6 Design Constraints](#37-design-constraints)

        -   [3.7 Online User Documentation and Help System Requirements](#38-online-user-documentation-and-help-system-requirements)

        -   [3.8 Purchased Components](#39-purchased-components)

        -   [3.9 Interfaces](#39-interfaces)

            -   [3.9.1 User Interfaces](#391-user-interfaces)
            -   [3.9.2 Hardware Interfaces](#392-hardware-interfaces)
            -   [3.9.3 Software Interfaces](#393-software-interfaces)
            -   [3.9.4 Communications Interfaces](#394-communications-interfaces)

        -   [3.10 Licensing Requirements](#310-licensing-requirements)

        -   [3.11 Legal, Copyright and other Notices](#311-legal-copyright-and-other-notices)

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
The following document gives a overview over the functionality of the product and provides a more detailed description of the requirements.

## 2. Overall Description

### 2.1 Vision
littleBeasts is a fantasy roleplay game in which you’re thrown into a bizarre world. You'll find friends in the beasts roaming the wild and cities, but you need to persuade them, to fight beside you. Find out what mystery lies behind these littleBeasts.

The game will include an interactive fighting system, an easy leveling mechanic and an explorable map. There will also be a story mode were the player can find NPCs and monsters to interact. In this world there will be safe-zones and battle-zones. In these battle-zones the player can engage in random encounters to find new beasts, gain EXP and loot.

The game will be designed in pixel-art-style with animations for movements and fights.

### 2.2 Use Case Diagram
<img src="https://raw.githubusercontent.com/LittleBeasts/documentation/master/useCases/diagrams/use_cases.png"/>

[Use Case Attack](https://github.com/LittleBeasts/documentation/blob/master/useCases/useCaseAttack.md)

[Use Case Catch](https://github.com/LittleBeasts/documentation/blob/master/useCases/useCaseCatch.md)


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
