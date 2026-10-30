---
layout: post
title: "Real-time anomaly detection at the CMS Level-1 trigger"
categories: [Projects]
label: "Trigger"
summary: "Unsupervised new-physics detection at 40 MHz in CMS."
tags: [anomaly detection, trigger, FPGA, CMS]
---

Can we look for new physics without knowing what it looks like? My group has been developing unsupervised (anomaly-detection) algorithms that run on FPGAs in the CMS Level-1 trigger, inspecting the 40 million collisions per second produced by the LHC.

The line of work started with *Variational autoencoders for new physics mining at the LHC* (2018) and *Autoencoders on FPGAs for real-time, unsupervised new physics detection at 40 MHz* (2021), and led to the anomaly-detection triggers **AXOL1TL** and **CICADA**, deployed by CMS in 2023. During 2024 data taking these algorithms selected more than four billion collision events. Recent work explores knowledge distillation of normalising flows into compact FPGA-ready models.

- [CERN Courier: Hunting anomalies with an AI trigger](https://cerncourier.com/a/hunting-anomalies-with-an-ai-trigger/)
- [arXiv:2609.15295 — Knowledge distillation of a normalising flow for real-time anomaly detection at the CMS L1 trigger](https://arxiv.org/abs/2609.15295)
