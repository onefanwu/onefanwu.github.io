---
layout: archive
title: "Projects"
permalink: /projects/
author_profile: true
---
{% include base_path %}

<div class="project-grid">

  <article class="project-card">
    <div class="project-card__header">
      <h3 class="project-card__title"><a href="https://onefanwu.github.io/projects/serverless-agent/">Serverless Multi-Agent System</a></h3>
      <span class="project-card__date">July 2026 - Present</span>
    </div>
    <p class="project-card__abstract">Autonomous AI agent platforms such as OpenClaw are increasingly deployed to serve long-running, interactive workloads that span multiple tool calls, model invocations, and external API interactions. However, existing deployments typically run agents on statically provisioned containers or fixed-size instances, leading to chronic resource inefficiency: agents sit idle between turns, blocking scarce GPU and memory when not actively reasoning, yet cannot acquire additional capacity on the spot when a complex multi-step task demands sudden bursts of compute. This project proposes a serverless, cloud-native system architecture that allows autonomous agents such as OpenClaw to elastically acquire and release resources at fine granularity while preserving interactive serving semantics. The system decouples agent identity and conversation state from the underlying execution runtime, enabling suspend/resume of containers without losing context or incurring cold-start penalties. A second focus is intelligent context sharing across agents, exposing a shared context layer through which cooperating agents securely exchange intermediate reasoning artifacts and memory snapshots, avoiding recomputation and redundant API spending.</p>
  </article>

  <article class="project-card">
    <div class="project-card__header">
      <h3 class="project-card__title"><a href="https://onefanwu.github.io/projects/agent-economy-and-data-market/">Agent Economy and Data Markets</a></h3>
      <span class="project-card__date">Mar 2026 - Present</span>
    </div>
    <p class="project-card__abstract">Autonomous agents increasingly rely on external data to complete downstream tasks such as model training and decision support. However, existing data discovery systems remain largely retrieval-oriented: they surface candidate datasets from heterogeneous sources, but provide limited support for estimating taskspecific utility, selecting cost-effective datasets under budget constraints, or incorporating trustworthy feedback from prior usage. This project presents Guixu, a valuation-driven data discovery system for autonomous agents. Guixu employs a three-phase valuation pipeline with proxy-label propagation and multi-round knapsack optimization for task-aware data valuation. Guixu integrates agentic payment protocol to enable budget-constrained data procurement workflows. Guixu leverages on-chain data market and attestation signals for verifiable data discovery.</p>
  </article>

  <article class="project-card">
    <div class="project-card__header">
      <h3 class="project-card__title"><a href="https://onefanwu.github.io/projects/serverless-data-warehouse/">Serverless Data Warehouse</a></h3>
      <span class="project-card__date">Dec 2024 - May 2026</span>
    </div>
    <p class="project-card__abstract">Memory overload is a common form of resource exhaustion in cloud data warehouses. When database queries fail due to memory overload, it not only wastes critical resources such as CPU time but also disrupts the execution of core business processes. This project proposes SafeLoad, the first query admission control framework specifically designed to identify memory-overloading (MO) queries, alongside SafeBench, an open-source, industrial-scale benchmark with 150 million real queries. SafeLoad achieves state-of-the-art prediction performance, improving precision by up to 66% over the best baseline and reducing wasted CPU time by up to 8.09x.</p>
  </article>

  <article class="project-card">
    <div class="project-card__header">
      <h3 class="project-card__title"><a href="https://onefanwu.github.io/projects/db4ai/">In-Database AI Inference</a></h3>
      <span class="project-card__date">Dec 2023 - July 2025</span>
    </div>
    <p class="project-card__abstract">To enable OLAP database systems to efficiently support emerging analytical workloads that incorporate AI inference, this project proposes AiQ, a novel in-database AI query acceleration framework. AiQ is integrated with Spark SQL and supports Spark RAPIDS, enabling efficient execution of real-world AI-enhanced database workloads. The core idea is to improve query performance by optimizing the execution of User-Defined Inference Functions (UDIFs) through dynamic processing granularity adjustment during Adaptive Query Execution, and an inference-aware operator offloading mechanism that leverages GPU residency of AI inference results.</p>
  </article>

  <article class="project-card">
    <div class="project-card__header">
      <h3 class="project-card__title"><a href="https://onefanwu.github.io/projects/cimdb/">Data Management on CIM Architecture</a></h3>
      <span class="project-card__date">Sep 2021 - Jul 2024</span>
    </div>
    <p class="project-card__abstract">This project aims to design an efficient storage method for emerging Compute-In-Memory (CIM) architectures to support diverse data structures and access patterns, thereby effectively accelerating multi-MVM queries.</p>
  </article>

  <article class="project-card">
    <div class="project-card__header">
      <h3 class="project-card__title"><a href="https://onefanwu.github.io/projects/acc/">Aerobic Capacity Clustering</a></h3>
      <span class="project-card__date">Nov 2019 - Jun 2021</span>
    </div>
    <p class="project-card__abstract">This project aims to learn the human's aerobic capacity from the exercise data (e.g., heart rate and speed) of undergraduate students, and thus a customized exercise program can be provided for each student. This project is co-funded by the National Student Innovation Training Program and Zhejiang Province New Talent Program. Please see <a href="https://patents.google.com/patent/CN112836105A/en">our patents</a> for more details.</p>
  </article>

  <article class="project-card">
    <div class="project-card__header">
      <h3 class="project-card__title"><a href="https://onefanwu.github.io/projects/rfc/">Rolled Fingerprint Construction</a></h3>
      <span class="project-card__date">Jan 2019 - Oct 2020</span>
    </div>
    <p class="project-card__abstract">Compared with a flat fingerprint, the rolled fingerprint has a larger fingerprint area and can be extracted more minutiae. We propose a novel rolled fingerprint construction algorithm called BlockRFC (Block-based Rolled Fingerprint Construction) to address distortion and mosaicking gap challenges. Please see <a href="https://ieeexplore.ieee.org/abstract/document/9274479">our papers</a> for more details.</p>
  </article>

</div>

<script>
(function() {
  var abstracts = document.querySelectorAll('.project-card__abstract');
  abstracts.forEach(function(p) {
    if (p.scrollHeight > 120) {
      p.classList.add('project-card__abstract--clamped');
      var btn = document.createElement('button');
      btn.className = 'project-card__toggle';
      btn.textContent = 'Read more';
      btn.addEventListener('click', function() {
        if (p.classList.contains('project-card__abstract--expanded')) {
          p.classList.remove('project-card__abstract--expanded');
          btn.textContent = 'Read more';
        } else {
          p.classList.add('project-card__abstract--expanded');
          btn.textContent = 'Show less';
        }
      });
      p.parentNode.insertBefore(btn, p.nextSibling);
    }
  });
})();
</script>
