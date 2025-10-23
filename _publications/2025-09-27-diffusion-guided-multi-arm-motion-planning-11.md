---
title: "Diffusion-Guided Multi-Arm Motion Planning" 
collection: publications
permalink: /publication/2025-09-27-diffusion-guided-multi-arm-motion-planning-11
date: 2025-09-27
venue: 'CoRL'
pub_type: conference
also_in:
  - "RSS Workshop on Scalable and Resilient Multi-Robot Systems"
authors:
  - Viraj Parimi
  - Brian C. Williams
summary: "Diffusion-guided MAPF decomposition lets us scale multi-arm planning by pairing single-arm generators with a collision-resolving duet, beating data-hungry baselines across large teams."
links:
  - label: CoRL Paper
    url: /files/paper13.pdf
    icon: file-pdf
    btn_class: btn--primary
  - label: RSS Paper
    url: /files/paper14.pdf
    icon: file-pdf
    btn_class: btn--primary
  - label: Website
    url: https://diff-mapf-mers.csail.mit.edu/
    icon: globe
abstract: |-
   Multi-arm motion planning is fundamental for enabling arms to complete complex long-horizon tasks in shared spaces efficiently but current methods struggle with scalability due to exponential state-space growth and reliance on large training datasets for learned models. Inspired by Multi-Agent Path Finding (MAPF), which decomposes planning into single-agent problems coupled with collision resolution, we propose a novel diffusion-guided multi-arm planner (DG-MAP) that enhances scalability of learning-based models while reducing their reliance on massive multi-arm datasets. Recognizing that collisions are primarily pairwise, we train two conditional diffusion models, one to generate feasible single-arm trajectories, and a second, to model the dual-arm dynamics required for effective pairwise collision resolution. By integrating these specialized generative models within a MAPF-inspired structured decomposition, our planner efficiently scales to larger number of arms. Evaluations against alternative learning-based methods across various team sizes demonstrate our method's effectiveness and practical applicability.
header:
  teaser: DGMAP.png
  teaser_alt: "Diffusion-Guided Multi-Arm Planner"
bibtex: |-
  @InProceedings{pmlr-v305-parimi25a,
    title = {Diffusion-Guided Multi-Arm Motion Planning},
    author = {Parimi, Viraj and Williams, Brian C.},
    booktitle = {Proceedings of The 9th Conference on Robot Learning},
    pages = {4684--4696},
    year = {2025},
    editor = {Lim, Joseph and Song, Shuran and Park, Hae-Won},
    volume = {305},
    series = {Proceedings of Machine Learning Research},
    month = {27--30 Sep},
    publisher = {PMLR},
    pdf = {https://raw.githubusercontent.com/mlresearch/v305/main/assets/parimi25a/parimi25a.pdf},
    url = {https://proceedings.mlr.press/v305/parimi25a.html},
  }
lead_image: /images/DGMAP.png
lead_image_alt: "Diffusion-Guided Multi-Arm Planner"
---

Develops DG-MAP, a MAPF-inspired framework that trains two conditional diffusion models, one for single-arm trajectories and one for pairwise collision resolution, to scale multi-arm motion planning without massive datasets; experiments across varying team sizes show consistently superior performance over learning-based baselines.
