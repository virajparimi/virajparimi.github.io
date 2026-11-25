---
title: "Belief-Aware Multi-Agent Path Finding under Map Uncertainty"
collection: publications
permalink: /publication/2026-09-01-belief-aware-multi-agent-path-finding-under-map-uncertainty-13
date: 2026-09-01
venue: 'arXiv:2609.40269'
venue_short: 'Under review'
status: 'Under review, 2026'
pub_type: preprint
authors:
  - Viraj Parimi
  - Shao-Hung Chan
  - Han Zhang
  - Jingkai Chen
  - Brian C. Williams
summary: "MAGIC infers the traversability of unobserved locations from the team's shared observations and turns these beliefs into detour-aware planning costs for existing MAPF planners."
links:
  - label: arXiv
    url: https://arxiv.org/abs/2609.40269
    icon: file-pdf
    btn_class: btn--primary
header:
  teaser: MAGIC_teaser.png
  teaser_alt: "Overview of MAGIC"
lead_video: /images/highlights/magic_hw.mp4
lead_video_poster: /images/highlights/magic_hw.jpg
lead_video_alt: "Two TurtleBots running MAGIC and then optimistic replanning, with camera footage beside the planning view"
lead_video_caption: "Two TurtleBots run MAGIC and then optimistic replanning in the same room, shown at 36× speed. With MAGIC, robot 1 finds the upper passage blocked, the shared belief lowers the chance that nearby cells are open, and robot 2 heads for the lower passage straight away. With optimistic replanning, robot 2 drives to the upper passage, finds it blocked and goes around. The executed sum of costs is 20 with MAGIC and 26 with optimistic replanning."
---

Multi-Agent Gaussian belief Inference for Coordination (MAGIC) maintains a shared belief about which uncertain locations are traversable, updating it whenever robots share new observations. A Gaussian Markov random field captures spatial dependencies, and Gaussian belief propagation updates the beliefs at locations no robot has observed yet. Each edge's cost combines its direct traversal cost and its shortest bypass, weighted by the estimated traversability, so existing planners such as CBS, PBS, PIBT, and LaCAM avoid likely blockages before the robots see them.

<figure class="page__lead-media">
  <img src="/images/MAGIC.png" alt="Shared belief, local sensing and inference, and detour-aware replanning in MAGIC" loading="lazy">
  <figcaption>(a) The team shares a belief about which uncertain locations are open. (b) When an agent senses part of the map, MAGIC updates the belief at the observed locations and infers updates for nearby unobserved ones. (c) An agent replans around a likely hidden obstacle before reaching it, while an optimistic plan would run into the blockage and detour later.</figcaption>
</figure>

MAGIC achieves **a lower executed sum of costs than existing approaches on 96.3% of benchmark instances** and **scales to teams of up to 800 agents**.
