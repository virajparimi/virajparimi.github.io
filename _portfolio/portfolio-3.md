---
title: "Sample-Based Planning under Discrete Space"
excerpt: "Proposed a hierarchical decomposition that discretizes the continuous sample space of PRM/RRT algorithms to tighten completeness guarantees."
collection: portfolio
header:
  teaser: Planning.png
  teaser_alt: "Discrete roadmap construction for robotic arm planning"
lead_image: /images/Planning.png
lead_image_alt: "Hierarchical discrete sampling for robotic arm motion planning"
summary: "dRRT couples discrete sampling with search-based refinement, reusing computation to accelerate 5-DOF arm planning versus traditional RRT."
project_links:
  - label: PDF
    url: /files/portfolio-3/report.pdf
    icon: file-pdf
    btn_class: btn--primary
  - label: Slides
    url: /files/portfolio-3/presentation.pptx
    icon: file-powerpoint
  - label: Code
    url: https://bitbucket.org/eaglez1111/16782_final_proj/src/master/
    icon: code
links:
  - label: PDF
    url: /files/portfolio-3/report.pdf
    icon: file-pdf
    btn_class: btn--primary
  - label: Slides
    url: /files/portfolio-3/presentation.pptx
    icon: file-powerpoint
  - label: Code
    url: https://bitbucket.org/eaglez1111/16782_final_proj/src/master/
    icon: code
---

Introduced dRRT, a discrete sampling-based planner that combines Bresenham-style edge discretization with search-based heuristics to deliver anytime motion plans while reusing prior computation. In 5-DOF arm benchmarks, the method achieves faster convergence than classical RRT thanks to its hierarchical decomposition of the configuration space.
