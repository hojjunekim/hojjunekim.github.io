---
layout: page
title: Display Virtual Cubes on Your Desk!
description: SE3, optical flow, RANSAC
img: assets/img/ARcube/demo.png
importance: 3
category: fun
---

Developed a program to display a 3D cube on a desk. You can click a point to place the cubes, and the cube will be placed on your video. RANSAC, SE3 explanation, Newton's method optimization and optical flow techniques are used. Developed with C++ and codes are uploaded in github.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/ARcube/ransac.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/ARcube/plane.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/ARcube/plan.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    plane detection via RANSAC
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/ARcube/optical_flow.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    This image can also have a caption. It's like magic.
</div>

You can see demo video.

<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include video.html path="assets/img/ARcube/demo.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
    </div>
</div>
<div class="caption">
    Demo video
</div>
