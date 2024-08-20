---
layout: page
title: Thermal camera & Lidar Direct SLAM 
description: Direct SLAM, visual-lidar SLAM
img: /assets/img/projects/TLslam/result.png
importance: 3
category: rpm
---

I have implemented Thermal-Lidar Direct SLAM by integrating thermal camera images and Lidar information using the Direct Sparse Odometry (DSO) algorithm, which was originally developed for mono RGB cameras. During the initialization phase, I selected points within the projected region of Lidar-observed points in the image and provided actual depth information obtained from Lidar measurements. The results showed a significant improvement in scale error when fusing Lidar information, compared to using only thermal camera images with range scaling in the DSO algorithm. This was particularly important as the scale error was notably reduced with the incorporation of Lidar data.

To apply this algorithm to the multimodal handheld system that I personally developed, I conducted intrinsic calibration for the thermal camera and extrinsic calibration between the thermal camera and Lidar using various methods. Additionally, I generated AR tags visible to the thermal camera to experiment with a new calibration approach. This ongoing effort is aimed at ensuring the effectiveness of the algorithm within the practical setup of the multimodal handheld system.

<div class="figure">
    <img height="50%" width="50%" src="{{ site.baseurl }}/assets/img/projects/TLslam/init.png" alt="" title="init"/>
</div>