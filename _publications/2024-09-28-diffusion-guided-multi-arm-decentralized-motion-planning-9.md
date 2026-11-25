---
title: "Diffusion-Guided Multi-Arm Decentralized Motion Planning" 
collection: publications
published: false
permalink: /publication/2024-09-28-diffusion-guided-multi-arm-decentralized-motion-planning
date: 2024-09-28
venue: 'Northeast Robotics Colloquium (NERC)'
venue_short: 'NERC 2024'
pub_type: workshop
authors:
  - Viraj Parimi
  - Annabel Gomez
  - Howard Chen
  - Andreas Hofmann
  - Brian C. Williams
summary: "Proposes decentralized diffusion policies for multi-arm motion planning that predict nearby arms' actions, avoiding costly collision checks between roadmaps."
links:
  - label: Paper
    url: /files/paper9.pdf
    icon: file-pdf
    btn_class: btn--primary
  - label: Poster
    page_only: true
    url: /files/poster1.pdf
    icon: file-image
header:
  teaser: Diff_De_Central_MP.png
  teaser_alt: "Diffusion-guided motion planning visual"
lead_image: /images/Diff_De_Central_MP.png
lead_image_alt: "Each arm's observations and those of the other arms pass through LSTM cells into a diffusion model that outputs actions"
lead_image_caption: "Each arm's policy encodes its own observation and those of the other arms with LSTM cells, and a diffusion model turns that encoding into the arm's next action."
---

Roadmap-based multi-arm planners check every pair of roadmap nodes for collisions before running MAPF, and this step can make even a simple pick-and-place task take hours. This abstract proposes replacing the roadmaps with a decentralized diffusion policy. Each arm encodes the observations of all arms and predicts what nearby arms will do, and an actor-critic signal from reinforcement learning teaches the policy about near-collisions that expert demonstrations rarely contain. The poster's next step, combining a learned diffusion model with MAPF planners, became [DG-MAP](/publication/2025-09-27-diffusion-guided-multi-arm-motion-planning-11).
