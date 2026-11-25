---
title: "Belief-Aware Lifelong Multi-Agent Path Finding under Dynamic Traversability"
collection: publications
permalink: /publication/2026-10-01-belief-aware-lifelong-multi-agent-path-finding-under-dynamic-traversability-14
date: 2026-10-01
venue_short: 'Under review'
status: 'Under review, 2026'
pub_type: preprint
authors:
  - Viraj Parimi
  - Brian C. Williams
summary: "MARBLE forecasts when blocked locations will clear from online estimates of environmental change, letting lifelong MAPF planners weigh waiting against detouring under noisy sensing."
header:
  teaser: MARBLE_teaser.png
  teaser_alt: "Overview of MARBLE"
lead_video: /images/highlights/marble_full.mp4
lead_video_poster: /images/highlights/marble_full.jpg
lead_video_alt: "Four TurtleBots running MARBLE in a LEGO arena, next to a panel showing MARBLE's beliefs"
lead_video_caption: "Four TurtleBots run MARBLE in a LEGO arena while passages are blocked and cleared, shown at 2× speed. The panel on the right shows MARBLE's belief about each passage."
---

Multi-Agent Routing with Beliefs for Lifelong Execution (MARBLE) models each uncertain location's traversability as a two-state Markov chain. Noisy observations update the beliefs through Bayesian updates that account for sensor reliability, while successful and failed moves provide exact evidence. MARBLE estimates blocking and clearing rates online and shares information across nearby locations, then converts its forecasts into time-dependent planning costs for existing lifelong planners such as RHCR, PIBT, LaCAM, and LLLG.

<figure class="page__lead-media">
  <img src="/images/MARBLE.png" alt="Changing blockages, beliefs that forecast clearing, and weighing waits against detours in MARBLE" loading="lazy">
  <figcaption>(a) Agents receive new goals while passages become blocked and later clear. (b) MARBLE keeps a belief about each uncertain location, combining local sensing with information shared from nearby locations, and forecasts when a blocked passage will clear. (c) With that forecast, an agent can wait for a passage to reopen instead of taking a longer detour.</figcaption>
</figure>

With RHCR and 100 agents on five benchmark maps, MARBLE **improves throughput by 18% over reactive replanning** and 37% over a static Bayesian filter, and its advantage persists across four lifelong planners and teams of up to 1,000 agents.
