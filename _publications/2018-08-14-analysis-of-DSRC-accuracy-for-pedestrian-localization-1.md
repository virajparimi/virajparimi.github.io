---
title: "Evaluating Accuracy of DSRC GPS for Pedestrian Localization in Urban Environments"
collection: publications
permalink: /publication/2018-08-14-analysis-of-DSRC-accuracy-for-pedestrian-localization
date: 2018-08-14
venue: 'RISS Working Papers Journal'
pub_type: misc
authors:
  - Aidan Lakshman*
  - Viraj Parimi*
  - Stephen F. Smith
  - Isaac K. Isukapati
summary: "Benchmarked the accuracy limits of DSRC GPS for pedestrian safety applications and fused smartphone and DSRC signals to cut low-speed localization error."
links:
  - label: Paper
    url: /files/paper1.pdf
    icon: file-pdf
    btn_class: btn--primary
abstract: |-
  Dedicated Short-Range Communications (DSRC) radios promise to reduce collisions between pedestrians and vehicles by enabling direct vehicle-to-infrastructure communication. Unfortunately, the commercial DSRC GPS units available today lose fidelity at the very walking speeds that matter most. We deployed a month-long urban field study to quantify this drift, capturing more than 20 hours of pedestrian trajectories that expose bias and variance patterns across both open-sky intersections and dense urban canyons.

  Drawing on these measurements, we designed a sensor-fusion pipeline that combines smartphone GPS, inertial sensing, and DSRC telemetry. By dynamically weighting each modality as velocity changes, the fused estimate curbs low-speed error enough to restore reliable crosswalk tracking without any hardware modifications. The resulting dataset and code offer a realistic baseline for cities planning DSRC deployments aimed at protecting vulnerable road users.
header:
  teaser: DSRC_Drift.png
  teaser_alt: "Pedestrian localization using DSRC"
lead_image: /images/DSRC_Drift.png
lead_image_alt: "Pedestrian localization using DSRC"
---

We quantify how much localization drift DSRC GPS introduces for pedestrians and show that fusing smartphone and DSRC sensors recovers reliable low-speed tracking for safety-critical interactions.
