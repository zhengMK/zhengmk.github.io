---
title: "COMPSO: Optimizing Gradient Compression for Distributed Training with Second-Order Optimizers"
publication_types:
  - "1"
authors:
  - Baixi Sun
  - Weijin Liu
  - J. Gregory Pauloski
  - Jiannan Tian
  - Jinda Jia
  - Daoce Wang
  - Boyuan Zhang
  - admin
  - Sheng Di
  - Sian Jin
  - Zhao Zhang
  - Xiaodong Yu
  - Kamil A. Iskra
  - Pete Beckman
  - Guangming Tan
  - Dingwen Tao
doi: 10.1145/3710848.3710852
publication: "in *Proceedings of the 30th ACM SIGPLAN Annual Symposium on Principles and Practice of Parallel Programming*"
publication_short: "in *PPoPP 2025*"
abstract: "Second-order optimization methods have been developed to enhance convergence and generalization in deep neural network (DNN) training compared to first-order methods like Stochastic Gradient Descent (SGD). However, these methods face challenges in distributed settings due to high communication overhead. Gradient compression, a technique commonly used to accelerate communication for first-order approaches, often results in low communication reduction ratios, decreased model accuracy, and/or high compression overhead when applied to second-order methods. To address these limitations, we introduce a novel gradient compression method for second-order optimizers called COMPSO. This method effectively reduces communication costs while preserving the advantages of second-order optimization. COMPSO employs stochastic rounding to maintain accuracy and filters out minor gradients to improve compression ratios. Additionally, we develop GPU optimizations to minimize compression overhead and performance modeling to ensure end-to-end performance gains across various systems. Evaluation of COMPSO on different DNN models shows that it achieves a compression ratio of 22.1×, reduces communication time by 14.2×, and improves overall performance by 1.9×, all without any drop in model accuracy."
draft: false
featured: false
tags:
  - Gradient Compression
  - Second-Order Optimization
  - Distributed Training
categories:
  - Distributed Deep Learning
date: 2025-02-28T00:00:00Z
---
