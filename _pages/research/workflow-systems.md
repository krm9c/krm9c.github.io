---
layout: research
title: Workflow Management & Anomaly Detection
permalink: /research/workflow-systems/
banner_color: emerald
banner_image: /assets/img/workflow_management.png
nav: false
---


<div class="research-hero-image">
  <img src="{{ '/assets/img/workflow_management.png' | relative_url }}" alt="Workflow Management & Anomaly Detection">
</div>

Scientific workflows orchestrate complex computational pipelines across distributed infrastructure, but failures and anomalies can waste millions of compute hours. My research develops AI-driven methods to monitor, detect, and respond to anomalies in real-time.

**Graph Neural Networks for Workflows**: Representing workflow executions as graphs enables learning structural patterns that distinguish normal from anomalous behavior. Our GNN-based detectors achieve state-of-the-art performance on workflow anomaly benchmarks and scale to production scientific workflows.

**Large Language Models**: Exploring how LLMs can interpret workflow logs and execution traces, providing explainable anomaly detection through in-context learning without extensive retraining. This work enables rapid adaptation to new workflow types and failure modes.

**Active Learning**: Developing human-in-the-loop systems that efficiently query operators for labels on uncertain cases, dramatically reducing annotation costs while maintaining detection accuracy. This is critical for deploying ML in operational HPC environments.

**Distributed Scheduling**: Novel consensus-based and bio-inspired algorithms for job scheduling in federated computing environments, including ant colony optimization approaches that balance solution quality with computational efficiency.

This work is part of the SWARM project, reimagining scientific workflow management for distributed, federated research infrastructure across DOE national laboratories.

---

## Publications

- [SWARM: Reimagining Scientific Workflow Management Systems in a Distributed World](https://doi.org/10.1177/10943420251339317) - *IJHPCA 2025*
- [Advancing Anomaly Detection in Computational Workflows with Active Learning](https://doi.org/10.1016/j.future.2024.107608) - *Future Generation Computer Systems 2025*
- [Large Language Models for Anomaly Detection in Computational Workflows](https://doi.org/10.1109/SC41406.2024.00098) - *SC24*
- [Graph Neural Networks for Detecting Anomalies in Scientific Workflows](https://doi.org/10.1177/10943420231172140) - *IJHPCA 2023*
- [Workflow Anomaly Detection with Graph Neural Networks](https://doi.org/10.1109/WORKS56498.2022.00011) - *WORKS 2022*
- [Self-Supervised Learning for Anomaly Detection in Computational Workflows](https://arxiv.org/abs/2310.01247) - *arXiv 2023*
- [Flow-Bench: A Dataset for Computational Workflow Anomaly Detection](https://arxiv.org/abs/2306.09930) - *arXiv 2023*
- [A Greedy Consensus-Based Approach to Distributed Job Selection](https://doi.org/10.1109/CCGrid62030.2025.00017) - *CCGrid 2025*
- [Bridging Speed and Optimality in Job Scheduling: A Hybrid Ant Colony Optimization Approach](https://doi.org/10.1145/3731599.3767585) - *SC25 Workshop*
- [DISTRI: Development and Integration of Simulation Tools for Resilient Infrastructure](https://doi.org/10.1109/BigData62323.2024.10825061) - *IEEE BigData 2024*
- [DGRO: Diameter-Guided Ring Optimization for Integrated Research Infrastructure](https://arxiv.org/abs/2410.11142) - *arXiv 2024*
