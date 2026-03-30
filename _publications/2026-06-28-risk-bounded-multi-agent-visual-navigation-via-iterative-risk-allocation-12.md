---
title: "Risk-Bounded Multi-Agent Visual Navigation via Iterative Risk Allocation" 
collection: publications
permalink: /publication/_publications/2026-06-28-risk-bounded-multi-agent-visual-navigation-via-iterative-risk-allocation-12
date: 2026-06-28
venue: "ICAPS"
pub_type: conference
also_in:
  - 'ICAPS Workshop on Bridging the Gap Between AI Planning and Reinforcement Learning (Oral)'
  - 'CoRL Workshop on Safe and Robust Learning for Operation in the Real World'
authors:
  - Viraj Parimi
  - Brian Williams
summary: "Dynamic CBS risk budgeting lets visual multi-agent teams push through higher-risk corridors when it pays off, delivering faster, collision-free plans while still honoring the user’s $\\Delta$ constraint."
links:
  - label: ICAPS Paper
    url: /files/paper17.pdf
    icon: file-pdf
    btn_class: btn--primary
  - label: CoRL Workshop Paper
    url: /files/paper15.pdf
    icon: file-pdf
    btn_class: btn--primary
  - label: ICAPS Workshop Paper
    url: /files/paper16.pdf
    icon: file-pdf
    btn_class: btn--primary
  - label: Website
    url: https://rb-safe-visual-mapf-mers.csail.mit.edu/
    icon: globe

abstract: |-
  Safe navigation is essential for autonomous systems operating in hazardous environments, especially when multiple agents must coordinate using only high-dimensional visual observations. While recent approaches successfully combine Goal-Conditioned RL (GCRL) for graph construction with Conflict-Based Search (CBS) for planning, they typically rely on deleting edges with high risk before running CBS to enforce safety. This binary strategy is overly conservative, precluding feasible missions that require traversing high-risk regions, even when the aggregate risk is acceptable. To address this, we introduce a framework for Risk-Bounded Multi-Agent Path Finding ($\Delta$-MAPF), where agents share a user-specified global risk budget ($\Delta$). Rather than permanently discarding edges, our framework dynamically distributes per-agent risk budgets ($\delta_i$) during search via an Iterative Risk Allocation (IRA) layer that integrates with a standard CBS planner. We investigate two distribution strategies: a greedy surplus-deficit scheme for rapid feasibility repair, and a market-inspired mechanism that treats risk as a priced resource to guide improved allocation. The market-based mechanism yields a tunable trade-off wherein agents exploit available risk to secure shorter, more efficient paths, but revert to longer, safer detours under tighter budgets. Experiments in complex visual environments show that our dynamic allocation framework achieves higher success rates than baselines and effectively leverages the available safety budget to reduce travel time.
header:
  teaser: RBCBS.svg
  teaser_alt: "Risk-Bounded multi-agent navigation depiction"
bibtex: |- 
  @inproceedings{parimi2026rbvisualmapf,
    author    = {Viraj Parimi and Brian C. Williams},
    title     = {Risk-Bounded Multi-Agent Visual Navigation via Iterative Risk Allocation},
    booktitle = {Proceedings of the 36th International Conference on Automated Planning and Scheduling (ICAPS 2026)},
    year      = {2026},
    address   = {Dublin, Ireland},
    note      = {To appear}
  }
lead_image: /images/RBCBS.svg
lead_image_alt: "Risk-Bounded  multi-agent navigation depiction"
---

Extends the CBS + goal-conditioned RL pipeline with a iterative risk-allocation layer, so a global risk budget $\Delta$ is redistributed into per-agent budgets $\delta$ that adapt mid-plan; as agents explore hazardous regions the planner rebalances these budgets, achieving safer-yet-faster multi-agent navigation than the prior fixed-pruning approach.
