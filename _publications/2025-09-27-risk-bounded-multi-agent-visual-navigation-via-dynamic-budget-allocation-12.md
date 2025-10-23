---
title: "Risk-Bounded Multi-Agent Visual Navigation via Dynamic Budget Allocation" 
collection: publications
permalink: /publication/_publications/2025-09-27-risk-bounded-multi-agent-visual-navigation-via-dynamic-budget-allocation-12
date: 2025-09-27
venue: 'CoRL | Safe and Robust Learning for Operation in the Real World'
pub_type: workshop
also_in:
  - "ICAPS Workshop on Bridging the Gap Between AI Planning and Reinforcement Learning"
authors:
  - Viraj Parimi
  - Brian Williams
summary: "Dynamic CBS risk budgeting lets visual multi-agent teams push through higher-risk corridors when it pays off, delivering faster, collision-free plans while still honoring the user’s $\\Delta$ constraint."
links:
  - label: CoRL Paper
    url: /files/paper15.pdf
    icon: file-pdf
    btn_class: btn--primary
  - label: ICAPS Paper
    url: /files/paper16.pdf
    icon: file-pdf
abstract: |-
  Safe navigation is essential for autonomous systems operating in hazardous environments, especially when multiple agents must coordinate using just visual inputs over extended time horizons. Traditional planning methods excel at solving long-horizon tasks but rely on predefined distance metrics, while safe Reinforcement Learning (RL) can learn complex behaviors using high-dimensional inputs yet struggles with multi-agent, goal-conditioned scenarios. Recent work combined these paradigms by leveraging goal-conditioned RL (GCRL) to build an intermediate graph from replay buffer states, pruning unsafe edges, and using Conflict-Based Search (CBS) for multi-agent path planning. Although effective, this graph-pruning approach can be overly conservative, limiting mission efficiency by precluding missions that must traverse high‐risk regions. To address this limitation, we propose RB-CBS, a novel extension to CBS that dynamically allocates and adjusts user-specified risk bound ($\Delta$) across agents to flexibly trade off safety and speed. Our improved planner ensures that each agent receives a local risk budget ($\delta$) enabling more efficient navigation while still respecting overall safety constraints. Experimental results demonstrate that this iterative risk-allocation framework yields superior performance in complex environments, allowing multiple agents to find collision-free paths within the user-specified $\Delta$.
header:
  teaser: RBCBS.svg
  teaser_alt: "Risk-Bounded multi-agent navigation depiction"
lead_image: /images/RBCBS.svg
lead_image_alt: "Risk-Bounded  multi-agent navigation depiction"
---

Extends the CBS + goal-conditioned RL pipeline with a dynamic risk-allocation layer, so a global risk budget $\Delta$ is redistributed into per-agent budgets $\delta$ that adapt mid-plan; as agents explore hazardous regions the planner rebalances these budgets, achieving safer-yet-faster multi-agent navigation than the prior fixed-pruning approach.
