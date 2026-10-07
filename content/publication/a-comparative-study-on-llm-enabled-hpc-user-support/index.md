---
title: "A Comparative Study on LLM-enabled HPC User Support"
publication_types:
  - "1"
authors:
  - admin
  - Fangru Linghu
  - Sikan Li
  - Marty Charles Kandes
  - Niall Gaffney
  - Ian Foster
  - Zhao Zhang
doi: 10.1145/3785462.3815796
publication: "in *Proceedings of the Practice and Experience in Advanced Research Computing 2026 (PEARC '26)*"
publication_short: "in *PEARC 2026*"
abstract: "Providing accurate and efficient user support with the emerging large language model (LLM) techniques for high-performance computing (HPC) centers is extremely challenging. The major obstacle lies in the integration of specialized knowledge that is not available in the base LLMs. Supervised Fine-tuning (SFT), Retrieval Augmented Generation (RAG), and In-Context Learning (ICL), are the common techniques to empower LLMs with domain knowledge. However, there is a lack of comprehensive understanding of their question-answering capabilities in the HPC domain. In this work, we present a comparative study of eight candidate methods by combining the base model (Llama-3.1-8B-Instruct), SFT, RAG, and ICL using a ticket database of 60,000 question-answer pairs from Texas Advanced Computing Center (TACC). We evaluate these methods with five metrics: correctness, coherence, relevance, fluency, and cosine similarity, using both human and LLMs as judges. Our results show that ICL+RAG with the base model achieves the highest correctness in general, and ICL with the base model outperforms others for debugging and testing questions. The results suggest that combining ICL, RAG, and a powerful base model is a promising solution for LLM-enabled user support in computing centers."
draft: false
featured: false
tags:
  - LLM
  - HPC User Support
  - RAG
categories:
  - High Performance Computing
date: 2026-07-26T00:00:00Z
---
