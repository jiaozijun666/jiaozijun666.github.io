---
layout: page
title: Backend and tool-agent orchestration for an air-gapped railway intelligence system
description: Tool-agent integration, an automated meeting-documentation workflow, and the permission model that makes on-premise deployment defensible.
img: assets/img/railway_llm.png
importance: 1
category: research experience
---

**Research Assistant, The Future Laboratory, Tsinghua University · advised by [Prof. Haipeng Mi](https://thfl.tsinghua.edu.cn/yjdw/jzg/zxjg/qt/yjy/mhp.htm) · June 2025 – present**

{% include figure.liquid loading="eager" path="assets/img/railway_llm.png" class="img-fluid rounded z-depth-1" alt="System diagram: multi-source enterprise data feeding a domain-adapted language model with retrieval and a knowledge graph, serving office-automation and maintenance applications on on-premise infrastructure." %}
<div class="caption">System overview, from enterprise data sources to the office and maintenance applications built on top.</div>

A network-isolated, on-premise language-model system supporting office and maintenance workflows at a heavy-haul railway operator. Nothing leaves the operator's own infrastructure, which is the constraint that shapes every design decision below.

**Backend and integration.** I am responsible for the backend: data processing, and the integration of the external tool agents the system calls out to.

**Meeting-documentation workflow.** I designed and built the automated meeting-minutes workflow as a two-tier agent. A controller selects among registered retrieval, transcription and reasoning tools; a sub-agent converts noisy transcripts into structured minutes through noise reduction, semantic reconstruction and topic structuring.

**Reliability and data governance.** I introduced a permissioned four-zone workspace — a read-only knowledge base, write-isolated user input, scratch space, and a results directory — together with an explicit delegation contract between the two tiers, so that agent actions cannot modify authoritative enterprise records. That guarantee is the governance requirement motivating on-premise deployment in the first place.

**Methods:** agent and tool orchestration · retrieval-augmented generation · ASR post-processing · permission modelling
