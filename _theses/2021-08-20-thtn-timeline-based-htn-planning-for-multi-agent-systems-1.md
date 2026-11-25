---
title: "T-HTN: Timeline based HTN Planning for Multi-Agent Systems" 
collection: theses
permalink: /thesis/2021-08-20-thtn-timeline-based-htn-planning-for-multi-agent-systems 
date: 2021-08-20
venue: "Master's Thesis, Carnegie Mellon University"
authors:
  - Viraj Parimi
summary: "Extends hierarchical task networks with flexible timelines to schedule multi-robot teams that share resources and face deadlines in deep-space habitats."
links:
  - label: Thesis PDF
    url: /files/thesis1.pdf
    icon: file-pdf
    btn_class: btn--primary
  - label: Code
    url: https://github.com/virajparimi/thtn
    icon: code
abstract: |-
  Planning in mission-critical systems like deep-space habitats with onboard robotic systems must be robust to unforeseen circumstances. Such systems are expected to complete a set of goals with different deadlines each day for routine maintenance while also accounting for emergencies. With the presence of humans within the habitat, the robotic systems can be required to perform specific tasks while possibly collaborating with the humans. Further, since the habitat can support multiple robots, this becomes a source of contention as they have to share the limited set of onboard resources. This dynamic between the humans, robots, and the habitat generates a complex system where failures at any level can cause significant delays leading to temporal uncertainty. Such delays can have huge implications depending on whether or not the delay causes the system to miss a goal’s deadline. Hence, it becomes crucial for the planner to address the overall schedule within the context of the current temporal deadlines of the goals and the resource constraints within the environment. Assuming a known map of the environment and a fixed horizon time, one can develop a schedule for the robotic systems that accounts for such temporal uncertainty and resource constraints by leveraging the timeline-based planning framework. To this end, this thesis proposes T-HTN, a novel planner that extends the Hierarchical Task Networks (HTN) model by incorporating temporal reasoning via flexible timeline structures to produce plans that respect the goal’s deadlines and the complex resource constraints introduced in multi-robot scenarios. T-HTN is a robust extension to a timeline-based planner whose efficacy has been tested on multiple example scenarios within a simulation environment.
bibtex: |-
  @mastersthesis{parimi2021thtn,
    title  = {{T-HTN}: Timeline Based {HTN} Planning for Multi-Agent Systems},
    author = {Parimi, Viraj},
    school = {Carnegie Mellon University},
    year   = {2021}
  }
header:
  teaser: THTN.png
  teaser_alt: "Multi-robot planning illustration"
lead_image: /images/THTN.png
lead_image_alt: "A functional method definition whose parameters feed a wrapper function around an external planner that returns actions"
lead_image_caption: "A functional method in T-HTN's domain language. The task it defines, clearing the rail so a robot can move to a block, is handed to a wrapper around a specialized external planner, which returns the actions and their timing constraints."
---

Robots that maintain a deep space habitat must meet each goal's deadline while sharing limited onboard resources, and a delay anywhere in the system can push a goal past its deadline. T-HTN extends hierarchical task network planning with flexible timelines, plans by allocating robots and other resources to tasks, and hands specialized subproblems, such as moving along a shared rail, to external planners. In simulated multi-robot scenarios it **plans faster than the POPF temporal planner**. A shorter version of this work appeared at the [ICAPS 2022 workshop on hierarchical planning](/publication/2022-06-13-thtn-timeline-based-htn-planning-for-multiple-robots).
