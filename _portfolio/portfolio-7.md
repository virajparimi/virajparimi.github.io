---
title: "Parallel Depth First Search for Directed Acyclic Graphs"
excerpt: "Implemented a CUDA-based parallel DFS for DAGs that delivers substantial speedups over serial traversals."
collection: portfolio
header:
  teaser: Parallel_DFS.jpg
  teaser_alt: "Parallel DFS architecture on GPU"
lead_image: /images/Parallel_DFS.jpg
lead_image_alt: "CUDA kernels exploring a directed acyclic graph"
summary: "Work-efficient GPU traversal expands frontier vertices in parallel and accelerates DFS-based analytics on massive DAGs."
project_links:
  - label: PDF
    url: /files/portfolio-7/report.pdf
    icon: file-pdf
    btn_class: btn--primary
  - label: Code
    url: https://github.com/divyanshu-talwar/Parallel-DFS
    icon: code
links:
  - label: PDF
    url: /files/portfolio-7/report.pdf
    icon: file-pdf
    btn_class: btn--primary
  - label: Code
    url: https://github.com/divyanshu-talwar/Parallel-DFS
    icon: code
---

Depth-first search underpins many graph algorithms, yet its inherently sequential nature complicates parallelization. We implemented a work-efficient GPU traversal for DAGs that explores independent frontier vertices concurrently, delivering significant speedups over the serial baseline on large graphs and enabling faster topological analyses.
