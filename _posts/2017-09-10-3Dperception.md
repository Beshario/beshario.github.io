---
layout: post
title: PR2 3D Perception
subtitle: Point Cloud Segmentation and Object Recognition with an RGB-D Camera
gh-repo: Beshario/Udacity-Robotics-Perception-Challenge/
gh-badge: [star, fork, follow]
thumbnail-img: /assets/img/3Dperception/perceptionchallenge.png
tags: [robotics, perception, point-cloud, ROS, computer-vision, education, Udacity]
comments: true
---

Perception pipeline for a PR2 robot using an RGB-D camera: filter raw point cloud data, segment objects, and classify them using a trained SVM model.

![demo-1](https://user-images.githubusercontent.com/20687560/28748231-46b5b912-7467-11e7-8778-3095172b7b19.png)

### Filtering

Raw point cloud data goes through three filters before segmentation:

**Statistical Outlier Removal** — removes noise points whose mean neighbor distance falls outside a defined standard deviation threshold (k=20, stddev=0.1).

**Voxel Grid Downsampling** — reduces point density by averaging points within each voxel (leaf size 0.01m), keeping enough detail for recognition while reducing compute load.

**Passthrough Filter** — crops the scene to a region of interest along Y (-0.4 to 0.4) and Z (0.6 to 0.9) axes, focusing the robot on the tabletop.

**RANSAC Plane Segmentation** — separates the table surface (inliers) from objects (outliers) using a max distance of 0.01m.

### Clustering

Used DBSCAN (Euclidean clustering) on a KD-tree representation of the point cloud. DBSCAN does not require a predefined number of clusters, making it well suited for unknown table arrangements.

### Object Recognition

Each cluster's color and surface normal histograms are extracted and matched against a trained SVM model (linear kernel, C=0.1). Training used 20–40 random poses per object per scene.

Object identification accuracy: **97%**

#### Test Scenes

![Test 1 object recognition](https://user-images.githubusercontent.com/6395647/31702880-c657ab38-b3a7-11e7-97cc-4d396134cdf2.png)

![Test 2 object recognition](https://user-images.githubusercontent.com/6395647/31702878-c63ce334-b3a7-11e7-808d-b7b6ed1ee663.png)

![Test 3 object recognition](https://user-images.githubusercontent.com/6395647/31704684-60f67fc2-b3b0-11e7-9f35-b72b70f6d3b1.jpeg)
