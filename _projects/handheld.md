---
layout: page
title: Modeling Multimodal Sensor system for Long-term Localization
description: a project with a background image
img: assets/img/handheld/handheld_real.png
importance: 1
category: work
giscus_comments: true
# related_publications: einstein1956investigations, einstein1950meaning
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

    ---
    layout: page
    title: project
    description: a project with a background image
    img: /assets/img/12.jpg
    ---

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/handheld/handheld.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/handheld/handheld_cad.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/handheld/handheld_real.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Caption photos easily. On the left, a road goes through a tunnel. Middle, leaves artistically fall in a hipster photoshoot. Right, in another hipster photoshoot, a lumberjack grasps a handful of pine needles.
</div>

You can see the demo video.

<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include video.html path="assets/img/handheld/handheld_demo.mov" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
    </div>
</div>
<div class="caption">
    A simple, elegant caption looks good between video rows, after each row, or doesn't have to be there at all.
</div>