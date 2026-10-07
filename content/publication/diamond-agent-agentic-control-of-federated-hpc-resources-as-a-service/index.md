---
title: "Diamond Agent: Agentic Control of Federated HPC Resources as a Service"
publication_types:
  - "3"
authors:
  - Haotian Xie
  - Junlin Chen
  - admin
  - Yifan Zhu
  - Minu Mathew
  - Max Burnette
  - Yadu Babuji
  - Volodymyr Kindratenko
  - Shivaram Venkataraman
  - Kyle Chard
  - Ian Foster
  - Zhao Zhang
publication: "*arXiv preprint arXiv:2609.06181*"
publication_short: "*arXiv*"
abstract: "Efficiently aggregating and orchestrating computing power across heterogeneous clusters for HPC workflows faces four practical challenges: preserving workflow context across independently administered clusters, moving large datasets between sites, reasoning about site-specific environments and scheduler policies, and exploiting live queue and resource states for efficient task scheduling. To this end, we design Diamond Agent, an agentic system that enables intelligent execution of HPC workflows across heterogeneous clusters with typed skills as the interface. Diamond Agent provides an agent-facing workspace and skills that unify cross-site resource discovery, resource specification, data movement, task execution, and result retrieval. A centralized Diamond Agent instance can operate multiple supercomputers without being deployed separately on each login node. Diamond Agent translates high-level agent actions into valid site-specific executions, moves data through Globus Transfer, and uses live system capability and queue information to select feasible placements. Its event-driven continuation mechanism decouples agent actions from long-running batch jobs: persistent services monitor remote execution and resume the agent only when a result or decision-relevant event is available. We experiment with 27 hours of telemetry and 19 matched multi-site submission rounds comprising 83 jobs across four production supercomputers. Compared with a fixed-site baseline, Diamond Agent reduces the median additional completion time relative to the fastest observed placement from 42 seconds to 4 seconds, a 10.5x reduction."
draft: false
featured: false
tags:
  - LLM Agents
  - HPC Workflows
  - Scheduling
categories:
  - High Performance Computing
url_pdf: https://arxiv.org/pdf/2609.06181
links:
  - name: arXiv
    url: https://arxiv.org/abs/2609.06181
date: 2026-09-05T00:00:00Z
---
