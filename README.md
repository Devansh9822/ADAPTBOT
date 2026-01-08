# ADAPTBOT – Autonomous Obstacle Avoidance and Line Following Robot


ADAPTBOT is a **battery-powered autonomous mobile robot** developed as a **first complete hands-on robotics project**. The project focuses on implementing and integrating the core fundamentals of **mobile robotics**, including motor control, sensor-based navigation, embedded programming, and mechanical design.

The robot is capable of **obstacle avoidance** and **line following**, operating completely onboard without any external computation or laptop connection.

---

## Project Overview

ADAPTBOT uses a **differential-drive mechanism** with two DC gear motors and a caster wheel for balance. Motor control is handled using an **L298N dual H-bridge motor driver**, interfaced with an **Arduino Uno**, enabling bidirectional motion and speed control through PWM.

For navigation, the robot combines **two sensing systems**:

- **Obstacle Avoidance:**  
  An **HC-SR04 ultrasonic sensor** mounted on a **servo motor** actively scans the environment by rotating left, center, and right. Based on distance measurements, the robot detects obstacles in its path, stops, and turns toward the direction with more free space.

- **Line Following:**  
  **Infrared (IR) reflectance sensors** are used to detect surface contrast and follow a predefined path. Left and right IR sensors provide feedback to correct wheel speeds, allowing the robot to track a line using differential steering.

These behaviors allow ADAPTBOT to autonomously navigate structured environments while reacting to obstacles in real time.

---

## Hardware Components

- Arduino Uno  
- L298N dual H-bridge motor driver  
- DC gear motors with wheels  
- HC-SR04 ultrasonic sensor  
- SG90 micro servo motor  
- IR reflectance sensors  
- 2S Li-ion battery pack  
- Buck converter for regulated logic power  
- Custom 3D-printed chassis  

---

## Software and Control Logic

The robot is programmed using **Arduino (C/C++)**. The control logic includes:
- Continuous forward motion under normal conditions  
- Real-time distance measurement using ultrasonic timing  
- Servo-based scanning to determine obstacle direction  
- Differential motor control for turning and correction  
- Line-following control based on IR sensor feedback  

The software emphasizes **clear logic flow, modular motor control, and reliable sensor interfacing**.

---

## Mechanical Design

All structural components, including the chassis and mounts, were **custom-designed in CAD and 3D printed**. The design prioritizes:
- Correct motor alignment  
- Adequate ground clearance  
- Compact and accessible component placement  

---

## Project Purpose

This project was built to gain **practical experience in end-to-end robotics system integration**, covering mechanical design, electronics, power management, and embedded software. ADAPTBOT serves as a foundational platform for learning and future improvements.

---

## Project Status

**ADAPTBOT v1.0 — Completed**

