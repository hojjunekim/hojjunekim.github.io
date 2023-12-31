---
layout: page
title: Fault Tolerant Control of Quadrotor
description: Feedback Linearization, SMC, Backstepping
img: assets/img/FTC/3dplot.jpg
importance: 3
category: fun
---

In this paper, the feedback linearization, sliding mode and backstepping control methods are used to con- trol the nonlinear quadrotor vehicle in fault-free condition and faulty condition. First, derived a mathematical model of the quadrotor. Then applied three different nonlinear control methods and showed the convergence stability and controllable variables. Moreover one of the blade goes faulty condition, we derived how the controller have to be changed. We showed controllable and stability in fault tolerant control using the controllers previously constructed by changing the input variables.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/FTC/inputs.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/FTC/error.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/FTC/3dplot.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

