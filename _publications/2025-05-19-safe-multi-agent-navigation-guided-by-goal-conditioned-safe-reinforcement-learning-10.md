---
title: "Safe Multi-Agent Navigation Guided by Goal-Conditioned Safe Reinforcement Learning" 
collection: publications
permalink: /publication/2025-05-19-safe-multi-agent-navigation-guided-by-goal-conditioned-safe-reinforcement-learning-10
date: 2025-05-19
venue: 'IEEE International Conference on Robotics and Automation (ICRA)'
venue_short: 'ICRA 2025'
pub_type: conference
also_in:
  - "NeurIPS IMOL 2024"
  - "CoRL LEAP 2024"
authors:
  - Meng Feng*
  - Viraj Parimi*
  - Brian C. Williams
summary: "Builds a waypoint graph from visual experience using learned distance and safety estimates, plans paths on it with conflict-based search, and executes them with a safe goal-conditioned policy."
links:
  - label: Paper
    url: https://doi.org/10.1109/ICRA55743.2025.11127461
    icon: file-pdf
    btn_class: btn--primary
  - label: arXiv
    page_only: true
    url: https://arxiv.org/abs/2502.17813
    icon: file-pdf
  - label: Code
    url: https://github.com/virajparimi/safe-visual-mapf
    icon: code
  - label: Website
    url: https://safe-visual-mapf-mers.csail.mit.edu/
    icon: globe
  - label: Poster
    page_only: true
    url: https://safe-visual-mapf-mers.csail.mit.edu/static/files/ICRA_Poster.pdf
    icon: file-image
abstract: |-
  Safe navigation is essential for autonomous systems operating in hazardous environments. Traditional planning methods are effective for solving long-horizon tasks but depend on the availability of a graph representation with predefined distance metrics. In contrast, safe Reinforcement Learning (RL) is capable of learning complex behaviors without relying on manual heuristics but fails to solve long-horizon tasks, particularly in goal-conditioned and multi-agent scenarios.

  In this paper, we introduce a novel method that integrates the strengths of both planning and safe RL. Our method leverages goal-conditioned RL (GCRL) and safe RL to learn a goal-conditioned policy for navigation while concurrently estimating cumulative distance and safety levels using learned value functions via an automated self-training algorithm. By constructing a graph with states from the replay buffer, our method prunes unsafe edges and generates a waypoint-based plan that the agent then executes by following those waypoints sequentially until their goal locations are reached. This graph pruning and planning approach via the learned value functions allows our approach to flexibly balance the trade-off between faster and safer routes especially over extended horizons.

  Utilizing this unified high-level graph and a shared low-level safe GCRL policy, we extend this approach to address the multi-agent safe navigation problem. In particular, we leverage Conflict-Based Search (CBS) to create waypoint-based plans for multiple agents allowing for their safer navigation over extended horizons. This integration enhances the scalability of goal-conditioned safe RL in multi-agent scenarios, enabling efficient coordination among agents. Extensive benchmarking against state-of-the-art baselines demonstrates the effectiveness of our method in achieving distance goals safely for multiple agents in complex and hazardous environments.
header:
  teaser: Safe_MAPF_clean.png
  teaser_alt: "Safe multi-agent navigation depiction"
bibtex: |-
  @inproceedings{feng2025safe,
    title     = {Safe Multi-Agent Navigation Guided by Goal-Conditioned Safe Reinforcement Learning},
    author    = {Feng, Meng and Parimi, Viraj and Williams, Brian C.},
    booktitle = {Proceedings of the IEEE International Conference on Robotics and Automation (ICRA)},
    pages     = {16869--16875},
    year      = {2025},
    doi       = {10.1109/ICRA55743.2025.11127461}
  }
lead_image: /images/Safe_MAPF_clean.png
lead_image_alt: "Learning phase with a safe goal-conditioned RL agent, and planning phase where a MAPF planner produces waypoint paths for each agent"
lead_image_caption: "In the learning phase, a safe goal-conditioned RL agent learns to estimate distance and safety between observations. In the planning phase, a MAPF planner uses those estimates to give each agent a sequence of waypoints, which the agent follows with the shared policy."
---

Safe RL policies can learn to navigate from raw observations such as camera images, but they struggle to reach distant goals, and classical planners need a map with known distances. This work builds a graph from states the agent has already visited, uses learned value functions to estimate distance and safety along each edge, and removes edges that are too risky. CBS then plans waypoints for each agent on this graph, so **a single shared policy** can take a team of agents to distant goals safely. [Follow-up work](/publication/2026-06-28-risk-bounded-multi-agent-visual-navigation-via-iterative-risk-allocation-12) replaces this edge pruning with a risk budget shared by the team.
