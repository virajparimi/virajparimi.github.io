---
title: "Automatic Reward Densification"
collection: portfolio
order: 1
header:
  teaser: ARD.png
  teaser_alt: "Automatic reward densification concept illustration"
lead_image: /images/ARD.png
lead_image_alt: "Pipeline in which a human writes a PDDL model and classifiers whose plans shape the reward for training a robot arm policy"
lead_image_caption: "A human expert writes an abstract PDDL model and classifiers that map simulator states to its predicates. Plans in that model define a potential-based shaping reward for training the policy."
summary: "Uses plans from a human-written PDDL model to shape sparse robot rewards, helping PPO learn better policies than with the sparse reward alone."
links:
  - label: PDF
    url: /files/portfolio-1/report.pdf
    icon: file-pdf
    btn_class: btn--primary
  - label: Code
    url: https://github.com/NishanthJKumar/airobot_reward_densification
    icon: code
  - label: Website
    url: http://nishanthjkumar.com/airobot_reward_densification/
    icon: globe
  - label: Slides
    url: https://docs.google.com/presentation/d/1M5sPGWkCsGoGVnfnY0i7reYVwLuUrs1Fx4Vm10iyals/edit?usp=sharing
    icon: file-powerpoint
---

Robot tasks are easy to specify with a sparse goal reward but hard to learn from it, and hand-designed dense rewards invite reward hacking. In this final project for MIT 6.484 with Nishanth Kumar and Willie McClinton, a human writes a PDDL model of the task, plus classifiers that map states to its predicates, and plans in that model shape the reward. We proved that an existing plan-based potential for discrete domains is sound, reimplemented it for continuous control, and added a dynamic potential that varies with distance to the next subgoal. On reaching, pushing and maze-reaching tasks, the shaped rewards **helped PPO learn better policies** than the sparse reward did, and finer PDDL models usually helped more. Beating a hand-crafted dense reward still took careful tuning.
