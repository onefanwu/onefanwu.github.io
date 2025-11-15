---
title: "Serverless Data Warehouse"
excerpt: "TBD"
collection: projects
---
Memory overload is a common form of resource exhaustion in  cloud data warehouses. When database queries fail due to memory overload, it not only wastes critical resources such as CPU  time but also disrupts the execution of core business processes, as  memory-overloading (MO) queries are typically part of complex  workflows. If such queries are identified in advance and scheduled  to memory-rich serverless clusters, it can prevent resource wastage  and query execution failure. Therefore, cloud data warehouses desire an admission control framework with high prediction precision,  interpretability, efficiency, and adaptability to effectively identify  memory-overloading queries. However, existing admission control  frameworks primarily focus on scenarios like SLA satisfaction and  resource isolation, with limited precision in identifying MO queries.  Moreover, there is a lack of publicly available MO-labeled datasets  with workloads for training and benchmarking. To tackle these challenges, we propose SafeLoad, the first query admission control  framework specifically designed to identify MO queries. Alongside,  we release SafeBench, an open-source, industrial-scale benchmark  for this task, which includes 150 million real queries. SafeLoad first  filters out memory-safe queries using the interpretable discriminative rule. It then applies a hybrid architecture that integrates both  a global model and cluster-level models, supplemented by a misprediction correction module to identify MO queries. Additionally,  a self-tuning quota management mechanism dynamically adjusts  prediction quotas per cluster to improve precision. Experimental  results show that SafeLoad achieves state-of-the-art prediction  performance with low online and offline time overhead. Specifically,  SafeLoad improves precision by up to 66% over the best baseline  and reduces wasted CPU time by up to 8.09× compared to scenarios  without SafeLoad.

### Team
- [Huan Li](https://longaspire.github.io/) (Project Leader)
- [Zhenhua Wang](https://www.linkedin.com/in/zhenhua-wang/) (Project Leader)
- [Yifan Wu](https://scholar.google.com/citations?user=l2GmQnQAAAAJ)
- Yuhan Li (Mentor)
- [Lidan Shou](https://scholar.google.com/citations?user=0OlITuIAAAAJ) (Advisor)
- [Ke Chen](https://scholar.google.com/citations?user=cqfBLecAAAAJ)

### Publications
**\* denotes the tagged author is my advisor**

[SafeLoad: Efficient Admission Control Framework for Identifying Memory-Overloading Queries in Cloud Data Warehouses]()
**Yifan Wu**, Yuhan Li, Zhenhua Wang, Zhongle Xie, Dingyu Yang, Ke Chen, Lidan Shou*, Bo  Tang, Liang Lin, Huan Li, Gang Chen
VLDB 2026, 52nd International Conference on Very Large Data Bases
[Homepage](https://safeload-project.github.io/Homepage) / [Benchmark](https://github.com/SafeLoad-project/SafeBench) / Slide / Video

### Patents