- [1. Specification - Edit profile](#1-use-case-specification-attack)
    - [1.1 Brief Description](#11-brief-description)
- [2. Flow of Events](#2-flow-of-events)
    - [2.1 Basic Flow](#21-basic-flow)
        - [2.1.1 Activity Diagram](#211-activity-diagram)
        - [2.1.2 Mockup](#212-mockup)
        - [2.1.3 Narrative](#213-narrative)
- [3. Special Requirements](#3-special-requirements)
- [4. Precondition](#4-preconditions)  
- [5. Postconditions](#5-postconditions)
- [6. Extension Points](#6-extension-points)
- [7. Function Points](#7-function-points)

## 1. Use Case Specification - Attack
### 1.1 Brief Description
This use case gives users the possibility to catch littleBeasts. The actor can try to catch a beast, and the system checks if all preconditions are met and the give a chance of success.
## 2. Flow of Events
### 2.1 Basic Flow
#### 2.1.1 Activity Diagram
![Activity Diagram](https://raw.githubusercontent.com/LittleBeasts/documentation/master/useCases/diagrams/Catch.png)
#### 2.1.2 Mockup
#### 2.1.3 Cucumber
You can find the Cucumber .feature file right [here](https://github.com/LittleBeasts/littleBeasts/blob/master/src/test/resources/catch.feature).
## 3. Special requirements
n/a
## 4. Preconditions
The main preconditions for this use case are:
- The actor is engaged in battle
- Actor has required items

## 5. Postconditions
### 5.1 Succesful catch
System checks if the player has a free slot for the caught beast. When there is a free slot, the new beast is added to it.
If not, the player can choose to release a beast from one of the slot or discard the newly aquired beast.
### 5.2 Catch unsuccesful
The player loses their turn and the item is lost. 
## 6. Extension Points
tbd
## 7. Function Points
tbd
