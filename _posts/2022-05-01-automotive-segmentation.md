---
title: "Compressed CNNs for autonomous driving, with Zenseact"
categories: [Other]
label: "Industry · Zenseact"
excerpt: "Real-time semantic segmentation of street scenes on FPGAs, using hls4ml and aggressive quantization."
tags: [automotive, semantic segmentation, FPGA, hls4ml, quantization]
header:
  teaser: /assets/img/projects/automotive-segmentation.jpg
---

{% include figure image_path="/assets/img/projects/automotive-segmentation.jpg" alt="A street scene and its semantic segmentation computed on an FPGA." caption="A street scene and its semantic segmentation computed on an FPGA. From <a href='https://arxiv.org/abs/2205.07690'>Real-time semantic segmentation on FPGAs for autonomous vehicles with hls4ml</a>." %}

With Zenseact, the automotive software company, we applied the hls4ml tools developed for the LHC
trigger to autonomous driving: compressing a convolutional neural network for semantic segmentation
of camera images, and deploying it on an FPGA with real-time latency and low power, as needed on
board a vehicle.

Selected papers:

- [Real-time semantic segmentation on FPGAs for autonomous vehicles with hls4ml](https://arxiv.org/abs/2205.07690), Mach. Learn.: Sci. Technol. 3 (2022) 045011
