---
title: "[VLDB 2024] TVM: A Tile-based Video Management Framework"
draft: false
date: 2023-11-17
description: "With the exponential growth of video data, there is a pressing need for efficient video analysis technology. This study introduces a novel tile-based video management framework, called TVM, which leverages the semantic information embedded in videos, without being dependent on specific query workloads. By constructing a tile-based semantic index for newly ingested videos, TVM effectively reduces the size of decoded and processed video data."
rating: "CCF-A"
author: "1st auth."
period: "M."
tags:
  - Publications
---

*Abstract: With the exponential growth of video data, there is a pressing need for efficient video analysis technology. Modern query frameworks aim to accelerate queries by reducing the frequency of calls to ex- pensive deep neural networks, which often overlook the overhead associated with video decoding and retrieval. Furthermore, video storage frameworks optimize video retrieval through video parti- tion or caching, often relying on prior information about the query workload. To further accelerate queries, this study introduces a novel tile-based video management framework, called TVM, which leverages the semantic information embedded in videos, without being dependent on specific query workloads. By constructing a tile-based semantic index for newly ingested videos, TVM effec- tively reduces the size of decoded and processed video data. To achieve this, TVM introduces an optimal index construction algo- rithm that utilizes cost function and pseudo-labels. Additionally, the framework proposes a query-driven tile parallel decoding algo- rithm and decoding cache algorithms, which further expedite the retrieval of video frames. Experimental results demonstrate that TVM can significantly enhance the throughput of various query tasks, achieving a notable speedup of more than 5.6$\times$.*