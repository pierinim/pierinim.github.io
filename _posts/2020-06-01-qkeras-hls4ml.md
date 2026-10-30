---
title: "QKeras and hls4ml, with Google"
categories: [Other]
label: "Industry · Google"
excerpt: "Automatic heterogeneous quantization of neural networks for ultra-low-latency inference on FPGAs."
tags: [quantization, FPGA, hls4ml, QKeras]
header:
  teaser: /assets/img/projects/qkeras-hls4ml.png
---

{% include figure image_path="/assets/img/projects/qkeras-hls4ml.png" alt="From a Keras model to FPGA firmware: QKeras quantization, AutoQKeras optimization and hls4ml synthesis." caption="From a Keras model to FPGA firmware: QKeras quantization, AutoQKeras optimization and hls4ml synthesis. From <a href='https://arxiv.org/abs/2006.10159'>Automatic heterogeneous quantization of deep neural networks for low-latency inference on the edge for particle detectors</a>." %}

Together with Google's QKeras team, we connected QKeras, Google's library for quantization-aware
training, to hls4ml. AutoQKeras searches for the best per-layer (heterogeneous) quantization under
accuracy and resource constraints, and hls4ml turns the quantized model into FPGA firmware. The
result: models that are both accurate and small and fast enough for the 40 MHz LHC Level-1
trigger. This workflow is now widely used to deploy neural networks on FPGAs in particle physics.

Selected papers:

- [Automatic heterogeneous quantization of deep neural networks for low-latency inference on the edge for particle detectors](https://arxiv.org/abs/2006.10159), Nature Mach. Intell. 3 (2021) 675
