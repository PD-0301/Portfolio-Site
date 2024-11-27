---
title: Air Purification Robot
description:  Conceptualized and modeled an innovative IoT-based air purification robot to detect and eliminate air pollutants,contributing to environmental sustainability. Successfully reduced the Air Quality Index (AQI) from 100 to 20 by integrating a high-efficiency HEPA filter, showcasing a commitment to creating tangible solutions for air quality improvement
imgurl: work5.1.png
---

## **Key Features**:-
1. **Sensors for Data Collection**
   - **DHT11 Sensor**: Measures temperature and humidity.  
   - **Gas and Particulate Sensors**: Detect air pollutant concentrations.
   
2. **Microcontroller**:  
   - **ESP-32 Board**: Controls system operations and processes sensor data.  
   - Data is displayed on an application interface.  

3. **Filter Control Mechanism**:  
   - A **fan-controlled air filter** is activated based on threshold values from sensor readings.  
   - The fan is managed via a **relay** switched by the microcontroller.

4. **Wireless Communication**:  
   - The system connects to the **Blynk app** via NodeMCU for remote monitoring and control.

5. **Motorized Mobility**:  
   - Wheels equipped with separate motors allow the system to be mobile.  
   - Directional control is achieved through an IoT app keypad.

---

## **System Functionality**:-
1. **Data Collection and Display**:
   - Sensors continuously monitor temperature, humidity, and pollutant levels.  
   - Data is sent to the **Blynk app** for real-time visualization.  

2. **Filter Operation**:
   - If pollutant levels exceed preset thresholds, the **filter fan** is activated to purify the air.  

3. **Motor Control**:
   - A mobile device app enables precise directional control of the system.  
   - Users can start, stop, or reverse motor operation, ensuring efficient air quality management in target areas.

---

## **Applications**:-
- **Indoor Air Monitoring**: Provides real-time tracking of air quality in homes and offices.  
- **Industries and Factories**: Monitors and filters air in environments with high gas and particulate emissions.  
- **Automobile Emission Tracking**: Detects and controls air pollution from vehicles.  
- **Awareness Creation**: Enhances individual understanding of air quality and its health impacts.

---

## **Advantages**:-
- Standalone performance in measuring multiple air parameters, including fine particles.  
- Supports **location identification** and **remote monitoring** for ease of use.  
- Highly adaptable for use in various settings, from residential spaces to industrial facilities.

---

## **Limitations**:-    
- **Device Size**: The inclusion of multiple components increases the system's physical size.  
- **Accuracy Concerns**: Sensor precision may decrease due to rapid changes in environmental parameters.

---

This **Smart Air Filter Monitoring and Controlling System** offers a comprehensive, cost-effective, and adaptable solution for addressing air quality challenges in real time, ensuring a healthier and safer environment.
