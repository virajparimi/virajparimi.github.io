---
title: "T-HTN: Timeline based HTN Planning for Multiple Robots" 
collection: publications
permalink: /publication/2022-06-13-thtn-timeline-based-htn-planning-for-multiple-robots
date: 2022-06-13
venue: 'ICAPS | Workshop on Hierarchical Planning'
pub_type: workshop
authors:
  - Viraj Parimi
  - Zachary B. Rubinstein
  - Stephen F. Smith
summary: "Combined timeline-based scheduling with HTNs to coordinate multi-robot teams under resource constraints, yielding resilient plans compared to state-of-the-art temporal planners."
links:
  - label: Paper
    url: /files/paper5.pdf
    icon: file-pdf
    btn_class: btn--primary
  - label: Poster
    url: /files/poster1.pptx
    icon: file-image
    btn_class: btn--primary
  - label: Slides
    url: /files/slides1.pptx
    icon: file-powerpoint
  - label: Video
    url: https://www.youtube.com/watch?v=eGNyj5lOrXY
    icon: file-video
abstract: |-
  Effective coordinated actions by a team of robots operating in close proximity to one another is an important requirement in many emerging applications, ranging from warehousing and material movement to the conduct of autonomous housekeeping and maintenance of deep space habitats during unmanned periods.  Yet, such multi-robot planning problems remain a significant challenge for contemporary planning technologies, due to several complicating factors: goals must be assigned to robots and accomplished over time in the presence of complex temporal and spatial constraints in a manner that optimizes overall team performance, attention must be given to the durational uncertainty inherent in robot task execution, and planning must be responsive to changing and unexpected execution circumstances. In this paper, we present T-HTN, a novel planner that attempts to overcome this challenge by coupling the structure and efficiency of Hierarchical Task Network (HTN) models with the flexible scheduling infrastructure of timeline-based planning systems. We present initial results on a simple set of multi-robot problems that show the potential of T-HTN in comparison to a state-of-the-art PDDL-style temporal planner.
bibtex: |-
  @inproceedings{parimi2022t,
    title={T-htn: Timeline based htn planning for multiple robots},
    author={Parimi, Viraj and Rubinstein, Zachary B and Smith, Stephen F}
  }
header:
  teaser: Timeline.svg
  teaser_alt: "Multi-robot planning illustration"
lead_image: /images/Timeline.svg
lead_image_alt: "Multi-robot planning illustration"
---

T-HTN threads HTN structure with flexible timelines so multi-robot teams honor temporal deadlines, shared resources, and unexpected execution delays while keeping plans tractable.
