---
layout: research
title: Continual Learning
permalink: /research/continual-learning/
banner_color: indigo
banner_image: /assets/img/continual_learning.png
nav: false
---


<div class="research-hero-image">
  <img src="{{ '/assets/img/continual_learning.png' | relative_url }}" alt="Continual Learning">
</div>

Continual learning addresses the fundamental challenge of training machine learning models on sequential, non-stationary data streams while preserving knowledge from previous tasks. My research in this area focuses on:

**Theoretical Foundations**: Formalizing the stability-plasticity trade-off that governs how models balance retaining old knowledge versus acquiring new capabilities. Our NeurIPS 2021 work established mathematical bounds on the generalization-forgetting trade-off, providing principled guidance for algorithm design.

**Dynamic Programming Approaches**: Developing algorithms that treat continual learning as an optimal control problem, enabling principled decision-making about when to update, consolidate, or protect learned representations. This perspective connects classical control theory with modern deep learning.

**Scientific Applications**: Applying continual learning to real-world scientific problems including defect identification in materials science (coherent diffraction imaging at synchrotron facilities) and chemical reaction yield prediction using large language models.

Key contributions include novel regularization strategies, graph-based continual learning methods for dynamic data structures, and uncertainty-aware approaches for detecting when models encounter distribution shifts.

---

## Publications

- Formalizing the Generalization-Forgetting Trade-Off in Continual Learning - *NeurIPS 2021*
- [Continual Learning via Dynamic Programming](https://doi.org/10.1109/ICPR56361.2022.9956042) - *ICPR 2022*
- [Learning Continually on a Sequence of Graphs -- The Dynamical System Way](https://arxiv.org/abs/2305.12030) - *arXiv 2023*
- [Automated Continual Learning of Defect Identification in Coherent Diffraction Imaging](https://doi.org/10.1109/AI4S56813.2022.00007) - *AI4S 2022*
- [Automated Defect Identification in Coherent Diffraction Imaging with Smart Continual Learning](https://doi.org/10.1007/s00521-024-10415-8) - *Neural Computing and Applications 2024*
- On Understanding of the Dynamics of Model Capacity in Continual Learning - *Preprint 2024*
- [LifeLong Learning for Large Language Models in Predicting Chemical Reaction Yields](https://doi.org/10.26434/chemrxiv-2025-xtvpc) - *ChemRxiv 2025*
