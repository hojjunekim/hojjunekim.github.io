---
layout: page
title: Crowd Navigation with LiDAR via Reinforcement Learning
affiliation: Perception and Learning for Robotics graduate course project, ETH Zürich
description: Teacher-Student RL, LiDAR Encoding
project_year: 2024
img: /assets/img/projects/plr/plr.gif
# img: /assets/img/projects/plr/thumb.png
pdf: /img/projects/plr/paper.pdf
video: https://youtu.be/vwoVTW57BS4
category: eth
---

Navigating around dynamic obstacles such as human crowds poses a significant challenge for mobile robots. This project introduces a pipeline to train a hierarchical, LiDAR based perception-navigation policy end-to-end with reinforcement learning. The planner utilizes an encoding of a LiDAR point cloud to predict velocity commands that are passed to a low-level policy. Utilizing the student-teacher approach, we first train a teacher policy using privileged observations, which include the velocities of the obstacles and a sparse 2D point cloud. A LiDAR encoder, trained using self-supervision, embeds the raw point-cloud data for the student policy. To enable the planner to reason about the motion of the obstacles and prevent it from getting stuck in local minima, we include a gated recurrent unit in our policy network. We evaluate the teacher policy in both static and dynamic environments, demonstrating that observing the velocities of the obstacles enhances performance in dynamic scenarios. Additionally, our results reveal that the current implementation of the recurrent unit in combination with recurrent PPO does not improve the performance in the static case, necessitating further research.