---
layout: post
title: Mail Delivery Robot (Bayesian Localization)
date: 2022-12-06 12:00:00
description: TurtleBot3 Waffle Pi Bayes Localization
img: trtlebot_prev.png # Add image post (optional)
fig-caption: # Add figcaption (optional)
tags: [ROS, Localization, TurtleBot3]
---
This project involved designing a mail delivery system using the TurtleBot 3 Waffle Pi, integrating state estimation, localization, and real-time control. The robot was programmed to navigate a closed-loop path, stopping at preselected locations (nodes) identified by unique colors.

## Control System
- A **PID controller** was implemented to guide the robot along the black line path, using a downward-facing camera for real-time feedback. 
- Camera data was converted to **HSV format** for improved color detection, overcoming initial challenges with RGB interpretation.

## Localization
- **Bayesian Localization** was applied to estimate the robot's position on a topological map, combining state prediction and measurement updates for accurate positioning.
- **Extended Kalman Filter (EKF)** techniques were used to enhance precision.
![Map]({{site.baseurl}}/assets/img/map.png)

## Simulation and Optimization
- **MATLAB** and **Simulink** were utilized to model robot behavior before deploying the control and localization algorithms in ROS.
- The system was designed to ensure reliable navigation even under challenging conditions, such as communication delays.

<img src="{{site.baseurl}}/assets/img/bayepy.png" alt="Probability Distrubution Change" style="width:40%;" />


## Key Features
- Real-time probability-based localization for high-confidence stops.
- Integration of state prediction and sensor measurements to minimize errors.
- System tuning to balance accuracy and efficiency, with recommendations for faster future performance.

---

This project demonstrated a robust approach to autonomous robot navigation, showcasing problem-solving in:
- Sensor integration.
- Algorithm design.
- Real-world testing.

\
![TurtleBot]({{site.baseurl}}/assets/img/trtlebot.jpg)
<img src="{{site.baseurl}}/assets/img/tbotpath.png" alt="Simulation" style="width:40%;" />


