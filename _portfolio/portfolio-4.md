---
title: "Lossy Compression using Neural Networks"
excerpt: "Formulated quantization techniques to generate discrete latent space representations among image and textbased autoencoder models without significant performance implications. Showcased that incorporating commit-loss to the learning process improved the compression ratio of both imageand text based models while maintaining the quality of reconstructions"
collection: portfolio
---

We used autoencoder models with discrete latent space representations to perform lossy compression of image and text based data without significant performance implicates with respect to continuous couterparts like Variational Autoencoders. To improve the compression ratio we tried a naive quantization technique followed by incorporating the quantization objective into a loss function to make the output closer to quantized numbers. Finally, we also tried a training time quantization
technique and performed extensive experiments on different image and text based datasets.
<br/><img style='margin: auto; display: block; width: 80% !important; max-width: 700px !important;' src='/images/Lossy_Compression.png'>

[[PDF]](https://viraj96.github.io/files/portfolio-4/report.pdf) [[Code]](https://github.com/divamgupta/dnn_lossy_compression)
