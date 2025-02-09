---
layout: post
title: a Contribution to DexHand
subtitle: Hour by hour building Moveit package and ros control for a humanoid hand
thumbnail-img: /assets/img/dexhand/dexHand.png

tags: [project, robotics]
comments: true
---

## Introductiozn

With time and resources and an interesting project I liked, I decided to reach out to the owner, to offer Moveit contribution of controlling the Hand.
Trent Shumay was working on the firmware side, while I contributed from higher level, the Moveit2 side. while the code was not integrated to [DexHand1](https://www.dexhand.org), it paved the way for dexHand2 Moveit2 integration.

This blog post documents the work produced as the DexHand1 project is sunsetted , but you can follow [DexHand](https://x.com/dexhandv2)

## Activites:

General literature review of available common hands from a control standpoint, such as shadow hand, chunk hand and leap hand.
I got to run dex hand package and make a moveit package to control the robot through joint state.
I also cleaned up some of the URDF, the control produced, which can be found in [github](Github: https://github.com/Beshario/dexhand_control)  control the finger chain one at a time, but it can be done in parallel.  
I have attached the prep work here
[investigationDocument](/assets/PDF/Moveit Config interface investigationDocument.pdf)

This is the end result

[![Everything Is AWESOME](https://img.youtube.com/vi/SxgqUeM372U/0.jpg)](https://www.youtube.com/watch?v=SxgqUeM372U "DexhandControlPackage")

## Conclusion:
During this journey I had the pleasure with working alongside smart people. I also learnt even open source projects require dedication and commitment. In addition, there is a need to connect like minded people on projects together. 