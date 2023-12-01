---
layout: post
title: The Evolution of My First Robot
subtitle: A Tale of Trials, Triumphs, and Technical Growth
thumbnail-img: /assets/img/robot1/robot+besh.jpg

tags: [project, robotics]
comments: true
---

## Introduction

Ever since my high school days in a robotics competition, the idea of **applying physics to create** something phenomenal has captivated me. This led to my dream: **building a robot**. Not just a machine, but a **companion** that understands the nuances of life.

## The Inspiration

Post-layoff, I found myself with time - the most valuable resource. It was the perfect opportunity to bring my dream to life: **making my own robot**. It was about learning and establishing a **testing ground** for new ideas.

## Early Decisions and Designs
<!-- add photo -->
![electronicParts](/assets/img/robot1/parts.jpg)
Starting with an idea to use components around me, hey if I cannot make a robot from a everyday diy components, who am I? With a friend of mine, we set out to test autonomy and motor control. The plan? A drivetrain with open loop stepper motors controlled by an **Arduino Uno board**, a motor driver hat, and a **Raspberry Pi** as a master. 

## Relevant links
[Onshape](https://cad.onshape.com/documents/3f70f4d1c3a2c5a8e45bfeff/w/4827bc6d187c9f5d1b09020b/e/4e4859beb36756ea167cbd20)
[github](https://github.com/zBeshTech/Assembled)

## Challenges with Everyday Components

The challenge was immediate. My parts were **limited**: stepper motors without encoders, no lidar, and an open-loop system. The need for the right equipment became glaringly apparent. However, I was able to teleoperate the robot, and also have it follow a open loop paths that was fascinating for me to see. [You can find some of the robot model C++ code here](https://github.com/zBeshTech/Assembled/tree/main/src/assembled/src)

![assembledRobot](/assets/img/robot1/assembled.jpg)
## Realization and Shift in Strategy

I faced a choice: continue with a limiting design or start afresh with a better solution. I chose the latter, focusing on **ROS2** - the current industry standard.

<!-- add a video content from youtube -->
<iframe class="d-block mx-auto" width="560" height="315" src="https://www.youtube.com/embed/p47VkIIDmBo?si=g9rIYxXNZuWXkphq" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

![assembledRobot](/assets/img/robot1/onshapeRobotAssembled.png)

## Research and Component Selection

Back to the drawing board, I broke down the robot's systems. My focus was on **seamless integration** and **minimizing components**. I browsed through various projects to understand what worked for others.

## Building and Testing the Robot

The second version of my robot is underway. With a **modular design** in mind, it's evolving beyond my initial concept. This version boasts a DC motor with an encoder, an IMU, and a power bank.

## Reflections and Future Directions

Though still in progress, this journey has been an invaluable learning curve in **robotics and mechatronics**. It's a stepping stone to many more modular robot designs, aiming to **empower makers**.

## Conclusion

This experience has taught me that picking the right components from the start is very important, and gets more expensive as the product advances in development.

