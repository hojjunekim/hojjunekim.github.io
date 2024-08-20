---
layout: page
title: Gaussian Belief Propagation for Continuus time SLAM
description: Graph Optimization, Continuous Time SLAM
# description: Computer Vision Course Project
img: /assets/img/projects/v4rl/thumb.png
importance: 1
category: eth
---

Conventional Simultaneous Localization and Mapping (SLAM) methods, typically based on discrete-time formulations, have demonstrated significant utility in various robotics applications. These methods, however, face challenges such as quantization errors and inefficiencies in handling asynchronous data from multiple sensors. Continuous-time SLAM approaches, utilizing splines to represent motion, o↵er a promising alternative by more naturally integrating sensor data captured at irregular intervals. Despite their potential, many continuous-time SLAM methods rely on centralized Non-Linear Least Squares (NLLS) solvers, which can be computationally expensive and inefficient for asynchronous data processing.
This project addresses challenges in SLAM by integrating the decentralized solver Gaussian Belief Propagation (GBP) with a continuous-time formulation, specifically utilizing Z-splines. The approach aims to enhance robustness and efficiency in multirobot systems. The method is validated using a real-world dataset and compared against traditional NLLS solvers. Results demonstrate that GBP with continuous time representation outperforms NLLS in handling perturbations, providing more stable and efficient optimization.