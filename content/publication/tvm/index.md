---
title: "[VLDB 2024] TVM: A Tile-based Video Management Framework"
draft: false
date: 2023-11-17
description: "This study introduces a novel tile-based video management framework, called TVM, which leverages the semantic information embedded in videos. By constructing a tile-based semantic index for newly ingested videos, TVM effectively reduces the size of decoded and processed video data."
rating: "CCF-A"
author: "1st auth."
period: "M."
link: "https://scholar.google.com/citations?view_op=view_citation&hl=zh-CN&user=ZkcJasgAAAAJ&citation_for_view=ZkcJasgAAAAJ:9yKSN-GCB0IC"
pdf: "https://www.vldb.org/pvldb/vol17/p671-zhang.pdf"
tags:
  - Publications
---

![poster.jpg](https://s2.loli.net/2024/06/21/PxwDtAeoZIgN7lu.jpg)

*Abstract: With the exponential growth of video data, there is a pressing need for efficient video analysis technology. Modern query frameworks aim to accelerate queries by reducing the frequency of calls to ex- pensive deep neural networks, which often overlook the overhead associated with video decoding and retrieval. Furthermore, video storage frameworks optimize video retrieval through video parti- tion or caching, often relying on prior information about the query workload. To further accelerate queries, this study introduces a novel tile-based video management framework, called TVM, which leverages the semantic information embedded in videos, without being dependent on specific query workloads. By constructing a tile-based semantic index for newly ingested videos, TVM effec- tively reduces the size of decoded and processed video data. To achieve this, TVM introduces an optimal index construction algo- rithm that utilizes cost function and pseudo-labels. Additionally, the framework proposes a query-driven tile parallel decoding algo- rithm and decoding cache algorithms, which further expedite the retrieval of video frames. Experimental results demonstrate that TVM can significantly enhance the throughput of various query tasks, achieving a notable speedup of more than 5.6$\times$.*