---
title: "[arXiv] VFRTok: Variable Frame Rates Video Tokenizer with Duration-Proportional Information Assumption"
draft: false
date: 2025-05-16
description: "This paper introduces VFRTok, a Transformer-based video tokenizer, that enables variable frame rate encoding and decoding. Furthermore, it proposes Partial Rotary Position Embeddings (RoPE) to improve content-awareness, which enhances the video generation capability."
author: "1st. auth."
period: "M."
link: "https://scholar.google.com/citations?view_op=view_citation&hl=zh-CN&user=ZkcJasgAAAAJ&citation_for_view=ZkcJasgAAAAJ:zYLM7Y9cAGgC"
pdf: "https://arxiv.org/pdf/2505.12053"
tags:
  - Publications
---

*Abstract: Modern video generation frameworks based on Latent Diffusion Models suffer from inefficiencies in tokenization due to the Frame-Proportional Information Assumption. Existing tokenizers provide fixed temporal compression rates, causing the computational cost of the diffusion model to scale linearly with the frame rate. The paper proposes the Duration-Proportional Information Assumption: the upper bound on the information capacity of a video is proportional to the duration rather than the number of frames. Based on this insight, the paper introduces VFRTok, a Transformer-based video tokenizer, that enables variable frame rate encoding and decoding through asymmetric frame rate training between the encoder and decoder. Furthermore, the paper proposes Partial Rotary Position Embeddings (RoPE) to decouple position and content modeling, which groups correlated patches into unified tokens. The Partial RoPE effectively improves content-awareness, enhancing the video generation capability. Benefiting from the compact and continuous spatio-temporal representation, VFRTok achieves competitive reconstruction quality and state-of-the-art generation fidelity while using only 1/8 tokens compared to existing tokenizers.*