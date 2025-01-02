---
title: "Automatic Reward Densification"
excerpt: "We implemented a system that is able to leverage classical planning over humanspecified PDDL models to automatically increase the density of robotic tasks with sparse, goal-based reward"
collection: portfolio
---

We implemented a system that is able to leverage classical planning over humanspecified PDDL models to automatically increase the density of robotic tasks with sparse, goal-based reward. We proved that an existing approach (plan-based potential) used in discrete environments is theoretically sound, implemented versions of previous approaches, and evaluated their utility to help improve performance on two robotic tasks with continuous state-action spaces and PDDL models with different granularities. Inspired by these approaches, we also developed our own potential-based shaping approach (dynamic distance-varying potential) and evaluated its utility across three different robotic tasks. Our results indicate that the granularity of the PDDL model plays an important role in how useful it is, and that while using our shaped reward generally outperforms using only the original sparse reward, outperforming a handcrafted dense reward usually requires a lot of tuning of the PDDL model and weighting assigned to various terms in the potential function.
<br/><img style='margin: auto; display: block; padding: 50px; width: 80% !important; max-width: 700px !important;' src='/images/ARD.png'>

[[PDF]](https://viraj96.github.io/files/portfolio-1/report.pdf) [[Website]](http://nishanthjkumar.com/airobot_reward_densification/) [[Code]](https://github.com/NishanthJKumar/airobot_reward_densification) [[Slides]](https://docs.google.com/presentation/d/1M5sPGWkCsGoGVnfnY0i7reYVwLuUrs1Fx4Vm10iyals/edit?usp=sharing)
