---
title: "[CVPR 2022] Learning Based Multi-Modality Image and Video Compression"
draft: false
date: 2022-03-20
description: "Multi-modality (i.e., multi-sensor) data is widely used in various vision tasks for more accurate or robust perception. This work proposes a multi-modality compression framework for infrared and visible image pairs by exploiting the cross-modality redundancy."
rating: "CCF-A"
author: "Co-1st auth."
period: "B.S."
link: "https://scholar.google.com/citations?view_op=view_citation&hl=zh-CN&user=ZkcJasgAAAAJ&citation_for_view=ZkcJasgAAAAJ:u5HHmVD_uO8C"
pdf: "http://openaccess.thecvf.com/content/CVPR2022/papers/Lu_Learning_Based_Multi-Modality_Image_and_Video_Compression_CVPR_2022_paper.pdf"
tags:
  - Publications
---

![poster](https://s2.loli.net/2023/11/29/ItiU7pEz9OZbBeR.jpg)

*Abstract: Multi-modality (i.e., multi-sensor) data is widely used in various vision tasks for more accurate or robust perception. However, the increased data modalities bring new challenges for data storage and transmission. The existing data compression approaches usually adopt individual codecs for each modality without considering the correlation between different modalities. This work proposes a multi-modality compression framework for infrared and visible image pairs by exploiting the cross-modality redundancy. Specifically, given the image in the reference modality (e.g., the infrared image), we use the channel-wise alignment module to produce the aligned features based on the affine transform. Then the aligned feature is used as the context information for compressing the image in the current modality (e.g., the visible image), and the corresponding affine coefficients are losslessly compressed at negligible cost. Furthermore, we introduce the Transformer-based spatial alignment module to exploit the correlation between the intermediate features in the decoding procedures for different modalities. Our framework is very flexible and easily extended for multi-modality video compression. Experimental results show our proposed framework outperforms the traditional and learning-based single modality compression methods on the FLIR and KAIST datasets.*

### Brief Introduction
The following 5-minute video is a brief introduction required for the CVPR 2022 online conference.

{{< rawhtml >}}
<video controls width="100%">
  <source src="http://storage.live.com/items/DC7EE90AFDCC4B11!330431:/introduction_720p_x264.mp4" type="video/mp4">
</video>
{{< /rawhtml >}}