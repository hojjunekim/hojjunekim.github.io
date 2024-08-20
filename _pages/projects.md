---
layout: page
title: Projects
permalink: /projects/
description: A collection of projects during my studies.
---

{% for project in site.projects %}

{% if project.redirect %}
<div class="project">
    <div class="thumbnail">
        <a href="{{ project.redirect }}" target="_blank">
        {% if project.img %}
        <img class="thumbnail" src="{{ project.img | prepend: site.baseurl | prepend: site.url }}"/>
        {% else %}
        <div class="thumbnail blankbox"></div>
        {% endif %}    
        <span>
            <h1>{{ project.title }}</h1>
            <br/>
            <p>{{ project.description }}</p>
        </span>
        </a>
    </div>
</div>
{% else %}

<div class="project ">
    <div class="thumbnail">
        <a href="{{ project.url | prepend: site.baseurl | prepend: site.url }}">
        {% if project.img %}
        <img class="thumbnail" src="{{ project.img | prepend: site.baseurl | prepend: site.url }}"/>
        {% else %}
        <div class="thumbnail blankbox"></div>
        {% endif %}    
        <span>
            <h1>{{ project.title }}</h1>
            <br/>
            <p>{{ project.description }}</p>
        </span>
        </a>
    </div>
</div>

{% endif %}

{% endfor %}

<div style="clear: both;"></div> 

##### At ETH Zurich

* Gaussian Belief Propagation for Continuous Time Bundle Adjustment
* Crowd navigation with LiDAR via Teacher-Student Reinforcement Learning in Orbit(Isaac-Sim)

<!-- * Using Semantics to detect Camera Miscalibrations
* Multi-camera DeepTAM ([report](/assets/documents/projects/Multicam_Deeptam.pdf), [code](https://github.com/surirohit/multi-camera-deeptam))
* Verification of Neural Networks using Linear Programming ([report](/assets/documents/projects/RIAI_Manuel_Mayank.pdf), [code](https://github.com/Mayankm96/verify_neural_networks))
* Monocular Odometry with Bundle Adjustment ([report](/assets/documents/projects/VA4MR_Mini_Project.pdf), [video](https://www.youtube.com/watch?v=trbBh8Rjc4s&feature=youtu.be), [code](https://github.com/Mayankm96/Mono-Odometry)) -->

##### At SNU

* 2D Odometry with only mmWave Radar via Two-way ICP
* EKF Localization and Obstacle Detection in Autonomous Driving Car
* Auto Landing via Bézier curve in Autonomous Flight Quadrotor
* Fault Tolerant Control in Quadrotor with Sliding Mode/Backsteppping Control
* Thermal camera and LiDAR fusion Direct SLAM modified from DSO
* Analysis of LiDAR SLAM in long term localization

<!-- * Survey on Variational Autoencoders for Bayesian Inference ([report](/assets/documents/projects/cs698-report.pdf))
* Multi- Robot System for Bomb Disposal ([poster](/assets/documents/projects/Abhyast_Plan.jpg), [code](https://github.com/Boeing-Abhyast/Phase-VII))
* Visual Odometry using careful Feature Selection and Tracking ([report](/assets/documents/projects/ee698-report.pdf), [code](https://github.com/Mayankm96/Stereo-Odometry-SOFT))
* MATLAB based GUI for Motion Planning ([code](https://github.com/Mayankm96/Motion-Planning-GUI))
* Failure Handling in Swarm of Quadrotors ([report](/assets/documents/projects/cs637-report.pdf)) -->

<!-- ### open source projects

* ROS package for AirSim simulator- in C++ ([code](https://github.com/Mayankm96/airsim_img_publisher))
* ROS package for AirSim simulator- in Python ([code](https://github.com/Mayankm96/airsim_ros_client))
* ROS package for saving data published from Zed Camera ([code](https://github.com/Mayankm96/extract_zed_data))
* ROS package for publishing data from Sparton AHRS8 sensor ([code](https://github.com/Mayankm96/sparton_ahrs8_driver))
* Python project for reinforcement learning with Trifinger robot [code](https://github.com/pairlab/leibnizgym/) -->
