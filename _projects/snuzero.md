---
layout: page
title: International Student Car Competition-Autonomous Driving
description: a project with a background image and giscus comments
img: assets/img/snuzero/zero.jpg
importance: 2
category: work
giscus_comments: true
---

I participated in the Autonomous Driving Car category of the International Student Autonomous Vehicle Competition organized by the Ministry of Land, Infrastructure and Transport, as a member of the SNU ZERO autonomous driving club at Seoul National University. The competition involved performing tasks such as driving, parking, delivery, and obstacle detection using the ERP-42 platform.

Within the SNU ZERO team, we divided our efforts into three teams: Path Planning, Vision, and Sensor Fusion. I belonged to the Sensor Fusion team, where I was responsible for handling GPS, IMU, Lidar, and camera sensors using the ROS1 framework. This involved tasks such as recognizing the car's orientation, movement, and understanding the surrounding environment. Additionally, I collaborated closely with other teams to discuss improved path planning algorithms, considering sensor-specific errors. We optimized data structures for the RRT* algorithm and engaged in detailed collaboration with other teams.

The competition took place at K-City, the world's largest test bed for autonomous vehicles, under the Ministry of Land, Infrastructure and Transport. For six months, we worked tirelessly at the Future Mobility Testing Center (FMTC) located at Seoul National University's Siheung campus, and during vacations, we commuted daily to prepare. We accomplished a variety of tasks, including recognizing and clustering cones using Lidar and cameras for cone navigation, avoiding dynamic and static obstacles, and lane recognition to correct heading orientation errors. As a result, we secured the first place in the preliminary cone navigation round and ultimately achieved a gold medal. You can watch our team's driving video in the link below.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/snuzero/zero.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    This image can also have a caption. It's like magic.
</div>

You can see demo video.

<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include video.html path="assets/img/snuzero/zero_cone.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
    </div>
</div>
<div class="caption">
    A simple, elegant caption looks good between video rows, after each row, or doesn't have to be there at all.
</div>


<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include video.html path="https://youtu.be/o3ppXvRwUdw?t=3977" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
