---
title: "Lossy Compression using Neural Networks"
excerpt: "Formulated quantization techniques for discrete latent autoencoders that compress image and text data without sacrificing reconstruction quality."
collection: portfolio
header:
  teaser: Lossy_Compression.png
  teaser_alt: "Autoencoder-based lossy compression overview"
lead_image: /images/Lossy_Compression.png
lead_image_alt: "Neural lossy compression architecture"
summary: "Tested quantization-aware autoencoders that couple commit loss and training-time discretization to achieve compact latent codes for images and text."
project_links:
  - label: PDF
    url: /files/portfolio-4/report.pdf
    icon: file-pdf
    btn_class: btn--primary
  - label: Code
    url: https://github.com/divamgupta/dnn_lossy_compression
    icon: code
links:
  - label: PDF
    url: /files/portfolio-4/report.pdf
    icon: file-pdf
    btn_class: btn--primary
  - label: Code
    url: https://github.com/divamgupta/dnn_lossy_compression
    icon: code
---

We built autoencoder models with discrete latent spaces to perform lossy compression of images and text while retaining quality comparable to continuous counterparts such as VAEs. After benchmarking naive post-hoc quantization, we incorporated quantization objectives (commit loss) directly into training and explored training-time discretization strategies. Experiments across multiple datasets show that the quantization-aware variants significantly improve compression ratios with minimal degradation in reconstructions.
