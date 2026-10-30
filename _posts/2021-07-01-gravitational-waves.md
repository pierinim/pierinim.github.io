---
title: "Anomaly detection for gravitational waves"
categories: [Other]
label: "Gravitational waves"
excerpt: "Unsupervised, source-agnostic detection of gravitational-wave signals with recurrent autoencoders."
tags: [gravitational waves, anomaly detection, autoencoders, FPGA]
header:
  teaser: /assets/img/projects/gravitational-waves.png
---

{% include figure image_path="/assets/img/projects/gravitational-waves.png" alt="A simulated binary black-hole signal in LIGO-like detector noise, with the autoencoder reconstruction." caption="A simulated binary black-hole signal in LIGO-like detector noise, with the autoencoder reconstruction. From <a href='https://arxiv.org/abs/2107.12698'>Source-agnostic gravitational-wave detection with recurrent autoencoders</a>." %}

The anomaly-detection techniques we developed for the LHC trigger also apply to gravitational-wave
interferometers. Recurrent autoencoders trained on detector noise only can flag transient signals
without assuming their shape, so they are sensitive to sources that template searches would miss.
We also showed how to run these networks on FPGAs for low-latency alerts.

Selected papers:

- [Source-agnostic gravitational-wave detection with recurrent autoencoders](https://arxiv.org/abs/2107.12698), Mach. Learn.: Sci. Technol. 3 (2022) 025001
- [Accelerating recurrent neural networks for gravitational wave experiments](https://arxiv.org/abs/2106.14089) (2021)
