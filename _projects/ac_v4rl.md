---
layout: page
title: Distributed Optimization with Gaussian Belief Propagation for Continuous-time SLAM
affiliation: Vision for Robotics Lab. ETH Zürich
position: Undergraduate Researcher
description: Distributed Optimization, Continuous Time SLAM
project_year: Feb. 2024 - Aug. 2024
img: /assets/img/projects/v4rl/gbp.gif
# img: /assets/img/projects/v4rl/thumb.png
code: https://github.com/VIS4ROB-lab/hyperion
slides: /assets/img/projects/v4rl/slides.pdf
pdf: /img/projects/v4rl/report.pdf
category: eth
---

Conventional Simultaneous Localization and Mapping (SLAM) methods, typically based on discrete-time formulations, have demonstrated significant utility in various robotics applications. These methods, however, face challenges such as quantization errors and inefficiencies in handling asynchronous data from multiple sensors. Continuous-time SLAM approaches, utilizing splines to represent motion, o↵er a promising alternative by more naturally integrating sensor data captured at irregular intervals. Despite their potential, many continuous-time SLAM methods rely on centralized Non-Linear Least Squares (NLLS) solvers, which can be computationally expensive and inefficient for asynchronous data processing.
This project addresses challenges in SLAM by integrating the decentralized solver Gaussian Belief Propagation (GBP) with a continuous-time formulation, specifically utilizing Z-splines. The approach aims to enhance robustness and efficiency in multirobot systems. The method is validated using a real-world dataset and compared against traditional NLLS solvers. Results demonstrate that GBP with continuous time representation outperforms NLLS in handling perturbations, providing more stable and efficient optimization.