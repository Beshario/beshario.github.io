---
layout: post
title: Building My First Autonomous Robot
subtitle: Iterating from Arduino and Steppers to a ROS2 Mobile Platform
thumbnail-img: /assets/img/robot1/robot+besh.jpg
tags: [project, robotics, ROS2, Arduino, autonomy]
comments: true
---

## Introduction

Building a fully autonomous robot from scratch has been a long-term goal: a personal testing ground for ideas in navigation, perception, and control outside of a work context.

## Early Decisions and Designs

![electronicParts](/assets/img/robot1/parts.jpg)

Starting with components on hand, the first version used a drivetrain with open-loop stepper motors controlled by an Arduino Uno and motor driver hat, with a Raspberry Pi as master. Built alongside a friend to test basic autonomy and motor control.

**Relevant links:**
- [OnShape CAD Model](https://cad.onshape.com/documents/3f70f4d1c3a2c5a8e45bfeff/w/4827bc6d187c9f5d1b09020b/e/4e4859beb36756ea167cbd20)
- [GitHub Repository](https://github.com/zBeshTech/Assembled)

## Challenges with Open-Loop Hardware

The constraints were immediate: stepper motors without encoders, no LiDAR, and no feedback loop. Still managed to teleoperate the robot and run open-loop paths.

[Robot model C++ code](https://github.com/zBeshTech/Assembled/tree/main/src/assembled/src)

![assembledRobot](/assets/img/robot1/assembled.jpg)

## Shift to ROS2

Rather than patch the first design, I restarted with ROS2 as the foundation, the current industry standard for autonomous mobile robotics.

<iframe class="d-block mx-auto" width="560" height="315" src="https://www.youtube.com/embed/p47VkIIDmBo?si=g9rIYxXNZuWXkphq" title="First Robot Build" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

![assembledRobot](/assets/img/robot1/onshapeRobotAssembled.png)

## Second Version

The second version is modular by design, built around DC motors with encoders, an IMU, and a power bank. The focus was on minimizing components while enabling proper closed-loop control and sensor integration.

## Takeaways

Component selection early in development has an outsized impact on the trajectory of the project. Getting the sensing and actuation right from the start avoids expensive redesigns downstream.
