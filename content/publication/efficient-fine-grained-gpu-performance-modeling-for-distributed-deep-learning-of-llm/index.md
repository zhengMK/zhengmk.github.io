---
title: "Efficient Fine-Grained GPU Performance Modeling for Distributed Deep Learning of LLM"
publication_types:
  - "1"
authors:
  - Biyao Zhang
  - admin
  - Debargha Ganguly
  - Xuecen Zhang
  - Vikash Singh
  - Vipin Chaudhary
  - Zhao Zhang
doi: 10.1109/HiPC66333.2025.00012
publication: "in *2025 IEEE 32nd International Conference on High Performance Computing, Data, and Analytics (HiPC)*"
publication_short: "in *HiPC 2025*"
abstract: "Training Large Language Models (LLMs) is one of the most compute-intensive tasks in high-performance computing. Predicting end-to-end training time for multi-billion parameter models distributed across hundreds of GPUs remains challenging due to complex interactions between transformer components, parallelism strategies (data, model, pipeline, tensor), and multi-tier communication. Learned models require costly sampling, while analytical models often struggle with real-world network and hardware complexities. We address this by decomposing LLMs into core computational primitives and modeling them with: (1) operator-level decomposition for fine-grained analysis; (2) lightweight sampling based hardware-aware prediction models for key operations; (3) an end-to-end prediction system integrating these components across complex parallelization strategies. Crucially, our methodology has been validated on two large-scale HPC systems. Our framework achieves low average prediction errors of 4.98% on Perlmutter (A100) and 9.38% on Vista (GH200) for models up to 20B parameters across 128 GPUs. Importantly, it runs entirely on CPUs, enabling rapid iteration over hardware configurations and training strategies without costly on-cluster experimentation."
draft: false
featured: false
tags:
  - Performance Modeling
  - LLM Training
  - GPU
categories:
  - Distributed Deep Learning
url_pdf: https://arxiv.org/pdf/2509.22832
links:
  - name: arXiv
    url: https://arxiv.org/abs/2509.22832
date: 2025-12-17T00:00:00Z
---
