---
title: "Catching a Ping Pong Ball with an iiwa"
excerpt: "We programmed the kinematics of a KUKA iiwa using Drake to catch and stabilize a ping pong ball."
collection: portfolio
header:
  teaser: Ping_Pong.png
  teaser_alt: "KUKA iiwa preparing to catch a ping pong ball"
lead_image: /images/Ping_Pong.png
lead_image_alt: "Ping pong catching pipeline for the KUKA iiwa"
summary: "Drake-based finite-state control splits the catch into pre- and post-contact modes, combining projectile modeling with stabilized IK to stop a ping pong ball on an iiwa paddle."
project_links:
  - label: PDF
    url: /files/portfolio-2/report.pdf
    icon: file-pdf
    btn_class: btn--primary
  - label: Video
    url: https://www.youtube.com/watch?v=c-lpFsNBOzU&list=PLkx8KyIQkMfUbHMSbSVTmCM63rICMdFNI&index=14
    icon: video
  - label: Code
    url: https://github.com/cameronwp/ping-pong-catcher
    icon: code
links:
  - label: PDF
    url: /files/portfolio-2/report.pdf
    icon: file-pdf
    btn_class: btn--primary
  - label: Video
    url: https://www.youtube.com/watch?v=c-lpFsNBOzU&list=PLkx8KyIQkMfUbHMSbSVTmCM63rICMdFNI&index=14
    icon: video
  - label: Code
    url: https://github.com/cameronwp/ping-pong-catcher
    icon: code
---

We programmed the kinematics of a KUKA iiwa in Drake to intercept and stabilize a ping pong ball using a ping pong paddle. The controller separates the task into pre-contact and post-contact regimes: before impact we apply projectile equations within a finite-state machine to position and orient the paddle, and after impact we switch to a PD controller with offset stabilization to keep the ball near equilibrium. Both regimes feed desired end-effector velocities to a differential IK controller that enforces joint limits. Using ground-truth ball and paddle states, the system consistently halts balls with diverse initial conditions, though long-term stabilization remains challenging and motivates future work.
