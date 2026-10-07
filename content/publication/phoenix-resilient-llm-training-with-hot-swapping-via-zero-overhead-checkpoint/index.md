---
title: "PHOENIX: Resilient LLM Training with Hot-Swapping via Zero-Overhead Checkpoint"
publication_types:
  - "3"
authors:
  - Haotian Xie
  - Junlin Chen
  - admin
  - Lishan Yang
  - Zhao Zhang
publication: "*arXiv preprint arXiv:2607.01646*"
publication_short: "*arXiv*"
abstract: "State-of-the-art large language model (LLM) training takes tens of thousands of graphics processing units (GPUs) for months and encounters failures across the software and hardware stack. Existing fault-tolerance mechanisms either impose non-trivial overhead during failure-free execution or suffer from prolonged recovery latency, particularly under scenarios where a small subset of compute nodes experience permanent failures. We present PHOENIX to simultaneously address both optimization objectives. PHOENIX incorporates a fault-tolerance mechanism that restores LLM training via hot-swapping, namely by replacing failed nodes with spare nodes without terminating the complete job. The hot-swapping of PHOENIX is enabled by two ideas: First, it exploits an off-critical-path in-memory checkpointing mechanism for spatial redundancy. Second, it introduces a communicator reconstruction protocol that replaces failed nodes with spare nodes at runtime. PHOENIX efficiently overlaps the in-memory checkpointing with computation, thus introducing zero overhead during error-free execution. Upon permanent node failures, PHOENIX can rebuild memory states with minimal recomputation by leveraging in-memory checkpoints. We evaluate PHOENIX across scales (up to 512 NVIDIA A100 GPUs) and LLMs (up to 65B parameters), and observe zero checkpoint overhead with hot-swapping recovery completing in under 40 seconds. These results show that PHOENIX simultaneously achieves both zero-overhead error-free execution and extremely low recovery cost."
draft: false
featured: false
tags:
  - Fault Tolerance
  - Checkpointing
  - LLM Training
categories:
  - Distributed Deep Learning
url_pdf: https://arxiv.org/pdf/2607.01646
links:
  - name: arXiv
    url: https://arxiv.org/abs/2607.01646
date: 2026-07-02T00:00:00Z
---
