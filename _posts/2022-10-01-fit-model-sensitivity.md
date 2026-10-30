---
title: "FIT: a metric for model sensitivity, with CEVA"
categories: [Other]
label: "Industry · CEVA"
excerpt: "A fast, Fisher-information-based metric to predict how quantization affects a neural network."
tags: [quantization, model compression, Fisher information]
header:
  teaser: /assets/img/projects/fit-model-sensitivity.png
---

{% include figure image_path="/assets/img/projects/fit-model-sensitivity.png" alt="The FIT metric predicts the accuracy of quantized models after quantization-aware training." caption="The FIT metric predicts the accuracy of quantized models after quantization-aware training. From <a href='https://arxiv.org/abs/2210.08502'>FIT: A Metric for Model Sensitivity</a>." %}

With CEVA, a company designing processors for edge AI, we developed FIT, a metric that estimates
how sensitive a neural network is to quantization of its weights and activations. Based on Fisher
information, it is cheap to compute and lets one choose mixed-precision configurations without
retraining every candidate.

Selected papers:

- [FIT: A metric for model sensitivity](https://arxiv.org/abs/2210.08502) (B. Zandonati, A. A. Pol, M. Pierini, O. Sirkin, T. Kopetz, 2022)
