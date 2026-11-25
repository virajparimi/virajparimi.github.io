---
title: "Towards efficient and scalable planning: Learning search heuristics for multi-agent planning frameworks" 
collection: publications
permalink: /publication/2023-10-23-towards-efficient-and-scalable-planning-learning-search-heuristics-for-multi-agent-planning-frameworks
date: 2023-10-23
venue: 'CoRL Workshop on Learning Effective Abstractions for Planning (LEAP)'
venue_short: 'CoRL LEAP 2023'
pub_type: workshop
authors:
  - Ashwin Misra
  - Viraj Parimi
  - Mansi Agarwal
  - Zachary B. Rubinstein
  - Stephen F. Smith
summary: "Trains an LSTM to predict which timeline slot the T-HTN planner would choose, matching the planner's choice 90% of the time while planning faster."
links:
  - label: Paper
    url: /files/paper6.pdf
    icon: file-pdf
    btn_class: btn--primary
abstract: |-
  The combinatorics of various search-based approaches to planning pose a solid barrier to scalable performance. Such approaches become increasingly complex and complicated, even in single-agent planning contexts, as the number of goals to be achieved increases. We propose that such complex combinatorics can be overcome by learning an abstract model of the planner’s search that utilizes various state characteristics to learn the relative quality of various search decisions over time. An efficient machine learning framework consisting of a Long Short Term Memory Network is developed to accelerate the time-consuming search process and achieve a substantial computational speedup by learning the planner’s reasoning from spatial and temporal global states and constraints. It generalizes well and enables efficient usage of multiple agents across multiple tasks.
bibtex: |-
  @inproceedings{misra2023towards,
    title     = {Towards Efficient and Scalable Planning: Learning Search Heuristics for Multi-Agent Planning Frameworks},
    author    = {Misra, Ashwin and Parimi, Viraj and Agarwal, Mansi and Rubinstein, Zachary B. and Smith, Stephen F.},
    booktitle = {CoRL Workshop on Learning Effective Abstractions for Planning (LEAP)},
    year      = {2023}
  }
header:
  teaser: HTN_Repr.png
  teaser_alt: "Learning-guided planning graphic"
lead_image: /images/HTN_Repr.png
lead_image_alt: "Hierarchical task network decomposing move_item into pick_item and drop_item and their subtasks"
lead_image_caption: "How a task to move an item decomposes into picking it up and dropping it off, and then into grasp, release and return-home steps, with the resources each step needs."
---

T-HTN schedules a new task by expanding every way to decompose it and checking each candidate slot on the robots' timelines, so planning time grows with the number of slots. This work trains an LSTM on T-HTN's own decisions to predict which slot the planner would choose. In a deep space habitat maintenance domain where two robots on a rail handle pick-and-place requests, the LSTM **picks the planner's slot 90.2% of the time**, against 86.3% for an MLP baseline. It also plans about 15% faster than T-HTN and the POPF temporal planner.
