---
layout: page
title: 2D Ego-motion with Only mmWave Radar
description: Feature Extraction, ICP
img: /assets/img/projects/radar/thumb.png
importance: 1
category: snu
---

The interest in single-chip mmWave Radar is driven by their compact form factor, cost-effectiveness, and robustness under harsh environmental conditions. Despite its promising attributes, the principal limitation of mmWave radar lies in its capacity for autonomous yaw rate estimation. Conventional solutions have often resorted to integrating inertial measurement unit (IMU) or deploying multiple radar units to circumvent this shortcoming. This paper introduces an innovative methodology for two-dimensional ego-motion estimation, focusing on yaw rate deduction, utilizing solely mmWave radar sensors. By applying a weighted Iterated Closest Point (ICP) algorithm to register processed points derived from heatmap data, our method facilitates 2D ego-motion estimation devoid of prior information. Through experimental validation, we verified the effectiveness and promise of our technique for ego-motion estimation using exclusively radar data.