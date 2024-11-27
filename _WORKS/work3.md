---
title: PNP Robotic ARM 
description: This project focuses on the design, prototyping and implementation of a 4DOF(Degree of Freedom) Robot Arm which is programmable through a Puppet model consisting of 4- potentiometers. The Robot can save up to 10 positions(States) and cycle through them. The states are reprogrammable and a mirror mode is also available that copies the orientation of the puppet robot in real time. This device is a close representation of the pick and place machine commonly deployed in most industrial automated factories and facilities.
imgurl: work1.png
---


## **Key Features**:-

#### **Save/Edit Mode**:
- Save or edit servo motor angular positions to EEPROM.
- **Steps**:
  - Press **Save/Edit** on the keypad.
  - Select the **State** to save/edit.
  - Confirm edits if the state already exists.
  - Position the robot as desired.
  - Press **Save/Edit** to save the position.

#### **Delete Mode**:
- Delete a saved state from EEPROM memory.
- **Steps**:
  - Press **Delete** on the keypad.
  - Warning: Deleting may cause gaps in the state sequence.
  - Select the state to delete and confirm by re-pressing.

#### **Cycle Mode**:
- Cycle through saved states in a loop for pick-and-place functionality.
- **Steps**:
  - Find the endpoint of states.
  - Check for gaps.
  - Resolve gaps or erase subsequent states if found.
  - Cycle states repeatedly until **Cycle**, **Cancel**, or **Reference** is pressed.

#### **Reference Mode**:
- Interrupts current function and sets the robot to a predefined reference position.

#### **Discrete Mode**:
- Test specific states saved in the controller.
- **Steps**:
  - Select a **State** to position the robot accordingly.

#### **Mirror Mode**:
- Mimics real-time movements using potentiometer data from a puppet robot.
- **Steps**:
  - Robot enters **Mirror Mode** after inactivity.
  - Exit the mode by pressing any keypad input.
