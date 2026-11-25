---
title: "Discrete Sampling-Based Planning"
collection: portfolio
order: 3
header:
  teaser: Planning.png
  teaser_alt: "Discrete roadmap construction for robotic arm planning"
lead_image: /images/Planning.png
lead_image_alt: "An RRT tree among obstacles in continuous space next to a dRRT tree on a grid"
lead_image_caption: "RRT grows its tree in continuous space (left), while dRRT samples points on a grid that it refines as needed (right)."
summary: "A grid-based variant of RRT that reuses collision checks across grid resolutions and plans faster than RRT on a 5-DOF arm."
links:
  - label: PDF
    url: /files/portfolio-3/report.pdf
    icon: file-pdf
    btn_class: btn--primary
  - label: Code
    url: https://bitbucket.org/eaglez1111/16782_final_proj/src/master/
    icon: code
  - label: Slides
    url: /files/portfolio-3/presentation.pptx
    icon: file-powerpoint
---

In this final project for CMU 16-782 (Planning and Decision-making in Robotics) with Dapeng Zhao and Rockey Hester, we built dRRT, a version of RRT that samples on a grid instead of in continuous space. dRRT connects grid points with Bresenham's line algorithm and refines the grid only when it needs to, which lets it reuse earlier collision checks. On a 5-DOF arm, dRRT **found plans in 0.027 seconds on average, against 0.076 for RRT**, and used far fewer samples. RRT-Connect and RRT* were still faster, and dRRT's paths cost more than RRT's.
