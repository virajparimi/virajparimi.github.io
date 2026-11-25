---
title: "Risk-Bounded Multi-Agent Visual Navigation via Iterative Risk Allocation" 
collection: publications
permalink: /publication/2026-06-28-risk-bounded-multi-agent-visual-navigation-via-iterative-risk-allocation-12
redirect_from:
  - /publication/_publications/2026-06-28-risk-bounded-multi-agent-visual-navigation-via-iterative-risk-allocation-12
date: 2026-06-28
venue: "International Conference on Automated Planning and Scheduling (ICAPS)"
venue_short: 'ICAPS 2026'
pub_type: conference
also_in:
  - 'ICAPS PRL 2025 (Talk)'
  - 'CoRL SAFE-ROL 2025'
authors:
  - Viraj Parimi
  - Brian C. Williams
summary: "Reallocates a team-wide risk budget among robots during conflict-based search, so robots navigating from visual observations can take shorter, riskier routes when the budget allows."
links:
  - label: Paper
    url: https://doi.org/10.1609/icaps.v36i1.42829
    icon: file-pdf
    btn_class: btn--primary
  - label: arXiv (with appendix)
    page_only: true
    url: https://arxiv.org/abs/2509.08157
    icon: file-pdf
  - label: Code
    url: https://github.com/virajparimi/rb-safe-visual-mapf
    icon: code
  - label: Website
    url: https://rb-safe-visual-mapf-mers.csail.mit.edu/
    icon: globe

abstract: |-
  Safe navigation is essential for autonomous systems operating in hazardous environments, especially when multiple agents must coordinate using only high-dimensional visual observations. While recent approaches successfully combine Goal-Conditioned RL (GCRL) for graph construction with Conflict-Based Search (CBS) for planning, they typically rely on deleting edges with high risk before running CBS to enforce safety. This binary strategy is overly conservative, precluding feasible missions that require traversing high-risk regions, even when the aggregate risk is acceptable. To address this, we introduce a framework for Risk-Bounded Multi-Agent Path Finding ($\Delta$-MAPF), where agents share a user-specified global risk budget ($\Delta$). Rather than permanently discarding edges, our framework dynamically distributes per-agent risk budgets ($\delta_i$) during search via an Iterative Risk Allocation (IRA) layer that integrates with a standard CBS planner. We investigate two distribution strategies: a greedy surplus-deficit scheme for rapid feasibility repair, and a market-inspired mechanism that treats risk as a priced resource to guide improved allocation. The market-based mechanism yields a tunable trade-off wherein agents exploit available risk to secure shorter, more efficient paths, but revert to longer, safer detours under tighter budgets. Experiments in complex visual environments show that our dynamic allocation framework achieves higher success rates than baselines and effectively leverages the available safety budget to reduce travel time.
header:
  teaser: RBCBS_teaser.png
  teaser_alt: "Risk-Bounded multi-agent navigation depiction"
bibtex: |-
  @inproceedings{parimi2026risk,
    title     = {Risk-Bounded Multi-Agent Visual Navigation via Iterative Risk Allocation},
    author    = {Parimi, Viraj and Williams, Brian C.},
    booktitle = {Proceedings of the International Conference on Automated Planning and Scheduling (ICAPS)},
    volume    = {36},
    pages     = {200--209},
    year      = {2026},
    doi       = {10.1609/icaps.v36i1.42829}
  }
lead_video: /images/highlights/rbcbs_sim.mp4
lead_video_poster: /images/highlights/rbcbs_sim.jpg
lead_video_alt: "Four simulated Crazyflie drones navigating around a central obstacle and through an apartment scene"
lead_video_caption: "Four simulated Crazyflie drones follow RB-CBS paths around a central obstacle (left) and through an apartment scene (right), sped up."
---

Earlier work on [safe visual navigation](/publication/2025-05-19-safe-multi-agent-navigation-guided-by-goal-conditioned-safe-reinforcement-learning-10) kept robots safe by deleting high-risk edges from the waypoint graph before planning, which rules out missions that must cross risky regions even when the total risk is acceptable. This work instead gives the team **one shared risk budget** and reallocates it between robots during conflict-based search, so robots can take shorter routes through hazardous areas whenever the total risk stays within the budget.

<figure class="page__lead-media">
  <img src="/images/RBCBS.svg" alt="Paths from four baselines and from RB-CBS at three global risk budgets" loading="lazy">
  <figcaption>Paths from four baselines and from RB-CBS at global risk budgets Δ of 0%, 5% and 25%. As the budget grows, RB-CBS accepts more risk in exchange for shorter paths.</figcaption>
</figure>
