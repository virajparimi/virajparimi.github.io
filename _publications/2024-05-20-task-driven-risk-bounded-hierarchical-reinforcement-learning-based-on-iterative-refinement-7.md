---
title: "Task-driven Risk-bounded Hierarchical Reinforcement Learning Based on Iterative Refinement" 
collection: publications
permalink: /publication/2024-05-20-task-driven-risk-bounded-hierarchical-reinforcement-learning-based-on-iterative-refinement
date: 2024-05-20
venue: 'AAAI Spring Symposium on Human-Like Learning'
pub_type: workshop
authors:
  - Viraj Parimi
  - Sungkweon Hong
  - Brian C. Williams
summary: "Bridged conditional planning with hierarchical RL to iteratively refine risk budgets, enabling agents to tackle long-horizon tasks while respecting safety constraints."
links:
  - label: Paper
    url: /files/paper7.pdf
    icon: file-pdf
    btn_class: btn--primary
  - label: Slides
    url: /files/slides2.pptx
    icon: file-powerpoint
abstract: |-
  Deep Reinforcement Learning(RL) faces significant scalability challenges when dealing with complex, long-horizon tasks. This paper addresses this issue by introducing a hybrid approach that combines model-based conditional planning with RL. The proposed approach incorporates a novel iterative primitive refinement technique that strategically biases computational effort to accelerate policy improvement, which is particularly beneficial in risk-bounded and time-critical domains. In addition, we explore a comprehensive range of prioritization methods and conduct a thorough analysis of their strengths and weaknesses. To demonstrate the scalability of the proposed approach, we evaluate it in both 2D and 3D robot manipulation environments with relevant baseline methods, while empirically examining the performance of the prioritization methods.
bibtex: |-
  @inproceedings{parimi2024task,
    title={Task-driven Risk-bounded Hierarchical Reinforcement Learning Based on Iterative Refinement},
    author={Parimi, Viraj and Hong, Sungkweon and Williams, Brian},
    booktitle={Proceedings of the AAAI Symposium Series},
    volume={3},
    number={1},
    pages={573--575},
    year={2024}
  }
header:
  teaser: Robot_Env.png
  teaser_alt: "Risk-aware hierarchical learning diagram"
lead_image: /images/Robot_Env.png
lead_image_alt: "Risk-aware hierarchical learning diagram"
---

Our approach incrementally tightens motion primitives with learned risk-aware priors, so safety-constrained agents can adapt planning horizons without exploding computation.
