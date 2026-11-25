---
title: "Catching a Ping Pong Ball with an iiwa"
collection: portfolio
order: 2
header:
  teaser: Ping_Pong.png
  teaser_alt: "KUKA iiwa preparing to catch a ping pong ball"
lead_image: /images/Ping_Pong.png
lead_image_alt: "Five simulation snapshots from 0 to 0.5 seconds of a KUKA iiwa raising a paddle to catch a falling ball"
lead_image_caption: "Snapshots of a catch in simulation. The paddle rises to meet the falling ball, and by 0.5 s the ball is on the paddle."
summary: "A finite-state controller in Drake catches a falling ping pong ball on a simulated iiwa's paddle and tries to keep it balanced there."
links:
  - label: PDF
    url: /files/portfolio-2/report.pdf
    icon: file-pdf
    btn_class: btn--primary
  - label: Code
    url: https://github.com/cameronwp/ping-pong-catcher
    icon: code
  - label: Video
    url: https://www.youtube.com/watch?v=c-lpFsNBOzU
    icon: video
---

In this final project for MIT 6.843 (Robotic Manipulation) with Cameron Pittman, we programmed a simulated KUKA iiwa in Drake to catch a falling ping pong ball on a paddle and keep it there. A finite-state machine splits the task in two. Before contact, the paddle follows a trajectory computed from projectile motion so that it meets the ball at the ball's velocity. After contact, a PD controller makes small translational and rotational corrections to keep the ball on the paddle. Both modes send end-effector velocities to a differential inverse kinematics controller that enforces joint limits, and the controller reads the true ball and paddle states instead of running perception. The arm stopped the ball from a range of starting positions and velocities, but keeping it balanced for long periods remained difficult.
