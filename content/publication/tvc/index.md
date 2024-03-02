---
title: "[JBUAA] A Transformer based deep conditional video compression"
draft: false
date: 2022-05-05
description: "It is difficult to attain the best compression performance given that typical CNN can only use local correlations and the sparsity of prediction residual. This paper proposed a Transformer-based deep conditional video compression algorithm, which can achieve better compression performance."
rating: "EI"
author: "Co-1st auth."
period: "B.S."
link: "https://kns.cnki.net/kcms2/article/abstract?v=Eo9-C_M6tLmXWOkD-sNcF8BKn9DBMuppP-IKA9SkB45YcOxBBYdKwTcuyw9t_Fo7eyrLdW8v31uQkBG7qU0ImBNH6o8WxShIOghQJjQX0XvCD3GULkF-bKaKXF32KVQSmAik21sDccE=&uniplatform=NZKPT&language=CHS"
tags:
  - Publications
---

![poster](https://s2.loli.net/2023/11/29/5TesQ8yoGHCu9m3.jpg)

*Abstract: Convolutional neural networks (CNN) are the foundation of most recent learning-based video compression algorithms, which also use residual coding and motion compensation architectures. It is difficult to attain the best compression performance given that typical CNN can only use local correlations and the sparsity of prediction residual. To solve the problems above, this paper proposed a Transformer-based deep conditional video compression algorithm, which can achieve better compression performance. Specifically, our algorithm first uses deformable convolution to obtain the predicted frame feature based on the motion information between the front and rear frames. Then, the predicted frame feature is used as conditional information to conditionally encode the original input frame feature which avoids the direct encoding of sparse residual signals. More importantly, our algorithm further utilizes the non-local correlation between the features and proposes a transformer-based autoencoder architecture to implement motion coding and conditional coding, which further improves the performance of compression. Experiments show that our Transformer based deep conditional video compression algorithm surpasses the current mainstream learning-based video compression algorithms in both HEVC and UVG datasets.*