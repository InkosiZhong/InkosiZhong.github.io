---
title: "[ECCV 2024] GTMS: A Gradient-driven Tree-guided Mask-free Referring Image Segmentation Method"
draft: false
date: 2023-11-17
description: "This study introduces a novel mask-free RIS method, called GTMS, which utilizes both structural and semantic information. It achieves SOTA performance compared with other mask-free RIS methods and even outperforms many fully-supervised RIS methods."
author: "2nd auth."
period: "M."
tags:
  - Publications
---
![poster](https://s2.loli.net/2024/09/11/L3DqlTA4iPJHMVE.jpg)

*Abstract: Referring image segmentation (RIS) aims to segment an object of interest by a given natural language expression. As fully-supervised methods require expensive pixel-wise labeling, mask-free solutions supervised by low-cost labels are largely desired. However, existing mask-free RIS methods suffer from complicated architectures or insufficient utilization of structural and semantic information resulting in unsatisfactory performance. In this paper, we propose a gradient-driven tree-guided mask-free RIS method, GTMS, which utilizes both structural and semantic information, while only using a bounding box as the supervised signal. Specifically, we first construct the structural information of the input image as a tree structure. Meanwhile, we utilize gradient information to explore semantically related regions from the text feature. Finally, the structural information and semantic information are used to refine the output of the segmentation model to generate pseudo labels, which in turn are used to optimize the model. To verify the effectiveness of our method, the experiments are conducted on three benchmarks, i.e., RefCOCO/+/g. RIS methods and even better than many fully supervised RIS methods. Our method achieves SOTA performance compared with other mask-free RIS methods and even outperforms many fully supervised RIS methods. Specifically, GTMS attains 66.54%, 69.98% and 63.41% IoU on RefCOCO Val-Test, TestA and TestB.*