---
layout: page
title: LLM-assisted ESG metric extraction and standardisation for healthcare reporting
description: A language-model extractor and a BERT matcher joined by typed data contracts, feeding an 18-topic scoring rubric.
img: assets/img/esg.png
importance: 3
category: research experience
---

**National University of Singapore · 2025** · [Code](https://github.com/ariahuang314/groupproject)

{% include figure.liquid loading="eager" path="assets/img/esg.png" class="img-fluid rounded z-depth-1" alt="Pipeline diagram: sustainability report PDFs parsed into text, quantitative and qualitative metrics extracted, matched by BERT, scored, and shown in a dashboard." %}
<div class="caption">From report PDF to extraction, standardisation, scoring and dashboard.</div>

Sustainability reports describe the same underlying quantity in different words, different units and different places in the document, which is much of why published ESG ratings are hard to reproduce. The problem is split here between two model families according to what each is good at.

**Extraction and standardisation architecture:** A language-model extractor parses heterogeneous report prose into tuples of metric, value, unit and confidence — that stage absorbs the linguistic variation. A BERT semantic matcher then maps free-form metric names onto a canonical taxonomy, which makes the output deterministic and joinable. The two are connected by typed data contracts, so extraction, matching and scoring stay independently replaceable.

**Scoring framework and validation plan:** An 18-topic, 39-indicator rubric aligned to SGX reporting guidance, with topic weights derived from mention frequencies across 83 Singapore-listed healthcare sustainability reports. An evaluation protocol for human annotation and comparison against external ratings is designed but belongs to a subsequent validation phase; the scores as they stand have not been checked against either.

**Individual contribution:** Developed the backend data-processing pipeline, including PDF parsing, text cleaning and segmentation, ESG indicator extraction, integration of NLP / LLM
components, and generation of structured outputs for downstream ESG scoring and frontend visualization.

**Methods:** LLM information extraction · BERT semantic matching · pdfplumber · MySQL · Flask · Dash
