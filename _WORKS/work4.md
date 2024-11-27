---
title: Smart Door Lock System
description: Developed a seamless door lock system that removes the conventional key and uses smart security features like RFID and a keypad feature that encrypts a 6-digit numeric passcode. It can add, edit, and block the user using a master user ID and save more than 1000 users into the database system for access.Collaborated additional feature of a burglar alarm for alerts in case of a trespass or breakage of the system.
imgurl: work4.jpg
---


### **Key Highlights**
- **Enhanced Security**: RFID cards/tags are uniquely encoded and cannot be fraudulently duplicated.
- **User Verification**: Only valid users in the database can unlock the door.  
- **Fallback Mechanism**: Integrated keypad for access if RFID tags are unreadable.

## **Features**
- **RFID Fast Access**  
- **Presence Detection** (using PING sensor)  
- **Keypad Access**  
- **Door Open Alarm**  
- **Auto Unlock Mechanism**  
- **Automatic User ID Allocation**  
- **User ID Blocking/Unblocking**  
- **User ID Deletion**  
- **Intruder Alarm**

---

## **Mechanical Design**
- **Tamper-Proof Design**: Screws and access points are placed at the back of the door to prevent tampering.  
- **Integrated Components**: RFID scanner and keypad aligned on the device's right side for seamless operation.

---

## **System Components**

##### **Microcontroller**
- **Teensy 3.5**: Includes an inbuilt SD card module for data storage.

##### **Inputs**
- **Parallax PING Sensor**: Detects human presence.  
- **Keypad**: Allows user input.  
- **RFID Module**: Enables fast access.  
- **IR Sensor**: Detects if the door is open.

##### **Outputs**
- **Parallax LCD Display**: Displays system messages, with an inbuilt buzzer.  
- **Solenoid**: Unlocks the door upon successful authentication.

##### **Power Supply**
- **12V Power Supply**: Provides power to the system.  
- **12V to 5V Buck Converter**: Powers components requiring 5V.

---



---  
This smart lock system combines innovative technology and robust design to provide **secure, reliable, and user-friendly access control**.  
