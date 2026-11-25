---
title: "Task-driven Risk-bounded Hierarchical Reinforcement Learning Based on Iterative Refinement" 
collection: publications
permalink: /publication/2024-05-20-task-driven-risk-bounded-hierarchical-reinforcement-learning-based-on-iterative-refinement
date: 2024-05-20
venue: 'AAAI Spring Symposium on Human-Like Learning (Talk)'
venue_short: 'AAAI SSS 2024'
pub_type: workshop
authors:
  - Viraj Parimi
  - Sungkweon Hong
  - Brian C. Williams
summary: "Combines risk-bounded conditional planning with learned motion primitives, iteratively refining the primitives that most affect the high-level plan."
links:
  - label: Paper
    url: https://doi.org/10.1609/aaaiss.v3i1.31281
    icon: file-pdf
    btn_class: btn--primary
  - label: Slides
    page_only: true
    url: /files/slides2.pptx
    icon: file-powerpoint
abstract: |-
  Deep Reinforcement Learning(RL) faces significant scalability challenges when dealing with complex, long-horizon tasks. This paper addresses this issue by introducing a hybrid approach that combines model-based conditional planning with RL. The proposed approach incorporates a novel iterative primitive refinement technique that strategically biases computational effort to accelerate policy improvement, which is particularly beneficial in risk-bounded and time-critical domains. In addition, we explore a comprehensive range of prioritization methods and conduct a thorough analysis of their strengths and weaknesses. To demonstrate the scalability of the proposed approach, we evaluate it in both 2D and 3D robot manipulation environments with relevant baseline methods, while empirically examining the performance of the prioritization methods.
bibtex: |-
  @inproceedings{parimi2024task,
    title     = {Task-Driven Risk-Bounded Hierarchical Reinforcement Learning Based on Iterative Refinement},
    author    = {Parimi, Viraj and Hong, Sungkweon and Williams, Brian C.},
    booktitle = {Proceedings of the AAAI Symposium Series},
    volume    = {3},
    number    = {1},
    pages     = {573--575},
    year      = {2024},
    doi       = {10.1609/aaaiss.v3i1.31281}
  }
header:
  teaser: Robot_Env.png
  teaser_alt: "Risk-aware hierarchical learning diagram"
lead_image: /images/Robot_Env.png
lead_image_alt: "A robot arm above a table with gray block obstacles and white sphere landmarks"
lead_image_caption: "The robot arm environment, with obstacles (gray blocks) and landmarks (white spheres) between which motion primitives are learned."
---

Deep RL struggles to learn long-horizon navigation directly. Its policies also cannot guarantee success, only bound the risk of failure. This work places landmarks in the environment, learns a motion primitive between each pair of nearby landmarks with deep RL, and treats each primitive as an action that either succeeds or fails. A conditional planner for constrained stochastic shortest path problems then chains the primitives into a plan **whose failure probability stays within a user-set bound**. Training time is limited, so the method alternates between planning and training and spends that training on the primitives that matter most to the current plan. The paper compares bandit-style rules for choosing those primitives.
