---
title: "Broken Symmetry in BF16 Attention: Why FlashAttention Gradients Blow Up Late in Training"
publication_types:
  - "3"
authors:
  - Junlin Chen
  - Daize Dong
  - Huanwei Di
  - Haolong Jia
  - Jiawei Wu
  - Haotian Xie
  - admin
  - Yang Li
  - Leshang Chen
  - Huishu Wang
  - Eric P. Xing
  - Hongyi Wang
publication: "*arXiv preprint arXiv:2609.34272*"
publication_short: "*arXiv*"
abstract: "BF16 is now standard in large-scale pretraining, including in fused attention kernels such as FlashAttention, and these kernels are widely trusted. When we used FlashAttention-3 to pretrain a 450M-parameter transformer on 50B tokens, however, we ran into a problem: training was healthy for 25B tokens, then the gradient norm grew a thousandfold and the loss ended 0.2 nats above FP32 attention, without a single NaN. Recomputing the attention backward of just two layers in FP32 removes almost all of the excess gradient. Part of the cause is known: a fused multiply-add in the forward softmax, so far treated as an extreme-input NaN case and never fixed in FlashAttention-3. Repairing it stops the blow-up, but the query gradient is still wrong by more than its own size, and training still drives attention logits to thousands of times their size under accurate gradients. The remaining error comes from a broken conservation law. The softmax score gradient sums to zero along every row, which makes the query gradient blind to where the keys sit as a group; rounding it to BF16 leaves a small nonzero sum that leaks the mean key into the gradient, and the leak grows exactly as late training makes keys large and attention sharp. We introduce GProj (gauge projection), which restores the zero sum after the cast with two rank-one corrections per row. It cuts the remaining median query/key gradient errors from 219%/13% to 0.34%/0.37%, on par with FP32 attention, for 4.7% more time per training step. In matched from-scratch runs it trains to the same loss as FP32 attention, while FlashAttention-3 and key smoothing both destabilize."
draft: false
featured: false
tags:
  - Attention
  - Numerical Stability
  - LLM Training
categories:
  - Distributed Deep Learning
url_pdf: https://arxiv.org/pdf/2609.34272
links:
  - name: arXiv
    url: https://arxiv.org/abs/2609.34272
date: 2026-09-28T00:00:00Z
---
