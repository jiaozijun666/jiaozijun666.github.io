---
layout: page
title: Multi-agent equity analysis with large language models
description: Four analyst agents exchanging information only through a typed shared state, with an adversarial stage built to disagree with them.
img: assets/img/stockagent.png
importance: 1
category: coursework projects
---

**National University of Singapore · 2025** · [Code](https://github.com/nusduck/QF5214_2025_G7_StockAgent)

{% include figure.liquid loading="eager" path="assets/img/stockagent.png" class="img-fluid rounded z-depth-1" alt="Architecture diagram: market, fundamental, news and technical data feeding four coordinating analyst agents that output reports, ratings and risk assessments." %}
<div class="caption">Four analyst agents over a shared state, with data sources on the left and outputs on the right.</div>

**Shared-state coordination.** I co-designed the shared state object through which four analyst agents — fundamentals, technical, sentiment and adversarial — exchange information. The agents never call one another. Data-collection tools write into six typed domains covering identifiers, market data, financial statements, external research, generated reports and workflow control, and downstream agents read only the fields they need, which is what keeps each agent independently testable and replaceable.

**Two-tier prompt architecture.** A system-level prompt fixes output format, tool-use protocol and fallback behaviour; role-specific prompts constrain each analyst's methodology and risk boundaries. Separating the two is what keeps four differently-specialised outputs machine-parsable and mergeable.

**Adversarial review stage.** A five-part challenge applied to the three analyst reports, testing for over-optimistic assumptions, under-weighted macro and governance risk, cross-report contradictions, assumption fragility, and horizon-separated forecasts — a deliberate hedge against convergent reasoning among agents that share their data sources.

**Methods:** LangChain · multi-agent orchestration · structured prompting · MySQL · AkShare · Next.js · Streamlit

*Scope: the project delivered a working system; no backtesting or forecast-validity evaluation was carried out.*
