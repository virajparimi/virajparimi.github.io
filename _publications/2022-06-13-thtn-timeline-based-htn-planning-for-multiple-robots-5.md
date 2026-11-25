---
title: "T-HTN: Timeline Based HTN Planning for Multiple Robots" 
collection: publications
permalink: /publication/2022-06-13-thtn-timeline-based-htn-planning-for-multiple-robots
date: 2022-06-13
venue: 'ICAPS Workshop on Hierarchical Planning (HPlan)'
venue_short: 'ICAPS HPlan 2022'
pub_type: workshop
authors:
  - Viraj Parimi
  - Zachary B. Rubinstein
  - Stephen F. Smith
summary: "Combines timeline-based scheduling with hierarchical task networks to plan for multi-robot teams that share resources and face deadlines."
links:
  - label: Paper
    url: /files/paper5.pdf
    icon: file-pdf
    btn_class: btn--primary
  - label: Poster
    page_only: true
    url: /files/poster1.pptx
    icon: file-image
  - label: Slides
    page_only: true
    url: /files/slides1.pptx
    icon: file-powerpoint
  - label: Video
    page_only: true
    url: https://www.youtube.com/watch?v=eGNyj5lOrXY
    icon: file-video
  - label: Code
    url: https://github.com/virajparimi/thtn
    icon: code
abstract: |-
  Effective coordinated actions by a team of robots operating in close proximity to one another is an important requirement in many emerging applications, ranging from warehousing and material movement to the conduct of autonomous housekeeping and maintenance of deep space habitats during unmanned periods.  Yet, such multi-robot planning problems remain a significant challenge for contemporary planning technologies, due to several complicating factors: goals must be assigned to robots and accomplished over time in the presence of complex temporal and spatial constraints in a manner that optimizes overall team performance, attention must be given to the durational uncertainty inherent in robot task execution, and planning must be responsive to changing and unexpected execution circumstances. In this paper, we present T-HTN, a novel planner that attempts to overcome this challenge by coupling the structure and efficiency of Hierarchical Task Network (HTN) models with the flexible scheduling infrastructure of timeline-based planning systems. We present initial results on a simple set of multi-robot problems that show the potential of T-HTN in comparison to a state-of-the-art PDDL-style temporal planner.
bibtex: |-
  @inproceedings{parimi2022thtn,
    title     = {{T-HTN}: Timeline Based {HTN} Planning for Multiple Robots},
    author    = {Parimi, Viraj and Rubinstein, Zachary B. and Smith, Stephen F.},
    booktitle = {ICAPS Workshop on Hierarchical Planning (HPlan)},
    year      = {2022}
  }
header:
  teaser: Timeline.svg
  teaser_alt: "Multi-robot planning illustration"
lead_image: /images/Timeline.svg
lead_image_alt: "Timelines for two robot arms, five rail blocks and a box, linked by constraint arrows"
lead_image_caption: "T-HTN's timelines for the running example, where arm ur5A moves a box along the rail. Each robot, rail block and the box has its own timeline, and arrows link each action on a robot's timeline to the rail blocks and box states it depends on."
---

Robot teams that work in close proximity, such as arms sharing a rail in a deep space habitat, must assign goals to robots, respect temporal and spatial constraints, and replan when execution goes wrong. T-HTN combines hierarchical task network models with the timelines used by timeline-based schedulers, and it builds a plan by allocating resources such as robots and rail blocks to tasks. On problems where two UR5 arms on a shared rail move 5 to 25 objects, T-HTN **finds a plan for every problem size within 18 seconds**, and its plans are usually shorter. The POPF temporal planner **hits its 10-minute limit on 13 of the 25 problem sizes**.
