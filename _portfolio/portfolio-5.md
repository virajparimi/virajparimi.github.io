---
title: "Autonomous Driving using CNNs"
excerpt: "Trained a custom CNN on Unreal Engine Blocks simulator data to steer the vehicle autonomously."
collection: portfolio
header:
  teaser: Autonomous_Driving.gif
  teaser_alt: "Autonomous vehicle navigating a simulated track"
lead_image: /images/Autonomous_Driving.gif
lead_image_alt: "CNN-driven autonomous driving simulation"
summary: "Collected simulator trajectories, trained a CNN to map images to steering commands, and demonstrated closed-loop driving in the Unreal Blocks environment."
project_links:
  - label: Code
    url: https://github.com/virajparimi/Autonomous-Driving-Simulation
    icon: code
links:
  - label: Code
    url: https://github.com/virajparimi/Autonomous-Driving-Simulation
    icon: code
---

We trained a custom convolutional neural network on data collected from the Unreal Engine Blocks driving simulator to learn vision-based steering. The model generates control commands directly from RGB frames and is able to drive the vehicle autonomously along the course, highlighting the potential of end-to-end behavioral cloning for simulated driving tasks.
