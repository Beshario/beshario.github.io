---
layout: post
title: Where Am I
subtitle: Robotics Localization Project
gh-repo: Beshario/Udacity-Robotics-Perception-Challenge/
gh-badge: [star, fork, follow]
# cover-img: /assets/img/path.jpg
thumbnail-img: /assets/img/WHEREAMI/3.png
tags: [education, robotics, Udacity]
comments: true
---
Two robots localizing itself in a know map using ROS and Gazebo

### INTRODUCTION

Two robots configurations were made to test against each other in localization and path planning.
The circular robot is mine adn the rectangular robot model is provided by Udacity.


<p align="center">
  <img src="/assets/img/WHEREAMI/circ robot model.png">
</p>

<p align="center">
  <img src="/assets/img/WHEREAMI/udacitybot.png">
</p>

Some of the performance results are shown below:

At the start the robot is not localized. Therefore the monte carlo alogrithm is used to localize the robot. The particles are generated randomly and the robot is moved around the map. The particles are then weighted based on the sensor readings and the particles are resampled. The process is repeated until the robot is localized. This can be show in the last image.


<p align="center">
  <img src="/assets/img/WHEREAMI/start.png">
</p>

<p align="center">
  <img src="/assets/img/WHEREAMI/2.png">
</p>

<p align="center">
  <img src="/assets/img/WHEREAMI/3.png">
</p>


The final localization results from both robots are shown below:

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