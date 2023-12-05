---
layout: page
title: Real-time flood monitoring system by water detection using Sentinel-1 satellite image
description: Semantic Segmentation, data achieve automizing
img: assets/img/satgeo/all_result.png
importance: 4
category: work
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

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/satgeo/make_shp.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>


<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.html path="assets/img/satgeo/geo_map.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="assets/img/satgeo/SAR_search.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>


