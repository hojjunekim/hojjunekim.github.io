---
layout: page
title: Real-time flood monitoring system by water detection using Sentinel-1 satellite image
description: another without an image
img: assets/img/satgeo/all_result.png
importance: 4
category: fun
---

During my time as an undergraduate research intern at the Earth and Planetary Physics Laboratory, Seoul National University, under the guidance of Professor Deokjin Kim, I conducted a comprehensive study for a duration of 11 months focused on establishing a real-time disaster monitoring system. The primary objective was to create a system that utilizes periodically acquired satellite imagery to enable nationwide real-time monitoring, particularly for disaster events like floods and wildfires.

Specifically, my research centered on the development of a system that employs Semantic Segmentation techniques to automatically detect floods when water levels surpass certain thresholds. This system utilized Synthetic Aperture Radar (SAR) satellite images and various terrain data, performing Semantic Segmentation on watershed regions. The dataset combined 7 channels, including Sentinel-1 SAR images, Digital Elevation Models (DEMs), and watercourse buffer data. The national land cover data, indexed according to scientific standards, known as the Land Cover Classification System, was used as label data. The advantage of this approach was the pre-labeled land cover types, enabling automated extraction of suitable training data for specific regions.

For the segmentation model, I experimented with Google's DeepLab v3+ model, which demonstrated excellent performance on RGB channels at the time. Data manipulation was carried out using QGIS, while AWS infrastructure with CUDA acceleration was employed for model training. The outcome was a watershed detection model with a pixel accuracy of 0.95, covering the entire Korean Peninsula.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/satgeo/all_result.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/satgeo/SAR_shp_crop.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/satgeo/sat_seg.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Caption photos easily. On the left, a road goes through a tunnel. Middle, leaves artistically fall in a hipster photoshoot. Right, in another hipster photoshoot, a lumberjack grasps a handful of pine needles.
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/satgeo/make_shp.png" title="example image" class="img-fluid rounded z-depth-1" %}
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
        {% include figure.html path="assets/img/satgeo/geo_map.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="assets/img/satgeo/SAR_search.png" title="example image" class="img-fluid rounded z-depth-1" %}
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
        {% include figure.html path="assets/img/satgeo/result_island.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="assets/img/satgeo/result_island_seg.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
```
{% endraw %}
