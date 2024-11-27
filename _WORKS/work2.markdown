---
title: Color Cube Sorting Robotic Arm
description: This project presents the design and implementation of a 4DOF robotic arm system for automated color sorting of cubes on a conveyor belt. Equipped with a color sensor, the robotic arm autonomously detects and sorts cubes based on their color as they move along the belt. By seamlessly integrating mechanical, electrical, and software components, this system showcases a fully automated solution for efficient color sorting in real-time.

imgurl: work2.png
---

## **Key Features**
- Simultaneous operation of multiple cogs for efficiency.
- Noise reduction in sensor readings using averaging.
- Robust color detection using machine learning (softmax regression).
- Dynamic conveyor control based on sensor input.
- Accurate tracking of conveyor travel distance to handle adjacent cube cases.

### **System Workflow**
There are 6 cogs working simultaneously in a loop to detect color, pick, and place the cubes:

1. **Cog 0**: Initializes other cogs and global variables.
2. **Cog 1**: Continuously acquires ultrasonic distance measurements.
3. **Cog 2**: Detects the color of cubes using a color sensor.
4. **Cog 3**: Performs pick-and-place operations with the manipulator.
5. **Cog 4**: Controls the conveyor motion based on distance measurements.
6. **Cog 5**: Tracks the conveyor’s travel distance.

---

## **Detailed Cog Functions**

### **Cog 0**: Initialization
- Initializes global variables, function declarations, and stack arrays.
- Sets up operations for:
  - Color detection.
  - Conveyor and manipulator actuation.
  - Ultrasonic sensor measurements.
  - Conveyor travel distance tracking.

---

### **Cog 1**: Ultrasonic Distance Measurement
- Continuously measures and updates the global `distance` variable.
- Uses the average of 3 consecutive ultrasonic sensor readings to reduce noise errors.
- Provides distance data for manipulator and conveyor actuation.

---

### **Cog 2**: Color Detection
- Performs robust color estimation using **softmax regression**.
- **Steps**:
  - Raw color sensor data is collected for each cube.
  - Softmax regression model is trained using the **Keras library** in Python:
    ```python
    # Example softmax regression in Python
    from keras.models import Sequential
    from keras.layers import Dense
    model = Sequential([
        Dense(3, activation='softmax', input_dim=input_dim)
    ])
    model.compile(optimizer='adam', loss='categorical_crossentropy', metrics=['accuracy'])
    ```
  - Trained model parameters are used in the `detect` function to estimate cube colors.
- **Error Mitigation**:
  - Takes the highest frequency estimate out of 3 continuous estimates.
  - Checks for adjacent cubes of the same color by comparing conveyor travel distance with the maximum cube size.

---

### **Cog 3**: Pick and Place Operation
- Controls manipulator servos to sort cubes.
- Places cubes based on the values stored in the global `colors` array.

---

### **Cog 4**: Conveyor Motion Control
- Operates the conveyor using a stepper motor.
- Conveyor runs continuously unless the global `distance` variable drops below 4, indicating a cube has reached the pickup position.

---

### **Cog 5**: Conveyor Distance Tracking
- Tracks the total distance traveled by the conveyor.
- Enables detection of adjacent cubes of the same color to avoid errors during sorting.

---



