---
title: "Large Neighborhood Search for Multi-Agent Task Assignment and Path Finding with Precedence Constraints"
collection: publications
permalink: /publication/2026-03-01-large-neighborhood-search-for-multi-agent-task-assignment-and-path-finding-with-precedence-constraints-17
date: 2026-03-01
venue: 'arXiv:2603.28968'
venue_short: 'Under review'
status: 'Under review, 2026'
pub_type: preprint
authors:
  - Viraj Parimi
  - Brian C. Williams
summary: "PACT reassigns precedence-related tasks with large neighborhood search and repairs only the affected robots' paths with existing MAPF-PC solvers, cutting precedence waits."
links:
  - label: arXiv
    url: https://arxiv.org/abs/2603.28968
    icon: file-pdf
    btn_class: btn--primary
header:
  teaser: PACT.png
  teaser_alt: "Fixed and flexible task assignment under precedence constraints"
lead_video: /images/highlights/pact_hw.mp4
lead_video_poster: /images/highlights/pact_hw.jpg
lead_video_alt: "Four TurtleBots running the PBS-PC plan and then the PACT plan in a LEGO arena, with the grid view beside the camera"
lead_video_caption: "Four TurtleBots run the PBS-PC plan with a fixed assignment and then the PACT plan for the same 14 tasks, shown at 9× speed. The on-screen label Global-PBS is PACT's best configuration. PACT's plan finishes in 8 timesteps instead of 15, and its sum of costs is 21 against 49 for PBS-PC."
---

When task assignments are not fixed in advance, reassigning a task under precedence constraints changes both travel distances and when dependent tasks can begin. Precedence-Aware Coordination of Tasks (PACT) improves an initial fixed-assignment solution with large neighborhood search. Two precedence-aware operators, Precedence-Wait and Low-Slack, choose which tasks to reconsider, and each neighborhood is expanded to include all downstream tasks. Rather than replanning the whole team, PACT repairs only the affected robots with existing MAPF-PC solvers, so it can evaluate the routing and timing consequences of each reassignment before accepting it.

<figure class="page__lead-media">
  <img src="/images/PACT.png" alt="Assigning each robot one precedence chain removes an 11-step wait and lowers the sum of costs from 24 to 14" loading="lazy">
  <figcaption>(a) With a fixed assignment, robot a1 must visit g2 then g4 and robot a2 must visit g3 then g1. Because g1 must come before g2, a1 waits 11 steps at g2, and the sum of costs is 24. (b) Giving each robot one precedence chain removes the wait and lowers the sum of costs to 14.</figcaption>
</figure>

With up to 500 robots and 1,600 tasks, PACT **improves 89.1% of fixed-assignment solutions** with **a median 12.3% reduction in the sum of costs**, while an LNS baseline with greedy regret-based repair achieves a median reduction of 0%.
