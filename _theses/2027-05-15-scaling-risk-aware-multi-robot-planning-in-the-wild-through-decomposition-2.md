---
title: "Scaling Risk-Aware Multi-Robot Planning in the Wild through Decomposition"
collection: theses
permalink: /thesis/2027-05-15-scaling-risk-aware-multi-robot-planning-in-the-wild-through-decomposition
date: 2027-05-15
venue: 'Ph.D. Thesis, Massachusetts Institute of Technology'
status: 'In progress, expected May 2027'
authors:
  - Viraj Parimi
summary: "Extends MAPF beyond its idealized assumptions to real-world multi-robot planning, covering shared environmental beliefs, shared risk budgets, task dependencies, learned visual navigation and learned multi-arm motion, at the scale of thousands of mobile robots and robot arms."
header:
  teaser: PhD_Thesis_teaser.jpg
  teaser_alt: "TurtleBots in LEGO arenas, robot arms around a shared bin, and a field of 10,000 arms"
lead_image: /images/PhD_Thesis.jpg
lead_image_alt: "TurtleBots in LEGO arenas, robot arms around a shared bin, and a field of 10,000 arms"
lead_image_caption: "In the top row, TurtleBots run MARBLE and PACT plans in a LEGO arena. In the bottom row, robot arms coordinate with DG-MAP, and distilled decentralized policies control 10,000 arms."
---

Planning for robot teams in the wild involves two intertwined challenges. Methods must scale to large teams, and they must handle interactions beyond collisions as well as individual robots that plan from visual observations or move articulated bodies. This thesis retains the separation that makes MAPF scalable. An agent runs each robot's goal-sense-act loop, and **a team coordinator manages the couplings between robots** by shaping each agent's goals, constraints, and costs.

### Team-level coordination (Part I)
- Planning costs from shared environmental beliefs ([MAGIC](/publication/2026-09-01-belief-aware-multi-agent-path-finding-under-map-uncertainty-13) and [MARBLE](/publication/2026-10-01-belief-aware-lifelong-multi-agent-path-finding-under-dynamic-traversability-14)).
- Shared risk budgets reallocated during conflict-based search ([Risk-Bounded Multi-Agent Visual Navigation](/publication/2026-06-28-risk-bounded-multi-agent-visual-navigation-via-iterative-risk-allocation-12), ICAPS 2026).
- Task assignment and precedence constraints ([configuration search for MAPF-PC](/publication/2026-08-01-scalable-configuration-search-framework-for-mapf-with-precedence-constraints-15) and [PACT](/publication/2026-03-01-large-neighborhood-search-for-multi-agent-task-assignment-and-path-finding-with-precedence-constraints-17)).

### Richer individual-agent capabilities (Part II)
- Multi-robot navigation from visual observations ([Safe Multi-Agent Navigation](/publication/2025-05-19-safe-multi-agent-navigation-guided-by-goal-conditioned-safe-reinforcement-learning-10), ICRA 2025).
- Learned motion generation for multi-arm coordination ([DG-MAP](/publication/2025-09-27-diffusion-guided-multi-arm-motion-planning-11), CoRL 2025).
- Distilling coordination into decentralized policies that act without online search (Distilled DG-MAP, in progress).
