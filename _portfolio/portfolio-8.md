---
title: "COTTON: A Light-Weight Work-Stealing Runtime"
excerpt: "Developed an energy-aware async-finish runtime that adjusts CPU frequency via task-aware heuristics without sacrificing performance."
collection: portfolio
header:
  teaser: COTTON.png
  teaser_alt: "COTTON runtime architecture"
lead_image: /images/COTTON.png
lead_image_alt: "Energy-aware work-stealing scheduler overview"
summary: "COTTON couples work stealing with CPU frequency scaling policies tuned by task heuristics, cutting energy use while preserving throughput."
project_links:
  - label: PDF
    url: /files/portfolio-8/report.pdf
    icon: file-pdf
    btn_class: btn--primary
  - label: Code
    url: https://github.com/dattatreya303/COTTON
    icon: code
links:
  - label: PDF
    url: /files/portfolio-8/report.pdf
    icon: file-pdf
    btn_class: btn--primary
  - label: Code
    url: https://github.com/dattatreya303/COTTON
    icon: code
---

COTTON is a lightweight work-stealing runtime for async-finish parallel programs that we augmented with energy-saving policies. By combining Linux power-saving drivers with task-aware heuristics that tune CPU frequency via `cpufreq`, the runtime reduces energy consumption while preserving performance across benchmarks.
