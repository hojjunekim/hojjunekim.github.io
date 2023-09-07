---
layout: page
title: International Student Car Competition-Autonomous Driving
description: a project with a background image and giscus comments
img: assets/img/zero.jpg
importance: 2
category: work
giscus_comments: true
---

I participated in the Autonomous Driving Car category of the International Student Autonomous Vehicle Competition organized by the Ministry of Land, Infrastructure and Transport, as a member of the SNU ZERO autonomous driving club at Seoul National University. The competition involved performing tasks such as driving, parking, delivery, and obstacle detection using the ERP-42 platform.

Within the SNU ZERO team, we divided our efforts into three teams: Path Planning, Vision, and Sensor Fusion. I belonged to the Sensor Fusion team, where I was responsible for handling GPS, IMU, Lidar, and camera sensors using the ROS1 framework. This involved tasks such as recognizing the car's orientation, movement, and understanding the surrounding environment. Additionally, I collaborated closely with other teams to discuss improved path planning algorithms, considering sensor-specific errors. We optimized data structures for the RRT* algorithm and engaged in detailed collaboration with other teams.

The competition took place at K-City, the world's largest test bed for autonomous vehicles, under the Ministry of Land, Infrastructure and Transport. For six months, we worked tirelessly at the Future Mobility Testing Center (FMTC) located at Seoul National University's Siheung campus, and during vacations, we commuted daily to prepare. We accomplished a variety of tasks, including recognizing and clustering cones using Lidar and cameras for cone navigation, avoiding dynamic and static obstacles, and lane recognition to correct heading orientation errors. As a result, we secured the first place in the preliminary cone navigation round and ultimately achieved a gold medal. You can watch our team's driving video in the link below.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/1.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/3.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/5.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Caption photos easily. On the left, a road goes through a tunnel. Middle, leaves artistically fall in a hipster photoshoot. Right, in another hipster photoshoot, a lumberjack grasps a handful of pine needles.
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/5.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    This image can also have a caption. It's like magic.
</div>

You can also put regular text between your rows of images.
Say you wanted to write a little bit about your project before you posted the rest of the images.
You describe how you toiled, sweated, *bled* for your project, and then... you reveal its glory in the next row of images.


<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.html path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    You can also have artistically styled 2/3 + 1/3 images, like these.
</div>


The code is simple.
Just wrap your images with `<div class="col-sm">` and place them inside `<div class="row">` (read more about the <a href="https://getbootstrap.com/docs/4.4/layout/grid/">Bootstrap Grid</a> system).
To make images responsive, add `img-fluid` class to each; for rounded corners and shadows use `rounded` and `z-depth-1` classes.
Here's the code for the last row of images above:

{% raw %}
```html
<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.html path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
```
{% endraw %}
