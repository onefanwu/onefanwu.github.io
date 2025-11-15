---
layout: archive
title: "Projects"
permalink: /projects/
author_profile: true
---
{% include base_path %}

## PhD period (Sep 2021 - Present)

### [Serverless Data Warehouse [Aug 2024 - Present]](https://onefanwu.github.io/projects/serverless/)

**Abstract**: Memory overload is a common form of resource exhaustion in  cloud data warehouses. When database queries fail due to memory overload, it not only wastes critical resources such as CPU  time but also disrupts the execution of core business processes, as  memory-overloading (MO) queries are typically part of complex  workflows. If such queries are identified in advance and scheduled  to memory-rich serverless clusters, it can prevent resource wastage  and query execution failure. Therefore, cloud data warehouses desire an admission control framework with high prediction precision,  interpretability, efficiency, and adaptability to effectively identify  memory-overloading queries. However, existing admission control  frameworks primarily focus on scenarios like SLA satisfaction and  resource isolation, with limited precision in identifying MO queries.  Moreover, there is a lack of publicly available MO-labeled datasets  with workloads for training and benchmarking. To tackle these challenges, we propose SafeLoad, the first query admission control  framework specifically designed to identify MO queries. Alongside,  we release SafeBench, an open-source, industrial-scale benchmark  for this task, which includes 150 million real queries. SafeLoad first  filters out memory-safe queries using the interpretable discriminative rule. It then applies a hybrid architecture that integrates both  a global model and cluster-level models, supplemented by a misprediction correction module to identify MO queries. Additionally,  a self-tuning quota management mechanism dynamically adjusts  prediction quotas per cluster to improve precision. Experimental  results show that SafeLoad achieves state-of-the-art prediction  performance with low online and offline time overhead. Specifically,  SafeLoad improves precision by up to 66% over the best baseline  and reduces wasted CPU time by up to 8.09× compared to scenarios  without SafeLoad.

### [In-Database AI Inference [Dec 2023 - Present]](https://onefanwu.github.io/projects/db4ai/)

**Abstract**: TBD


### [Data Management on CIM Architecture [Sep 2021 - Jul 2024]](https://onefanwu.github.io/projects/cimdb/)

**Abstract**: This project aims to design an efficient storage method for emerging Compute-In-Memory (CIM) architectures to support diverse data structures and access patterns, thereby effectively accelerating multi-MVM queries.


## Undergraduate period (Sep 2017 - Jun 2021)

### [Aerobic Capacity Clustering [Nov 2019 - Jun 2021]](https://onefanwu.github.io/projects/acc/)

**Abstract**: This project is the subject of my internship as a machine learning engineer at the Southeast Digital Economic Development Institute (Quzhou). It aims to learn the human's aerobic capacity from the exercise data (e.g., heart rate and speed) of undergraduate students, and thus a customized exercise program can be provided for each student. This project is co-funded by the National Student Innovation Training Program and Zhejiang Province New Talent Program. Please see [our patents](https://patents.google.com/patent/CN112836105A/en) for more details.

### [Rolled Fingerprint Construction [Jan 2019 - Oct 2020]](https://onefanwu.github.io/projects/rfc/)

**Abstract**: Compared with a flat fingerprint, the rolled fingerprint has a larger fingerprint area and can be extracted more minutiae. It has high requirements in many fields, not only in the military environment or the police field but also in many civil application fields. The challenge that has been troubled for a long time is that contact-based rolled fingerprint registration is easy to cause obvious distortion without human experts’ supervision, which has a negative impact on fingerprint recognition performance. Due to the elastic deformation of fingertips, the mosaicking gaps in the rolled fingerprint are usually visible but challenging to locate. To address these problems, we propose a novel rolled fingerprint construction algorithm called BlockRFC (Block-based Rolled Fingerprint Construction). Please see [our papers](https://ieeexplore.ieee.org/abstract/document/9274479) for more details.
