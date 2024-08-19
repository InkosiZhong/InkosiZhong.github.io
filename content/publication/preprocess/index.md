---
title: "[TCSVT] Preprocessing Enhanced Image Compression for Machine Vision"
draft: false
date: 2022-07-10
description: "In this work, we propose a preprocessing enhanced image compression method for machine vision tasks to address this challenge. Instead of relying on the learned image codecs for end-to-end optimization, our framework is built upon the traditional non-differential codecs."
period: "B.S."
link: "https://scholar.google.com/citations?view_op=view_citation&hl=zh-CN&user=ZkcJasgAAAAJ&citation_for_view=ZkcJasgAAAAJ:u-x6o8ySG0sC"
pdf: "https://arxiv.org/pdf/2206.05650"
tags:
  - Publications
---

*Abstract: Recently, more and more images are compressed and sent to the back-end devices for machine analysis tasks (e.g., object detection) instead of being purely watched by humans. However, most traditional or learned image codecs are de- signed to minimize the distortion of the human visual system without considering the increased demand from machine vision systems. In this work, we propose a preprocessing enhanced image compression method for machine vision tasks to address this challenge. Instead of relying on the learned image codecs for end-to-end optimization, our framework is built upon the traditional non-differential codecs, which means it is standard compatible and can be easily deployed in practical applications. Specifically, we propose a neural preprocessing module before the encoder to maintain the useful semantic information for the downstream tasks and suppress the irrelevant information for bitrate saving. Furthermore, our neural preprocessing module is quantization adaptive and can be used in different compression ratios. More importantly, to jointly optimize the preprocessing module with the downstream machine vision tasks, we introduce the proxy network for the traditional non-differential codecs in the back-propagation stage. We provide extensive experiments by evaluating our compression method for several representative downstream tasks with different backbone networks. Experimen- tal results show our method achieves a better trade-off between the coding bitrate and the performance of the downstream machine vision tasks by saving about 20% bitrate.*