---
layout: page
title: Organized Autonomous RC car competition for 200+ Students Nationwide
affiliation: AI Tech Play, non-profit organization for AI education
position: Hardware Team Leader
description: System Design and Manufacture, Motor Control, Software Implementation
project_year: 2021
img: /assets/img/projects/AI-tech/car.png
youtube: https://www.youtube.com/channel/UCfmSTxHQ6Y43XtHsQ7l_H3Q
html: https://outta.ai/en
category: club
---

A group of engineering enthusiasts, driven by a sincere passion for the field, came together to establish the AI TechPlay organization. The objective was to share engineering knowledge widely among students. With the aim of creating an avenue for firsthand experiences in engineering, we designed a program targeting middle school students nationwide. This program aimed to offer them a free opportunity to experience autonomous driving technology and coding, culminating in a linked coding competition. Inspired by the autonomous driving RC-car competition held annually at MIT, we sought to provide students with the opportunity to code autonomous driving algorithms, simulate them, and run the code on an actual RC-car, offering a real-world testing platform.

I took on the role of the Car Assemble Team Leader, responsible for modifying the code-controllable RC-car. My focus was on various hardware aspects. This involved integrating control board PWM, inertial sensors, lidar, RGB-D cameras, and other sensors onto a Jetson Nano board using the ROS2 framework. We essentially stripped down all components of the existing RC-car except the wheels and chassis, then reassembled and transformed it. This required the reconstruction of not only ADAS sensors but also the entire system, from motors to communication, enabling control via code and wireless controller. We adapted existing MIT autonomous driving code to our new platform, making necessary parameter changes due to the hardware differences and optimizing code execution speed.

As a result, the Autonomous Driving Mini Car AI Coding Experience and Competition saw the participation of over 200 middle school students from across the nation, successfully concluding the initiative. The competition process can be observed in the YouTube link provided below.

[**Youtube**](https://www.youtube.com/channel/UCfmSTxHQ6Y43XtHsQ7l_H3Q), [**Facebook**](https://www.facebook.com/aitechplay/)

<div class="row">
    <img class="one" src="{{ site.baseurl }}/assets/img/projects/AI-tech/car.png" alt="" title="RC car"/>
    <img class="one" src="{{ site.baseurl }}/assets/img/projects/AI-tech/map.png" alt="" title="map"/>
    <img class="one" src="{{ site.baseurl }}/assets/img/projects/AI-tech/poster.png" alt="" title="poster"/>
</div>
