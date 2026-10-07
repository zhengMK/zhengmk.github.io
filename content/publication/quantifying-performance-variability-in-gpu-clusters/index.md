---
title: "Quantifying Performance Variability in GPU Clusters"
publication_types:
  - "2"
authors:
  - Michael Mogilevsky
  - Hazem Zaky
  - Yu Sun
  - admin
  - Lishan Yang
  - Zhao Zhang
doi: 10.1109/TPDS.2026.3684387
publication: "in *IEEE Transactions on Parallel and Distributed Systems*"
publication_short: "in *IEEE TPDS*"
abstract: "Modern supercomputers are equipped with massive amounts of Graphics Processing Units (GPUs) to meet the growing demands of scientific computing and machine learning. However, GPUs, even of the same type, exhibit performance variability, leading to resource under-utilization and prolonged execution times. In this work, we perform a characterization study on the performance variability of NVIDIA A100 GPUs and GH200 superchips using the GEMM and STREAM micro-benchmarks and seven real-world applications across two supercomputing systems: TACC Vista (GH200) and NERSC Perlmutter (A100). Our results reveal GEMM performance variability ranging from 0.1% to 8.8%, though outliers can push deviations significantly higher. For scientific applications, the variability ranges from 1.0% to 12.2% on Vista. The variability of single-GPU GPT 4.8B and Llama 3B training is 10.4% and 8.9%, respectively. We further extend this study by training a GPT 19B model using eight GH200s in the 3D parallel configuration, observing up to 3.6% throughput variability and 8.5% slowdown in the worst case. By comparing the variability across GPU types, compute paths, data precisions, and applications, we observe that applications that use Tensor Cores and FP64 on CUDA cores show higher variability than other applications. Supercomputer users can leverage the observed variability to diagnose performance issues and enhance execution efficiency. Computing centers can design variability-aware scheduling approaches to achieve higher machine utilization without sacrificing individual application performance."
draft: false
featured: false
tags:
  - Performance Variability
  - GPU
  - Supercomputing
categories:
  - High Performance Computing
date: 2026-06-01T00:00:00Z
---
