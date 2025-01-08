# Visual Servoing and Control

## Overview
This project, **Visual Servoing and Control**, focuses on developing a visual servoing system to control a robotic device using image-based feedback. The work combines computer vision techniques, mathematical modeling, and control algorithms to achieve precise robotic movements based on real-time visual data.

## Key Features
- **Real-Time Image Processing**:
  - Detects and tracks visual markers in real-time (every 40 ms).
  - Calculates the center of gravity of markers for precise localization.
  - Implements thresholding and weighted pixel intensity analysis for robust detection.

- **3D Measurement Reconstruction**:
  - Utilizes the camera's pinhole model to compute the Cartesian position of the target relative to the camera.
  - Integrates intrinsic and extrinsic camera parameters to map image-plane coordinates to real-world positions.

- **Control System**:
  - Employs a Proportional-Integrator (PI) controller for precision and zero steady-state error.
  - Adjusts commands dynamically to correct biases introduced by the interaction between rotational and translational movements of the robot.

## Results
- **System Performance**:
  - Achieved stable convergence of positional and rotational errors within approximately 13 seconds in experiments.
  - Corrected biases caused by the interplay between effector rotation and marker translation.

- **Simulation**:
  - Demonstrated improved servoing performance after bias correction.
  - Visual results and response curves illustrate the system's effectiveness under different conditions.

## Methodology
1. **Image Processing**:
   - Detect and localize markers using intensity-based thresholding and geometric center calculation.
2. **Measurement Reconstruction**:
   - Map image-plane coordinates to 3D Cartesian coordinates using camera calibration parameters.
3. **Control Implementation**:
   - Design and tune a PI controller to ensure accurate tracking with zero steady-state error.

## Visual Results
- Graphs showing the system's positional and command responses.
- Comparison of marker trajectories before and after bias correction.

## Learn More
The complete analysis, along with simulation videos, is available in the report and accompanying resources.

[Watch the simulation video](https://drive.google.com/file/d/1G9j12TRtXA1cIZMSNYV0TnFxQsdkZ0lF/view?usp=share_link)

---

## Author
**Nkimo Lenou Randolf**  
Telecom Physique Strasbourg, 2023  

Supervised by: **Zanne Philippe**

## Acknowledgements
This project was part of the TPE-ISAV course and reflects extensive work in robotic visual servoing and control systems.

---

