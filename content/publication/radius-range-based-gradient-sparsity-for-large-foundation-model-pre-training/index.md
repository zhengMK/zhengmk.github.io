---
title: "Radius: Range-based Gradient Sparsity for Large Foundation Model Pre-training"
publication_types:
  - "1"
authors:
  - admin
  - Zhao Zhang
publication: "in *Proceedings of Machine Learning and Systems 7 (MLSys 2025)*"
publication_short: "in *MLSys 2025*"
abstract: "We present Radius, a gradient sparsity algorithm and system to accelerate large foundation model (FM) training while preserving downstream task performance. Radius leverages two key insights in large FM pre-training: 1) only a small portion of gradients contribute to the model updates in each iteration, and 2) the spatial distribution of the gradients with large magnitude is stable over time. Radius overcomes the scaling problem of existing top-k sparsity methods, as it maintains the structure of sparse gradients, which avoids dense communication in later phases of the existing top-k sparsity approaches. We examine the convergence and speed of Radius on pre-training GPT models (355M and 2.0B) in data-parallel and compare it with the existing top-k sparsification method. Our results show that using the existing top-k method with AdamW optimizer fails to converge, and the expected training speed improvement with sparse communication is marginal. In contrast, when pre-training GPT-2.0B model with 64 NVIDIA A100 GPUs, Radius with sparsity set to 40%, can reduce the per-step training time by 21% and overall pre-training time by 19%, respectively, without degradation on the evaluation scores of the downstream tasks."
draft: false
featured: false
tags:
  - Gradient Sparsity
  - LLM Training
  - Sparse Communication
categories:
  - Distributed Deep Learning
url_pdf: https://proceedings.mlsys.org/paper_files/paper/2025/file/54dd9e0cff6d9214e20d97eb2a3bae49-Paper-Conference.pdf
links:
  - name: Proceedings
    url: https://proceedings.mlsys.org/paper_files/paper/2025/hash/54dd9e0cff6d9214e20d97eb2a3bae49-Abstract-Conference.html
  - name: OpenReview
    url: https://openreview.net/forum?id=UCQPWBOWb6
date: 2025-05-12T00:00:00Z
---
