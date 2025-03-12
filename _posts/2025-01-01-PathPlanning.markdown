---
layout: post
title: RRT Path Planning for Robot Navigation
date: 2025-03-12 12:00:00
description: Implementation of Rapidly-exploring Random Tree (RRT) and RRT* algorithms for efficient robot path planning with collision avoidance in complex environments.
img: rrt_planning.png # Add image post (optional)
fig-caption: Robot Path Planning using RRT and RRT*
tags: [Robotics, Path Planning, RRT, RRT*, Collision Avoidance, Motion Planning]
---

This project implements **Rapidly-exploring Random Tree (RRT)** and its optimized variant **RRT*** algorithms for robot path planning in complex environments. The system enables a mobile robot to autonomously navigate from a starting position to a goal while avoiding obstacles in maps of varying complexity.

## Section 1: **Path Planning with RRT**

The standard RRT algorithm was implemented to find feasible paths through complex environments:

- **Random Sampling**: The algorithm randomly samples points in the configuration space to explore the environment efficiently.
- **Tree Expansion**: From the nearest node in the tree, the algorithm attempts to expand toward the sampled point.
- **Collision Detection**: Implemented an efficient collision checking system using precomputed collision maps to speed up the planning process.

![RRT Path Planning Expansion]({{site.baseurl}}/assets/img/rrt_expansion.png)
<img src="{{site.baseurl}}/assets/img/pathplanning_rrt.png" alt="RRT Tree Expansion" style="width:50%;" />

The standard RRT algorithm provides rapid exploration of the configuration space and finds feasible paths quickly, but these paths are typically not optimal in terms of distance or smoothness.

## Section 2: **Optimal Path Planning with RRT***

The RRT* algorithm improves upon standard RRT by continuously optimizing the tree structure:

- **Near-Optimal Paths**: RRT* converges to the optimal path as the number of iterations increases.
- **Tree Rewiring**: After adding a new node, nearby nodes are checked to see if connecting through the new node would reduce their cost.
- **Dynamic Ball Radius**: The algorithm dynamically adjusts the search radius based on the number of nodes in the tree.

<img src="{{site.baseurl}}/assets/img/pathplannning_rrtstar.png" alt="RRT* Rewiring Process" style="width:50%;" />

The implementation includes:
- Efficient neighbor searching within a dynamically calculated radius
- Path cost optimization through tree rewiring
- Smooth trajectory generation between nodes

## Environment Representation

The system works with different environment maps:

- **Occupancy Grid Maps**: Loaded from image files with configurable resolution.
- **Precomputed Collision Maps**: Generated to accelerate collision checking during planning.
- **Map Bounds**: Automatic detection and enforcement of navigable areas.

<img src="{{site.baseurl}}/assets/img/map_representation.png" alt="Map Representation" style="width:40%;" />

## Robot Kinematics and Simulation

The planner accounts for the robot's kinematic constraints:

- **Unicycle Model**: The robot follows a unicycle motion model with controllable linear and angular velocities.
- **Motion Simulation**: Realistic trajectory prediction based on velocity and steering commands.
- **Collision Footprint**: Circular robot footprint used for collision checking.

## Results and Performance

The implementation was tested on multiple environments:

- **Willow Garage Map**: A complex office environment with narrow corridors and multiple rooms.
- **MyHal Map**: A simple environment with various obstacles and open spaces.


Performance metrics:
- RRT* consistently produced shorter, smoother paths compared to standard RRT
- Collision checking optimization resulted in significant performance improvements
- The system successfully navigated through complex environments with narrow passages

<video width="90%" controls>
  <source src="{{site.baseurl}}/assets/img/pathplanning_sim.webm" type="video/webm">
  Your browser does not support the video tag.
</video>

## Implementation Details

The system was implemented in Python with the following key components:

- **Map Processing**: Tools for loading and processing occupancy grid maps
- **Collision Detection**: Efficient collision checking using precomputed maps
- **Visualization**: Real-time visualization of the planning process using Pygame
- **Path Recovery**: Extraction of the final path from the constructed tree

This project demonstrates expertise in:
- **Sampling-based planning algorithms**
- **Robot motion planning and control**
- **Collision detection and avoidance**
- **Path optimization techniques**
