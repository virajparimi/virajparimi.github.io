---
title: "A Computationally Scalable Bayesian Sequential Learning Framework for Time-Series Forecasting"
collection: publications
permalink: /publication/2022-01-01-computationally-scalable-bayesian-sequential-learning-framework-for-time-series-forecasting
date: 2022-01-01
pub_type: misc
authors:
  - Viraj Parimi
  - Isaac K. Isukapati
  - Stephen F. Smith
summary: "Scales Bayesian sequential forecasting to real-time deployments by swapping costly MCMC with Nested Sampling, keeping accuracy high even in small, non-stationary datasets."
links:
  - label: Paper
    url: /files/paper4.pdf
    icon: file-pdf
    btn_class: btn--primary
abstract: |-
  Time-series forecasting is a widely used data science technique for predicting the future state of stochastic mechanisms. Application domains that benefit from such practices include stock markets, inventory planning, supply chain management, healthcare, and resource allocation under uncertainty. In recent years, deep learning has increasingly become the method of choice in time-series forecasting applications where historical data is abundant. Alternatively, frequentist approaches are quite popular in applications where historical data is limited, but their underlying assumption of stationary data tends to restrict their performance. This paper considers an alternative approach to small data applications, extending a Bayesian sequential learning technique to overcome this shortcoming. Historically, Bayesian learning approaches have suffered from scalability problems when applied to time-series forecasting due to the Bayesian estimation step's complexity. Contemporary Bayesian approaches utilize Markov Chain Monte Carlo methods such as Metropolis-Hastings and Hamiltonian Monte Carlo for this purpose. While these methods have proved useful for offline time-series analysis, their computational requirements limit their utility in online, high temporal frequency forecasting. We propose substituting Nested Sampling, another method for estimating Bayesian evidence, as a means of achieving a scalable time-series forecasting framework. We demonstrate our approach's effectiveness via comparative experimental analysis on three prediction problems of practical interest.
header:
  teaser: Nested_Sampling.png
  teaser_alt: "Bayesian Sequential Learning with Nested Sampling"
lead_image: /images/Nested_Sampling.png
lead_image_alt: "Bayesian Sequential Learning with Nested Sampling"
---

Develops a Bayesian sequential learning framework for time-series forecasting that replaces expensive MCMC inference with Nested Sampling, enabling scalable online predictions. By comparing against frequentist and deep-learning baselines across three real-world datasets, the authors show their approach handles limited, non-stationary data more efficiently while retaining forecasting accuracy.
