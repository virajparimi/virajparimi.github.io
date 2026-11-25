---
title: "A Scalable Configuration-Search Framework for Multi-Agent Path Finding with Precedence Constraints"
collection: publications
permalink: /publication/2026-08-01-scalable-configuration-search-framework-for-mapf-with-precedence-constraints-15
date: 2026-08-01
venue_short: 'Under review'
status: 'Under review, 2026'
pub_type: preprint
authors:
  - Viraj Parimi
  - Brian C. Williams
summary: "Extends configuration-based search to precedence-constrained goals by tracking task progress and donating priority to the robots that must finish prerequisites, scaling to 6,000 robots."
header:
  teaser: MAPF_PC_runtime.png
  teaser_alt: "Runtime against instances solved for CBS-PC, PBS-PC, PIBT-PC, LaCAM-PC, and LaCAM*-PC"
lead_video: /images/highlights/mapfpc_maze.mp4
lead_video_poster: /images/highlights/mapfpc_maze.jpg
lead_video_alt: "CBS-PC showing no solution next to PIBT-PC moving 17 robots through a maze"
lead_video_caption: "On a maze with 17 robots, CBS-PC finds no solution within the 30-second limit, while PIBT-PC plans in under a millisecond."
---

Existing solvers for MAPF with precedence constraints plan complete paths for individual robots and have been shown to handle only dozens (CBS-PC) or hundreds (PBS-PC) of robots. This work generates one joint move at a time while tracking both robot positions and task progress, and introduces precedence donation, which transfers priority from a robot waiting on an unfinished prerequisite to the robot responsible for completing it. PIBT-PC generates joint moves efficiently, LaCAM-PC embeds it in lazy configuration search for completeness, and LaCAM\*-PC adds anytime improvement and eventual optimality.

<figure class="page__lead-media">
  <img src="/images/MAPF_PC.png" alt="Joint-move planning lets a robot step aside while still completing goal A before goal B" loading="lazy">
  <figcaption>(a) When the precedence order decides which robot goes first, robot 1 is planned first and parks at A, which seals robot 2 in the dead end with no path to B. (b) Planning one joint move at a time lets robot 1 step aside so that robot 2 can leave the dead end first, and A is still completed before B.</figcaption>
</figure>

Across 5,020 instances on fourteen maps, LaCAM\*-PC **solves 91.7% of instances within 30 seconds**, compared with 24.0% for PBS-PC and 2.6% for CBS-PC, and the planners **scale to warehouse instances with 6,000 robots and 12,000 goals**.

<figure class="page__lead-media" style="max-width: 560px; margin-left: auto; margin-right: auto;">
  <img src="/images/MAPF_PC_runtime.png" alt="Runtime against the percentage of 5,020 instances solved for each planner" loading="lazy">
  <figcaption>Runtime against the share of the 5,020 benchmark instances solved by each planner.</figcaption>
</figure>
