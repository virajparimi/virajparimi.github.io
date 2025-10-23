---
title: "Safe Multi-Agent Navigation guided by Goal-Conditioned Safe Reinforcement Learning" 
collection: publications
permalink: /publication/2025-05-19-safe-multi-agent-navigation-guided-by-goal-conditioned-safe-reinforcement-learning-10
date: 2025-05-19
venue: 'ICRA'
pub_type: conference
also_in:
  - "NeurIPS Workshop on Intrinsically Motivated Open-Ended Learning"
  - "CoRL Workshop on Learning Effective Abstractions for Planning"
authors:
  - Meng Feng*
  - Viraj Parimi*
  - Brian C. Williams
summary: "Unified conflict-based search with goal-conditioned safe RL to plan long-horizon multi-agent navigation that stays safe without sacrificing efficiency."
links:
  - label: ICRA Paper
    url: /files/paper12.pdf
    icon: file-pdf
    btn_class: btn--primary
  - label: NeurIPS Paper
    url: /files/paper10.pdf
    icon: file-pdf
    btn_class: btn--primary
  - label: CoRL Paper
    url: /files/paper11.pdf
    icon: file-pdf
    btn_class: btn--primary
  - label: Website
    url: https://safe-visual-mapf-mers.csail.mit.edu/
    icon: globe
abstract: |-
  Safe navigation is essential for autonomous systems operating in hazardous environments. Traditional planning methods are effective for solving long-horizon tasks but depend on the availability of a graph representation with predefined distance metrics. In contrast, safe Reinforcement Learning (RL) is capable of learning complex behaviors without relying on manual heuristics but fails to solve long-horizon tasks, particularly in goal-conditioned and multi-agent scenarios.

  In this paper, we introduce a novel method that integrates the strengths of both planning and safe RL. Our method leverages goal-conditioned RL (GCRL) and safe RL to learn a goal-conditioned policy for navigation while concurrently estimating cumulative distance and safety levels using learned value functions via an automated self-training algorithm. By constructing a graph with states from the replay buffer, our method prunes unsafe edges and generates a waypoint-based plan that the agent then executes by following those waypoints sequentially until their goal locations are reached. This graph pruning and planning approach via the learned value functions allows our approach to flexibly balance the trade-off between faster and safer routes especially over extended horizons.

  Utilizing this unified high-level graph and a shared low-level safe GCRL policy, we extend this approach to address the multi-agent safe navigation problem. In particular, we leverage Conflict-Based Search (CBS) to create waypoint-based plans for multiple agents allowing for their safer navigation over extended horizons. This integration enhances the scalability of goal-conditioned safe RL in multi-agent scenarios, enabling efficient coordination among agents. Extensive benchmarking against state-of-the-art baselines demonstrates the effectiveness of our method in achieving distance goals safely for multiple agents in complex and hazardous environments.
header:
  teaser: Safe_MAPF.png
  teaser_alt: "Safe multi-agent navigation depiction"
bibtex: |-
  @INPROCEEDINGS{11127461,
    author={Feng, Meng and Parimi, Viraj and Williams, Brian},
    booktitle={2025 IEEE International Conference on Robotics and Automation (ICRA)},
    title={Safe Multi-Agent Navigation Guided by Goal-Conditioned Safe Reinforcement Learning},
    year={2025},
    volume={},
    number={},
    pages={16869-16875},
    keywords={Training;Visualization;Navigation;Scalability;Heuristic algorithms;Reinforcement learning;Manuals;Distance measurement;Planning;Safety},
    doi={10.1109/ICRA55743.2025.11127461}
  }
lead_image: /images/Safe_MAPF.svg
lead_image_alt: "Safe multi-agent navigation depiction"
---

We prune risky graph edges with learned value functions and feed the remainder into CBS, allowing a shared goal-conditioned safe RL policy to scale to multi-agent navigation problems while retaining safety guarantees.
