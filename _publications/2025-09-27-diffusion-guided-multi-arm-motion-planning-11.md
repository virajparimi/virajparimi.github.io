---
title: "Diffusion-Guided Multi-Arm Motion Planning" 
collection: publications
permalink: /publication/2025-09-27-diffusion-guided-multi-arm-motion-planning-11
date: 2025-09-27
venue: 'Conference on Robot Learning (CoRL)'
venue_short: 'CoRL 2025'
pub_type: conference
also_in:
  - "RSS MRS 2025"
authors:
  - Viraj Parimi
  - Brian C. Williams
summary: "Generates each arm's motion with a single-arm diffusion model and repairs conflicts with a dual-arm model, keeping average success above 92% with up to eight arms while training only on single- and dual-arm data."
links:
  - label: Paper
    url: https://proceedings.mlr.press/v305/parimi25a.html
    icon: file-pdf
    btn_class: btn--primary
  - label: Code
    url: https://github.com/virajparimi/diff-mapf
    icon: code
  - label: Website
    url: https://diff-mapf-mers.csail.mit.edu/
    icon: globe
  - label: Video
    page_only: true
    url: https://diff-mapf-mers.csail.mit.edu/static/videos/spotlight_video.mp4
    icon: file-video
  - label: Poster
    page_only: true
    url: https://diff-mapf-mers.csail.mit.edu/static/files/CoRL_Poster.pdf
    icon: file-image
abstract: |-
   Multi-arm motion planning is fundamental for enabling arms to complete complex long-horizon tasks in shared spaces efficiently but current methods struggle with scalability due to exponential state-space growth and reliance on large training datasets for learned models. Inspired by Multi-Agent Path Finding (MAPF), which decomposes planning into single-agent problems coupled with collision resolution, we propose a novel diffusion-guided multi-arm planner (DG-MAP) that enhances scalability of learning-based models while reducing their reliance on massive multi-arm datasets. Recognizing that collisions are primarily pairwise, we train two conditional diffusion models, one to generate feasible single-arm trajectories, and a second, to model the dual-arm dynamics required for effective pairwise collision resolution. By integrating these specialized generative models within a MAPF-inspired structured decomposition, our planner efficiently scales to larger number of arms. Evaluations against alternative learning-based methods across various team sizes demonstrate our method's effectiveness and practical applicability.
header:
  teaser: DGMAP_teaser.png
  teaser_alt: "Diffusion-Guided Multi-Arm Planner"
bibtex: |-
  @inproceedings{parimi2025diffusion,
    title     = {Diffusion-Guided Multi-Arm Motion Planning},
    author    = {Parimi, Viraj and Williams, Brian C.},
    booktitle = {Proceedings of the 9th Conference on Robot Learning (CoRL)},
    series    = {Proceedings of Machine Learning Research},
    volume    = {305},
    pages     = {4684--4696},
    year      = {2025},
    publisher = {PMLR},
    url       = {https://proceedings.mlr.press/v305/parimi25a.html}
  }
lead_video: /images/highlights/dgmap.mp4
lead_video_poster: /images/highlights/dgmap.jpg
lead_video_alt: "Four robot arms placing objects in a shared bin"
lead_video_caption: "Four arms pick objects off the ground and place them in a shared bin."
---

Collisions between arms are mostly pairwise, so DG-MAP plans with two diffusion models instead of learning the whole team's motion end to end. A single-arm model plans each arm on its own, and a dual-arm model repairs conflicts between pairs, the way MAPF planners split a team problem into single-agent searches plus collision resolution.

<figure class="page__lead-media">
  <img src="/images/DGMAP.png" alt="Overview of DG-MAP, with single-arm and dual-arm diffusion models inside a search over conflicts" loading="lazy">
  <figcaption>Each arm first plans on its own with a single-arm diffusion model. When two arms conflict, one of them uses a dual-arm diffusion model, conditioned on both arms' observations, to generate a collision-free motion.</figcaption>
</figure>

Trained only on single-arm and dual-arm data, it **keeps average success above 92% with up to eight arms** and **reaches 89% on a pick-and-place task** where arms move objects from the ground into a shared bin.

<figure class="page__lead-media">
  <video autoplay muted loop playsinline preload="metadata" poster="/images/highlights/dgmap_3to8.jpg" aria-label="DG-MAP on test tasks with three to eight arms">
    <source src="/images/highlights/dgmap_3to8.mp4" type="video/mp4">
  </video>
  <figcaption>DG-MAP on test tasks with three to eight arms (left to right, top to bottom).</figcaption>
</figure>
