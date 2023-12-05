---
layout: page
title: Lidar-Inertial Odometry
description: Faster-LIO & Fast-LIO2, evaluation, ROS1
img: assets/img/handheld/LIO.png
importance: 2
category: work
giscus_comments: true
# related_publications: einstein1956investigations, einstein1950meaning
---

To compare two LIO algorhithms Faster-LIO and Fast-LIO2, I implemented those in MULRAN dataset and complex-urban dataset from KAIST IRAP lab. Evaluated the algorithms by plotting the trajectory by evo library.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/LIO/urban.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/LIO/mulran.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/LIO/faster1.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Faster-LIO tested with indoor dataset taken by our Livox-mid360
</div>
