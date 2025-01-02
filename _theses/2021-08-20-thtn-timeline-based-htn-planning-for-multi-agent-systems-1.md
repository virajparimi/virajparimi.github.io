---
title: "T-HTN: Timeline based HTN Planning for Multi-Agent Systems" 
collection: theses
permalink: /thesis/2021-08-20-thtn-timeline-based-htn-planning-for-multi-agent-systems 
date: 2021-08-20
venue: 'Masters Thesis | Carnegie Mellon University'
---

Planning in mission-critical systems like deep-space habitats with onboard robotic systems must be robust to unforeseen circumstances. Such systems are expected to complete a set of goals with different deadlines each day for routine maintenance while also accounting for emergencies. With the presence of humans within the habitat, the robotic systems can be required to perform specific tasks while possibly collaborating with the humans. Further, since the habitat can support multiple robots, this becomes a source of contention as they have to share the limited set of onboard resources. This dynamic between the humans, robots, and the habitat generates a complex system where failures at any level can cause significant delays leading to temporal uncertainty. Such delays can have huge implications depending on whether or not the delay causes the system to miss a goal’s deadline. Hence, it becomes crucial for the planner to address the overall schedule within the context of the current temporal deadlines of the goals and the resource constraints within the environment. Assuming a known map of the environment and a fixed horizon time, one can develop a schedule for the robotic systems that accounts for such temporal uncertainty and resource constraints by leveraging the timeline-based planning framework. To this end, this thesis proposes T-HTN, a novel planner that extends the Hierarchical Task Networks (HTN) model by incorporating temporal reasoning via flexible timeline structures to produce plans that respect the goal’s deadlines and the complex resource constraints introduced in multi-robot scenarios. T-HTN is a robust extension to a timeline-based planner whose efficacy has been tested on multiple example scenarios within a simulation environment.

[[Paper]](https://viraj96.github.io/files/paper4.pdf)
