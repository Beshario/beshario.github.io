---
layout: post
title: Where Am I
subtitle: Robot Localization with AMCL in ROS and Gazebo
gh-repo: Beshario/Udacity-Robotics-Perception-Challenge/
gh-badge: [star, fork, follow]
thumbnail-img: /assets/img/WHEREAMI/3.png
tags: [robotics, localization, AMCL, ROS, Gazebo, education, Udacity]
comments: true
---

Two robot configurations tested against each other for localization and path planning in a known map using ROS and Gazebo. The circular robot is a custom design; the rectangular model is provided by Udacity.

<p align="center">
  <img src="/assets/img/WHEREAMI/circ robot model.png">
</p>

<p align="center">
  <img src="/assets/img/WHEREAMI/udacitybot.png">
</p>

Monte Carlo Localization (AMCL) is used to localize each robot. Particles are generated randomly, weighted against sensor readings, and resampled iteratively until the robot converges on its position in the map.

<p align="center">
  <img src="/assets/img/WHEREAMI/start.png">
</p>

<p align="center">
  <img src="/assets/img/WHEREAMI/2.png">
</p>

<p align="center">
  <img src="/assets/img/WHEREAMI/3.png">
</p>

Final localization results for both robots:

<p align="center">
  <img src="/assets/img/WHEREAMI/final%20udacity%20bot.png">
</p>

<p align="center">
  <img src="/assets/img/WHEREAMI/lastCircleBotPic.png">
</p>

### Final Report

<object data="/assets/img/WHEREAMI/Localization_reportpdf.pdf" type="application/pdf" width="700px" height="700px">
    <embed src="/assets/img/WHEREAMI/Localization_reportpdf.pdf">
        <p>This browser does not support PDFs. Please download the PDF to view it: <a href="/assets/img/WHEREAMI/Localization_reportpdf.pdf">Download Report</a>.</p>
    </embed>
</object>
