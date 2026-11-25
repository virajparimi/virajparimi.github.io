---
title: "MoMo: Conditioned Contrastive Representation Learning for Preference-Modulated Planning"
collection: publications
permalink: /publication/2026-05-01-momo-conditioned-contrastive-representation-learning-for-preference-modulated-planning-16
date: 2026-05-01
venue: 'arXiv:2605.08512'
venue_short: 'Under review'
status: 'Under review, 2026'
pub_type: preprint
also_in:
  - 'ICAPS PRL 2026 (Talk)'
authors:
  - Yusuf Syed
  - Viraj Parimi
  - Brian C. Williams
summary: "Preference-conditioned contrastive representations let the tradeoff between path efficiency and risk exposure be adjusted at inference time, without retraining."
links:
  - label: arXiv
    url: https://arxiv.org/abs/2605.08512
    icon: file-pdf
    btn_class: btn--primary
header:
  teaser: MoMo_teaser.png
  teaser_alt: "Conservative and aggressive plans from MoMo"
lead_image: /images/MoMo_quad.png
lead_image_alt: "MoMo plans for risk preferences from 0.01 to 0.99, compared with IvI"
lead_image_caption: "Plans as the risk preference Δ moves from conservative (0.01) to aggressive (0.99), compared with IvI (Eysenbach et al., 2025)."
---

Contrastive representation learning can reduce long-horizon planning to inference in a low-dimensional linear system, but existing contrastive planners learn a single latent geometry and return one behavior for each start and goal. MoMo conditions both the representation geometry and the latent transition operator on a scalar preference, using Feature-Wise Linear Modulation for the encoder and low-rank modulation for the operator. A user can then shift plans between conservative and aggressive **at inference time without retraining**. The conditioning preserves the density ratio that contrastive planning relies on, so planning stays as efficient as before.

Across six environments with point, drone, quadruped and robot-arm agents, MoMo adapts plan safety smoothly to the preference and is more consistent over time and across preferences than baselines that append the preference to the state.

<figure class="page__lead-media">
  <img src="/images/MoMo_ant.png" alt="MoMo plans in an indoor navigation scene for risk preferences from 0.01 to 0.99" loading="lazy">
  <figcaption>The same sweep for a quadruped Ant robot in an indoor scene from AI Habitat.</figcaption>
</figure>

<figure class="page__lead-media">
  <img src="/images/MoMo_ur5.png" alt="MoMo motions for a UR5 arm for risk preferences from 0.01 to 0.99" loading="lazy">
  <figcaption>The same sweep for a UR5 arm, from lifting over the divider to passing through the slot.</figcaption>
</figure>
