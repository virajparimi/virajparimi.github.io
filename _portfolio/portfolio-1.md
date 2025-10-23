---
title: "Automatic Reward Densification"
excerpt: "We implemented a system that is able to leverage classical planning over human-specified PDDL models to automatically increase the density of robotic tasks with sparse, goal-based reward."
collection: portfolio
header:
  teaser: ARD.png
  teaser_alt: "Automatic reward densification concept illustration"
lead_image: /images/ARD.png
lead_image_alt: "Reward densification pipeline across multiple robotics tasks"
summary: "Classical planning over human-specified PDDL models, combined with potential-based shaping, densifies sparse rewards and speeds up learning across robotic tasks."
project_links:
  - label: PDF
    url: /files/portfolio-1/report.pdf
    icon: file-pdf
    btn_class: btn--primary
  - label: Website
    url: http://nishanthjkumar.com/airobot_reward_densification/
    icon: globe
  - label: Code
    url: https://github.com/NishanthJKumar/airobot_reward_densification
    icon: code
  - label: Slides
    url: https://docs.google.com/presentation/d/1M5sPGWkCsGoGVnfnY0i7reYVwLuUrs1Fx4Vm10iyals/edit?usp=sharing
    icon: file-powerpoint
links:
  - label: PDF
    url: /files/portfolio-1/report.pdf
    icon: file-pdf
    btn_class: btn--primary
  - label: Website
    url: http://nishanthjkumar.com/airobot_reward_densification/
    icon: globe
  - label: Code
    url: https://github.com/NishanthJKumar/airobot_reward_densification
    icon: code
  - label: Slides
    url: https://docs.google.com/presentation/d/1M5sPGWkCsGoGVnfnY0i7reYVwLuUrs1Fx4Vm10iyals/edit?usp=sharing
    icon: file-powerpoint
---

We implemented a system that leverages classical planning over human-specified PDDL models to automatically increase the density of sparse, goal-based rewards for robotic tasks. We first revisited plan-based potential shaping for discrete domains, proved its soundness, reproduced prior methods, and evaluated them on continuous control problems with varying PDDL granularities. Building on these insights, we proposed a dynamic distance-varying potential that consistently accelerates learning across three robotic benchmarks. Our analysis highlights how model granularity and potential weighting interact, and shows that with careful tuning our shaped reward matches or exceeds handcrafted dense signals.
