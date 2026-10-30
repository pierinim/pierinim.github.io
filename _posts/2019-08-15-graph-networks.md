---
title: "Graph neural networks for particle physics"
categories: [Projects]
label: "GNN"
excerpt: "Graph networks for jet tagging and particle reconstruction."
tags: [GNN, jet tagging, reconstruction]
header:
  teaser: /assets/img/projects/graph-networks.png
---

{% include figure image_path="/assets/img/projects/graph-networks.png" alt="Particle-shower reconstruction in an irregular calorimeter geometry with distance-weighted graph networks." caption="Particle-shower reconstruction in an irregular calorimeter geometry with distance-weighted graph networks. From <a href='https://arxiv.org/abs/1902.07987'>Learning representations of irregular particle-detector geometry with distance-weighted graph networks</a>." %}

Early applications of deep learning in high-energy physics turned collision data into images or sequences, which limited the performance gain. With S. R. Qasim et al. I proposed adopting graph neural networks for particle physics, and in a series of papers we showed that graph architectures on a point-cloud representation of LHC data significantly improve performance. Work in this direction includes **JEDI-net**, a jet-identification algorithm based on interaction networks, **GarNet** / distance-weighted graph networks for irregular calorimeter geometries, and their implementation on FPGAs for real-time use in the trigger.

- [JEDI-net (Eur. Phys. J. C 80 (2020) 58)](https://arxiv.org/abs/1908.05318)
- [Distance-weighted graph networks (arXiv:1902.07987)](https://arxiv.org/abs/1902.07987)
- [Optimizing GNNs for jet tagging on FPGAs (FPL 2022)](https://www.doc.ic.ac.uk/~zque/papers/22/fpl22zq.pdf)
