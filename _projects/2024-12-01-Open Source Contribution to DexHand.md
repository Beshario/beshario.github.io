---
layout: post
title: Open Source Contribution to DexHand
subtitle: Building a ROS2 MoveIt2 Control Package for a Humanoid Robotic Hand
thumbnail-img: /assets/img/dexhand/dexHand.png
tags: [robotics, ROS2, MoveIt2, open-source, manipulation, URDF]
comments: true
---

Contributed to the [DexHand](https://www.dexhand.org) project by building the ROS2 MoveIt2 control package for the humanoid hand. Trent Shumay led firmware development; this contribution covered the higher-level motion planning and control stack. While the code was not merged into DexHand1 before the project was sunsetted, it informed the MoveIt2 integration direction for DexHand2.

Follow [DexHand](https://x.com/dexhandv2) for the current project.

### Work Done

- Literature review of common robotic hand control approaches: Shadow Hand, Chunk Hand, and Leap Hand
- Built and ran the existing DexHand ROS package
- Created a MoveIt2 package to control the hand through joint state commands
- Cleaned up URDF and controller configuration
- Implemented per-finger chain control with parallel execution support

[GitHub Repository](https://github.com/Beshario/dexhand_control)

[Investigation Document](/assets/PDF/Moveit Config interface investigationDocument.pdf)

### Demo

Click the image to watch the MoveIt2 control demo:

[![DexHand MOVEIT2 Demo](https://img.youtube.com/vi/SxgqUeM372U/0.jpg)](https://www.youtube.com/watch?v=SxgqUeM372U "DexHand Control Package")
