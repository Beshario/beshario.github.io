---
layout: post
title: Robotic Arm Pick and Place
subtitle: Forward and Inverse Kinematics for a Kuka KR210 in Gazebo
gh-repo: Beshario/Robotic-Arm-Pick-and-Place
gh-badge: [star, fork, follow]
thumbnail-img: /assets/img/Robot-Arm/F210.png
tags: [robotics, ROS, Gazebo, kinematics, Kuka, education, Udacity]
comments: true
---

Programmed a [Kuka KR210](https://www.kuka.com/en-us/products/robotics-systems/industrial-robots/kr-210-2-f-exclusive) 6-DoF serial manipulator in [Gazebo](http://gazebosim.org/#features) to pick a cylinder from a randomized shelf position and drop it into a bin.

![Robotic arm in front of a shelf](/assets/img/Robot-Arm/F210.png)

### Kinematic Analysis

Derived the DH parameter table from the KR210 URDF and built individual transformation matrices for each joint in Python using SymPy.

DH parameter reference frame:

![dh parameter reference frame](https://user-images.githubusercontent.com/6395647/30779703-9bb8ff02-a0c5-11e7-8cc0-52bacc8e6bea.jpeg)

| Links | alpha(i-1) | a(i-1) | d(i) | theta(i) |
|---|---|---|---|---|
| 0->1 | 0 | 0 | 0.75 | q1 |
| 1->2 | -pi/2 | 0.35 | 0 | -pi/2 + q2 |
| 2->3 | 0 | 1.25 | 0 | q3 |
| 3->4 | -pi/2 | 0 | 1.5 | q4 |
| 4->5 | pi/2 | 0 | 0 | q5 |
| 5->6 | -pi/2 | 0 | 0 | q6 |
| 6->EE | 0 | 0 | 0.303 | 0 |

### Inverse Kinematics

The KR210 has a spherical wrist (joints 4, 5, 6 intersect at joint 5), enabling a closed-form IK solution. The first three joints position the wrist center; the last three orient the end-effector.

![ik](https://user-images.githubusercontent.com/6395647/30779765-8266aa7a-a0c7-11e7-871c-4d21910fac6f.png)
