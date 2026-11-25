---
title: "Evaluating Accuracy of DSRC GPS for Pedestrian Localization in Urban Environments"
collection: publications
published: false
permalink: /publication/2018-08-14-analysis-of-DSRC-accuracy-for-pedestrian-localization
date: 2018-08-14
venue: 'RISS Working Papers Journal'
venue_short: 'RISS 2018'
pub_type: misc
authors:
  - Aidan Lakshman*
  - Viraj Parimi*
  - Stephen F. Smith
  - Isaac K. Isukapati
summary: "Finds that DSRC GPS is off by 5 to 200 meters at walking speed, far worse than phone GPS, and proposes combining the two to locate pedestrians."
links:
  - label: Paper
    url: /files/paper1.pdf
    icon: file-pdf
    btn_class: btn--primary
abstract: |-
  Dedicated Short-Range Communications (DSRC) are a standard of communications designed for vehicle-to-vehicle and vehicle-to-infrastructure communication. This technology offers significant promise for improving pedestrian safety, as it allows pedestrians to communicate directly with nearby infrastructure elements and vehicles, and offers more precise GPS localization. Our work shows the current standard is too imprecise at low speeds, and as such cannot be used for pedestrian localization. We propose a method to increase the accuracy of DSRC GPS readings at low velocities and to increase precision by utilizing both iPhone and DSRC GPS readings.
header:
  teaser: DSRC_Drift.png
  teaser_alt: "Pedestrian localization using DSRC"
lead_image: /images/DSRC_Drift.png
lead_image_alt: "Satellite map of Craig St. and Forbes Ave. with the walked path, iPhone GPS track and DSRC GPS track"
lead_image_caption: "A walking test at Craig St. and Forbes Ave. in Pittsburgh. The blue line is the path walked, green is the iPhone's GPS and red is the DSRC GPS."
---

DSRC radios let pedestrians communicate directly with vehicles and intersections, and DSRC GPS claims accuracy under 1 meter. Walking through Pittsburgh intersections with an iPhone 7 and a DSRC unit, we found that the iPhone's GPS was accurate to about 1 to 2 meters, while the DSRC GPS was off by 5 meters at best and about 200 meters at worst. At driving speeds the DSRC GPS was accurate to under half a meter, which suggests that it relies on vehicle speed to correct its position. The paper concludes that DSRC GPS is not yet precise enough to locate pedestrians and proposes combining it with phone GPS.
