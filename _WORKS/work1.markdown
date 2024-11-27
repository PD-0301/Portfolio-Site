---
title: Automated Object Retrieval Mobile Robot
description: Developed an automated mobile robot capable of identifying and retrieving color cubes placed on an arena, based on color detection. By integrating computer vision and robotic manipulation, the system will detect the position of both the arena and the target object, instructing the robot to navigate, grip, and relocate the object to a designated area based on its color.


imgurl: work3.jpg
---

# **Key Features**:-
- **Camera Calibration**: Accurate transformation of 2D pixel data to 3D world coordinates.
- **Color & Shape Detection**: Robust identification and classification of objects.
- **Object Localization**: Precise determination of object and robot positions.
- **PID-Based Navigation**: Efficient trajectory control for object retrieval.

---

# **Algorithm**:-

##### **1. Camera Calibration**
**Purpose**: Relate 2D pixel coordinates to 3D world coordinates.  
- **Intrinsic Parameters**: 
  - Captured using 30 checkerboard images from various angles using MATLAB.
  - Calibrated to compute the focal length, optical center, and distortion coefficients.
- **Extrinsic Parameters**:  
  - Arena dimensions are determined using checkerboards placed at known corners.
  - Corners detected via image processing for calculating the camera’s position and orientation.

---

##### **2. Color and Shape Detection**:-
1. **Image Capture**: Acquire high-resolution images.  
2. **BGR to HSV Conversion**: Convert to HSV for better segmentation of colors.  
3. **Color Masking**: Filter colors (blue, green, magenta) using HSV thresholds.  
4. **Centroid Detection**: Use moments to calculate object positions.  
5. **Classification**: Distinguish patches and cubes based on their area.  
6. **World Coordinate Transformation**: Convert centroid positions to world coordinates.

---

##### **3. Object Localization**:-
Using calibrated parameters, the robot determines the pose of objects and itself in the world frame.  
- **Depth (Zw)**: Calculated first to find **Xw** and **Yw** coordinates of the target.

---

##### **4. Navigation**:-
**Control Technique**:  
- **PID Controller**: Guides the robot’s trajectory to the target using wheel angular velocity ratio.  
- **Error Term**: Difference between the robot's current orientation and the target direction.

**Tuning**:  
- Simulated in Simulink for initial parameters:  
  - **Kp** = 1.317, **Ki** = 0.5039, **Kd** = -0.1388.  
- Manually tuned for best performance:  
  - **Kp** = 1, **Ki** = 0, **Kd** = 0.

---

# **Applications**:-
- **Logistics**: Automated sorting and retrieval systems.  
- **Automation**: Smart factories for material handling.  
- **Research**: Advanced robotics and AI integration.

  