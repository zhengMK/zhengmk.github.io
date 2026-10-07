---
title: "SCAPE: Accurate and Efficient LLM Training with Extreme Sparse Communication"
publication_types:
  - "3"
authors:
  - admin
  - Junlin Chen
  - Haotian Xie
  - Zhao Zhang
publication: "*arXiv preprint arXiv:2607.01678*"
publication_short: "*arXiv*"
abstract: "Communication increasingly dominates the cost of Large Language Model (LLM) pre-training, especially under data-parallel and sharded training schemes, where gradient synchronization and parameter reconstruction overhead increase with model size and system scale. Existing communication-reduction methods either sparsify raw gradients, which can be unstable for modern Adam-style optimizers at high sparsity, or quantize communication, whose savings are fundamentally bounded by bit width and often incur additional runtime overhead. We present SCAPE, a communication-efficient distributed optimizer for LLM training that exploits the stability of AdamS's first-moment to enable aggressive sparsification without loss of LLM quality. Instead of constructing masks from raw gradients, SCAPE derives them from first-moment-based statistics, partitions mask generation across workers to align with optimizer sharding, and delays mask usage by one step so that mask synchronization can overlap with computation. SCAPE also reconstructs the quantities required for second-moment updates from a single synchronized sparse buffer, avoiding an additional collective. We implement SCAPE in Megatron-LM and evaluate its convergence by pre-training GPT-345M on OpenWebText and Llama-500M on SlimPajama-6B using 32 NVIDIA GH200 GPUs on TACC Vista. In both models, SCAPE preserves training stability, validation loss, and downstream task accuracy under 90% and 99% sparsity. For Llama-500M, SCAPE reduces end-to-end pre-training wall-clock time by up to 43.3% while maintaining model quality comparable to dense AdamW and AdamS. For Llama-1.8B, SCAPE achieves up to 3.26× speedup per step compared to dense AdamS."
draft: false
featured: false
tags:
  - Sparse Communication
  - LLM Training
  - Distributed Optimizer
categories:
  - Distributed Deep Learning
url_pdf: https://arxiv.org/pdf/2607.01678
links:
  - name: arXiv
    url: https://arxiv.org/abs/2607.01678
date: 2026-07-02T00:00:00Z
---
