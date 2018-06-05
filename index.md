# Table of Contents
- [1. Introduction](#1-introduction)
  * [1.1 Project Summary](#11-project-summary)
  * [1.2 Project Purpose](#12-project-purpose)
- [2. Object Classification](#2-object-classification)
  * [2.1 Object Diagram](#21-object-diagram)
  * [2.2 Entity Objects](#22-entity-objects)
  * [2.3 Control Objects](#23-control-objects)
  * [2.4 Boundary Objects](#24-boundary-objects)
- [3. Further Steps](#3-further-steps)
  * [3.1 User Event Loop](#31-user-event-loop)
  * [3.2 Device Controller Event Loop](#32-device-controller-event-loop)  
  * [3.3 User Controls](#33-user-controls)  
- [4. Versions](#4-versions)
- [5. Authored By](#5-authored-by)

# 1. Introduction
## 1.1 Project Summary
_Shout!_  is a bluetooth low energy (BLE) mesh-based messaging application that is supported on Android and iOS. It allows users to talk to other users within a single messaging room as long as they are all connected to the same bluetooth mesh.

## 1.2 Project Purpose
This document will cover all of the analysis needed for _Shout!_ and will describe all of its features and how they work.

The intended audience for this document will be the client (David Brown) and the project team. They will use this document to be reminded of the analysis of the project. The document will also be used as the basis for the project.
			
# 2. Object Classification
						
## 2.1 Object Diagram 

<img src="https://cp317s18.github.io/analysis/analysis-object-diagram.png" align="left" hspace="70" />

## 2.2 Entity Objects
- User - A user of the _Shout!_ application
- Message - User generated text to be broadcasted to other _Shout!_ users
- Device -  The basis for the Bluetooth LE software and its connections 


## 2.3 Control Objects 
- Controller Interface - Coordinates all matters related to the exchange of messages between users
- User Controller - Coordinates all matters related to user data

## 2.4 Boundary Objects
- Relay - Enables the user to pass along messages to or from other users
- Send - Enables the user to export or send messages to other users 
- Receive - Enables the user to obtain or receive messages from other users
- Connect - Establishes the first connection between relay nodes 
- UserView - The UI of the application, connects the user to the application backend 

# 3. Further Steps 

## 3.1 User Event Loop
<img src="https://cp317s18.github.io/analysis/User-Event-Loop.png" align="center" hspace="70" />

## 3.2 Device Controller Event Loop
<img src="https://cp317s18.github.io/analysis/Device-Controller-Event-Loop.png" align="center" hspace="70" width="600"/>

## 3.3 User Controls 
<img src="https://cp317s18.github.io/analysis/User-Controls-Event-Loop.png" align="center" hspace="70" width="400" height="400"/>

# 4. Versions
- Version 0.1 6/03/2018 `Document outline created` 

# 5. Authored by: 
- Jayanth Koroth
- Emily Hryb
- Tiffany Chan
- Greg Murray
- Delina Ghebrekristos
- Andrew Badali

