# ROBOFEST-4.0
Autonomous Rocker-Bogie Rover developed for ROBOFEST Gujarat 4.0 (Level-III Prototype), featuring GNSS-based navigation, LiDAR &amp; Depth Camera SLAM, ROS 2 (Foxy), and rugged mechanical design for extreme terrains.
This repository documents the design, development, and implementation of an autonomous rover built for ROBOFEST Gujarat 4.0 – Level III Prototype.
The rover is designed to operate in harsh and uneven terrains, combining a rocker-bogie suspension, high-torque planetary motors, and a ROS 2–based autonomous navigation stack.
The project integrates mechanical design, embedded systems, robotics middleware, and autonomous navigation, making it suitable for planetary exploration, disaster response, and industrial inspection

# Key Features
- Rocker-Bogie suspension for high terrain adaptability
- High-torque planetary motors (≈100 Nm)
- Custom power distribution & signal routing PCBs
- ROS 2 (Foxy) based distributed architecture
- GNSS-assisted outdoor navigation
- LiDAR & depth-camera based SLAM (RTAB-Map)
- Nav2 framework for autonomous path planning
- Manual & autonomous control modes
- Modular and scalable system architecture

# System Architecture
- Hardware Overview
- Raspberry Pi 5 – High-level processing & autonomy
- ESP32 (Micro-ROS) – Motor & sensor interface
- Planetary DC Motors (12V)
- MDD10A Motor Drivers
- YD LiDAR (360° scanning)
- MPU6050 / MPU9250 IMU
- GNSS Module (RUSH FPV GNSS Pro)
- Depth Camera
- Custom Power Distribution PCB
- Custom Signal PCB

# Mechanical Design
- Chassis: Stainless steel + aluminium extrusion
- Suspension: Passive rocker-bogie with rod differential
- Wheel Design: Hollow PVC wheels with high-grip surface
- Drive System: Independent wheel motors

# Advantages:
- Maintains all six wheels in contact with terrain
- Reduced body jerk via differential averaging
- Capable of climbing obstacles up to 2× wheel diameter

# Software Stack
- Operating Environment
- OS: Raspberry Pi OS (64-bit)
- Containerization: Docker
- Middleware: ROS 2 Foxy
- Core ROS 2 Components
- Nodes, Topics, Services, Actions
- TF2 transform tree
- DDS middleware with QoS control
- Lifecycle-managed nodes

# Navigation & Mapping
- RTAB-Map: Real-time SLAM using LiDAR & depth camera
- Nav2: Path planning, control, and recovery behaviors
- robot_localization: EKF-based sensor fusion
- RViz & RQT Graph: Visualization and debugging

# Control Modes
- Autonomous Mode: GNSS + SLAM + Nav2
- Manual Mode: PS5 controller via ESP32
- Safety: Emergency stop on obstacle detection

# Competition Details
- Event: ROBOFEST Gujarat 4.0
- Level: Level-III (Prototype Demonstration)
- Team: Team Manik
- Mentor: Dr. Milind V. Bhalerao
- Institution: SGGSIE&T, Nanded
