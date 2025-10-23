---
title: "GitHub Recommender System" 
excerpt: "Built an implicit-feedback recommender that suggests open-source repositories, achieving 0.72 recall."
collection: portfolio
header:
  teaser: Github_Recommender_System.png
  teaser_alt: "GitHub recommender system workflow"
lead_image: /images/Github_Recommender_System.png
lead_image_alt: "Autoencoder-based GitHub recommendation pipeline"
summary: "Collected contribution signals, formed confidence-weighted implicit ratings, and trained a custom autoencoder that surfaces relevant GitHub repos for contributors."
project_links:
  - label: PDF
    url: /files/portfolio-9/report.pdf
    icon: file-pdf
    btn_class: btn--primary
  - label: Code
    url: https://github.com/divyanshu-talwar/Github-Recommender-System
    icon: code
links:
  - label: PDF
    url: /files/portfolio-9/report.pdf
    icon: file-pdf
    btn_class: btn--primary
  - label: Code
    url: https://github.com/divyanshu-talwar/Github-Recommender-System
    icon: code
---

We built an Amazon-style recommender for GitHub by mining implicit feedback signals, constructing confidence-weighted interaction matrices, and training an autoencoder with a custom loss tailored to sparse developer-repository interactions. The resulting system delivers a recall of 0.72, offering relevant open-source projects to contributors and encouraging community participation.
