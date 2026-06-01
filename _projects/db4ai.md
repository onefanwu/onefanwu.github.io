---
title: "In-Database AI Inference"
excerpt: "TBD"
collection: projects
---

To enable OLAP database systems to efficiently support emerging analytical workloads that incorporate AI inference, this project focuses on optimizing query vectorization and GPU co-processing for accelerating In-Database AI Inference Queries (In-DB AI Inference Queries). The work aims to improve the execution efficiency of OLAP queries containing AI inference operators and proposes AiQ, a novel in-database AI query acceleration framework. AiQ is integrated with Spark SQL and supports Spark RAPIDS, enabling efficient execution of real-world AI-enhanced database workloads, including semantic search, sentiment analysis, and time-series analytics.

The core idea of AiQ is to improve query performance by optimizing the execution of User-Defined Inference Functions (UDIFs). Specifically, AiQ models the throughput of a UDIF using a Rows-Per-Second (RPS) function and dynamically adjusts the processing granularity of UDIFs during Adaptive Query Execution (AQE) to maximize GPU utilization and minimize query latency. This optimization problem is formulated as a multi-objective optimization task and is solved using a gradient-ascent-based strategy to identify the optimal inference batch granularity. In addition, AiQ introduces an inference-aware operator offloading mechanism, which leverages the residency of AI inference results on GPUs to offload portions of the query pipeline, thereby reducing data movement and I/O overhead while exploiting GPU acceleration for relational operators. Experimental evaluations demonstrate that AiQ effectively accelerates AI-enabled analytical queries and significantly improves the efficiency of in-database AI inference workloads.



### Patents
[Method, Device, and Storage Medium for In-Database AI Inference Based on Selective Awareness]()  
Lidan Shou, **Yifan Wu**, Huan Li, Ke Chen, Xinyuan Luo, Gang Chen  
2026


### Team
- [Lidan Shou](https://scholar.google.com/citations?user=0OlITuIAAAAJ) (Project Leader & Advisor)
- [Yifan Wu](https://scholar.google.com/citations?user=l2GmQnQAAAAJ)
- [Ke Chen](https://scholar.google.com/citations?user=cqfBLecAAAAJ)
- [Huan Li](https://longaspire.github.io/)