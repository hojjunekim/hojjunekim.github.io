---
layout: page
title: Modeling and Making Multimodal Sensor system
affiliation: Robust Perception and Mobile Robotics Lab. SNU
position: Undergraduate Researcher
description: System Design and Manufacture, Multi-sensor Calibration
project_year: 2023
img: /assets/img/projects/handheld/handheld_real.png
# video: 
category: rpm
---

To implement Simultaneous Localization and Mapping (SLAM), a technology that estimates the position and constructs a map of the surrounding environment, various sensors are utilized. These include Stereo Cameras, LiDAR, thermal cameras, IMUs, GPS, among others. While outdoor scenarios can involve attaching these sensors to vehicles or robots for data acquisition, indoor environments pose challenges due to complexity. As a result, I conducted work in Professor Ayoung Kim's RPM Laboratory at Seoul National University's Department of Mechanical Engineering to design and create a handheld multimodal sensor system for Long-term Localization, enabling convenient data acquisition and localization indoors.

Using Solidworks 3D CAD, I designed a structure that allows easy portability of several sensors, a PC, and batteries. This structure was then fabricated using a 3D printer. The list of devices used is as follows:

- Sensors
    
    LiDAR: LIVOX Mid-70
    
    RGB: intel realsense d455
    
    LWIR: FLIR boson(stereo)
    
    GNSS: Ublox zed-f9p + Tallysman TW8889
    
    PC: intel NUC 11
    
    Peripherals: 480*800 LCD monitor, USB hub
    

Based on the ROS1 framework, I connected various sensors to test the functionality of basic SLAM algorithms. Currently, I am in the process of implementing DSO-based Direct SLAM using a thermal camera and LiDAR with the constructed handheld multimodal sensor system. I have applied an algorithm that estimates depth from mono RGB camera to thermal 8-bit images. Additionally, I have modified the system to directly receive depth from LiDAR data. This modification aims to enable data acquisition and SLAM processing both indoors and outdoors, day and night.

<div class="figure">
    <img class="one" src="{{ site.baseurl }}/assets/img/projects/handheld/handheld_cad.png" alt="" title="cad"/>
    <img class="one" src="{{ site.baseurl }}/assets/img/projects/handheld/handheld_real.png" alt="" title="real"/>
</div>

<div class="figure">
    <img class="two" src="{{ site.baseurl }}/assets/img/projects/handheld/handheld_demo.mp4" alt="" title="demo"/>
</div>