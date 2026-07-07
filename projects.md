---
layout: page
title: Projects
permalink: /projects/
---

## BioGraph Agent

**LangGraph + NVIDIA BioNeMo for translational research workflows**

BioGraph Agent is a life sciences agent framework that shows how I think about AI products in regulated healthcare and life sciences environments. The project combines LangGraph orchestration, a BioNeMo Evo2 integration boundary, governance checks, evaluation rubrics, and product-facing documentation.

It is built around a cohort-to-target validation scenario: given an EHR/omics cohort, molecular targets, and reference/alternate sequences, the graph produces a research brief with evidence, BioNeMo-style signals, readiness scoring, and human-review guardrails.

<p><a class="btn" href="https://github.com/KewalMishra/bionemo-langgraph-agent-framework">Open GitHub repo</a></p>

### What It Shows

- Agent design with explicit state, tool boundaries, and review gates.
- BioNeMo integration as a portable adapter rather than a hard-coded demo dependency.
- HCLS product thinking: intended use, governance, evaluation, and adoption metrics.
- Documentation for architecture, product framing, governance, evaluation, and roadmap.

### Why It Matters

AI is already strong at producing code. The harder product problem is knowing what should be built, where it fits into scientific workflows, how it should be evaluated, and what trust boundaries must exist before users can adopt it. BioGraph Agent is a compact artifact for that point of view.

