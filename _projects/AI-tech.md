---
layout: page
title: Autonomous Driving RC-car making
description: a project that redirects to another website
img: assets/img/7.jpg
# redirect: https://unsplash.com
importance: 3
category: work
---

A group of engineering enthusiasts, driven by a sincere passion for the field, came together to establish the AI TechPlay organization. The objective was to share engineering knowledge widely among students. With the aim of creating an avenue for firsthand experiences in engineering, we designed a program targeting middle school students nationwide. This program aimed to offer them a free opportunity to experience autonomous driving technology and coding, culminating in a linked coding competition. Inspired by the autonomous driving RC-car competition held annually at MIT, we sought to provide students with the opportunity to code autonomous driving algorithms, simulate them, and run the code on an actual RC-car, offering a real-world testing platform.

I took on the role of the Car Assemble Team Leader, responsible for modifying the code-controllable RC-car. My focus was on various hardware aspects. This involved integrating control board PWM, inertial sensors, lidar, RGB-D cameras, and other sensors onto a Jetson Nano board using the ROS2 framework. We essentially stripped down all components of the existing RC-car except the wheels and chassis, then reassembled and transformed it. This required the reconstruction of not only ADAS sensors but also the entire system, from motors to communication, enabling control via code and wireless controller. We adapted existing MIT autonomous driving code to our new platform, making necessary parameter changes due to the hardware differences and optimizing code execution speed.

As a result, the Autonomous Driving Mini Car AI Coding Experience and Competition saw the participation of over 200 middle school students from across the nation, successfully concluding the initiative. The competition process can be observed in the YouTube link provided below.

[AI Tech Play](https://www.youtube.com/channel/UCfmSTxHQ6Y43XtHsQ7l_H3Q)

[AI Tech Play](https://www.facebook.com/aitechplay/)


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
