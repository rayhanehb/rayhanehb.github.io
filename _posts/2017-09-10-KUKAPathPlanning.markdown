---
layout: post
title: Robotic Arm Motion Planning - 6-DOF KUKA Manipulator
date: 2024-11-27 12:00:00
description: Design and implementation of forward and inverse kinematics for a 6-DOF KUKA manipulator, along with motion planning for obstacle avoidance.
img: kuka.png # Add image post (optional)
fig-caption: Robotic Arm Motion Planning with Obstacle Avoidance
tags: [Robotics, Motion Planning, Kinematics, Obstacle Avoidance, Trajectory Optimization]
---

This project involved designing and implementing forward and inverse kinematics for a **6-DOF KUKA industrial manipulator** and developing motion planning algorithms for obstacle avoidance. The system enables the robotic arm to perform automated tasks with precise control, tracing objects and navigating through obstacles.

## Section 1: **Drawing with Inverse Kinematics**

The robotic arm was tasked with **tracing a jug** using inverse kinematics. By solving the inverse kinematic equations, the arm successfully determined the joint angles required to move its end effector to each point along the jug’s outline.

- **Forward Kinematics**: First, the position of the end effector was determined from the joint angles.
- **Inverse Kinematics**: The arm solved for joint angles corresponding to a desired end effector position, allowing it to trace the outline of the jug precisely.

![Robotic Arm Tracing Jug]({{site.baseurl}}/assets/img/kuka_jug.png)
<img src="{{site.baseurl}}/assets/img/kuka_jug.png" alt="Simulation" style="width:40%;" />

The algorithm ensured smooth motion and precise placement of the arm at each point along the jug’s outline, allowing for detailed tracing. The robotic arm adapted to each segment of the jug's curve, ensuring an accurate representation of the shape.

## Section 2: **Obstacle Avoidance with Motion Planning**

In addition to inverse kinematics, the project also included **motion planning** for **obstacle avoidance**. The robotic arm was programmed to navigate around obstacles while maintaining an optimized path to its destination. 

- **Artificial Potential Fields (APF)** were implemented to generate safe, efficient paths. The attractive force guided the arm toward its target, while the repulsive force kept the arm away from obstacles.
- The algorithm optimized the trajectory in real time, ensuring smooth motion while avoiding any interference with obstacles in the workspace.

<img src="{{site.baseurl}}/assets/img/kuka_potfield_diag.png" alt="Simulation" style="width:40%;" />


## Simulation Results
- The system demonstrated successful **obstacle avoidance** during real-time simulations.
- The robotic arm moved efficiently through a cluttered environment, adjusting its path as needed to avoid obstacles and reach the destination.

<img src="{{site.baseurl}}/assets/img/kuka_sim3.png" alt="Simulation" style="width:50%;" />


## Final Outcome
The project successfully demonstrated the ability of the robotic arm to trace complex shapes using **inverse kinematics** and navigate through a workspace with **obstacle avoidance**.

<!-- <a href="https://drive.google.com/file/d/18MrcxGV1CKtQKMXuPYICOO4k5warMc_t/view?usp=sharing" target="_blank">
    <img src="{{site.baseurl}}/assets/img/kuka_vid_prev.png" alt="KUKA Obstacle Avoidance Path Planning" style="width:100%; max-width:600px; border: 1px solid #ddd; border-radius: 4px;">
</a> -->

<video width="90%" controls>
  <source src="{{site.baseurl}}/assets/img/kuka_demo2.webm" type="video/webm">
  Your browser does not support the video tag.
</video>

This project showcases expertise in:
- **Kinematic modeling** for robotics.
- **Motion planning algorithms** using artificial potential fields.
- **Obstacle avoidance** and real-time trajectory optimization.

<!-- ![Robotic Arm Final Path]({{site.baseurl}}/assets/img/robot_arm_final.png) -->
