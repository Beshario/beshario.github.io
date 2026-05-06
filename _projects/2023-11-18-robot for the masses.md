---
layout: post
title: Modular Robot Platform
subtitle: An Open-Source, Accessible ROS2 Mobile Robot
thumbnail-img: /assets/img/robotMasses.png
tags: [robotics, ROS2, open-source, AMR, hardware]
comments: true
---

An ongoing project to build a well-documented, modular mobile robot that anyone can replicate. The goal is to close the gap in open-source robotics projects that are often incomplete, undocumented, or difficult to source components for.

### The Problem

Most open-source robot projects lack one or more of the following:
- Complete, working software (not just demos)
- Reproducible hardware with sourcing guidance
- Docker containers or environment setup for ROS
- Clear documentation for getting from zero to running

### The Approach

Building a mobile robot platform iteratively, starting from basic motor control and working toward full ROS2 autonomy. Each stage is documented and designed to be reproducible.

![first robot attempt](/assets/img/robot1/assembled.jpg)

Hardware currently includes DC motors with encoders, an IMU, and a Raspberry Pi running ROS2. The design is modular to allow sensor and compute upgrades without a full rebuild.
