---
title: "Towards efficient and scalable planning: Learning search heuristics for multi-agent planning frameworks" 
collection: publications
permalink: /publication/2023-10-23-towards-efficient-and-scalable-planning-learning-search-heuristics-for-multi-agent-planning-frameworks
date: 2023-10-23
venue: 'CoRL | Workshop on Learning Effective Abstractions for Planning'
pub_type: workshop
authors:
  - Ashwin Misra
  - Viraj Parimi
  - Mansi Agarwal
  - Zachary B. Rubinstein
  - Stephen F. Smith
summary: "Trained recurrent models that learn search heuristics for multi-agent planners, accelerating long-horizon planning while preserving solution quality."
links:
  - label: Paper
    url: /files/paper6.pdf
    icon: file-pdf
    btn_class: btn--primary
abstract: |-
  The combinatorics of various search-based approaches to planning pose a solid barrier to scalable performance. Such approaches become increasingly complex and complicated, even in single-agent planning contexts, as the number of goals to be achieved increases. We propose that such complex combinatorics can be overcome by learning an abstract model of the planner’s search that utilizes various state characteristics to learn the relative quality of various search decisions over time. An efficient machine learning framework consisting of a Long Short Term Memory Network is developed to accelerate the time-consuming search process and achieve a substantial computational speedup by learning the planner’s reasoning from spatial and temporal global states and constraints. It generalizes well and enables efficient usage of multiple agents across multiple tasks
header:
  teaser: HTN_Repr.png
  teaser_alt: "Learning-guided planning graphic"
lead_image: /images/HTN_Repr.png
lead_image_alt: "Learning-guided planning graphic"
---

We show how sequence models capture a planner’s decision patterns and use the learned heuristics to shrink search time across diverse multi-agent planning tasks.
