---
title: "[ICDE 2025] QaVA: Query-aware Video Analysis Framework Based on Data Access Pattern"
draft: false
date: 2024-11-10
description: "This study proposes QaVA, a query-aware video analysis framework, focusing on query preference data to accelerate the query processing. It introduce a technique to extract query data preferences from the data access pattern of historical queries and a tunable lightweight proxy score generator to accurately and quickly fit the interested data."
author: "1st. auth."
period: "M."
tags:
  - Publications
---

*Abstract: With the explosive growth of video data, efficient video analysis technology has garnered widespread attention. Existing online methods train proxy neural networks upon query arrival and use these networks to scan the entire dataset, guiding the invocation of the expensive deep neural network. While index-based methods advance this process to the index-building stage, significantly reducing the time overhead of video queries. However, the data to query often presents a long-tail distribution, and different types of queries are sensitive to different parts of the distribution. Since the index-based methods cannot predict the queries, they can only provide ad-hoc proxy score generating strategies. This paper proposes a query-aware video analysis framework, QaVA, to improve query performance further. QaVA retains the time-consuming, query-independent semantic extraction process during the index-building stage and employs a tunable lightweight adapter network to accurately and quickly focus on the data parts most relevant to the query after it arrives. Meanwhile, QaVA can automatically tune the training strategy of the adapter network by analyzing the data access pattern of historical queries, thus meeting the needs of general users. Experimental results demonstrate that QaVA can significantly reduce the cost of various queries across multiple datasets, and can speed up query processing by up to 9.2$\times$ compared to the most advanced index-based method. Our code is available: https://github.com/InkosiZhong/QaVA.*