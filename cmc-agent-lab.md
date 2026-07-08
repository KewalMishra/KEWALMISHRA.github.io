---
layout: page
title: CMC Agent Lab
permalink: /cmc-agent-lab/
---

## CMC Agent Lab

**Agentic AI for late-stage pharmaceutical process development**

CMC Agent Lab is an auditable AI workbench for CMC and pharmaceutical technology development.
It is designed around a practical development question: how can a scientist move from a
molecule, product target, sparse historical experiments, and process constraints to a smaller,
better set of experiments?

<div class="pill-row">
	<span>LangGraph</span>
	<span>Mechanistic simulation</span>
	<span>Reinforcement learning</span>
	<span>QbD risk controls</span>
	<span>Auditability</span>
</div>

<p><a class="btn" href="https://github.com/kewalmishra/cmc-agent-lab">GitHub</a> <a class="btn btn--quiet" href="https://github.com/kewalmishra/cmc-agent-lab/blob/main/demo/rl-policy-memo.md">RL memo</a></p>

### Product Thesis

Generic RAG is not the hard problem in late-stage pharma development. The harder problem is
coordinating scientific models, sparse data, experiment budgets, regulatory expectations, and
human review in one decision-support workflow.

CMC Agent Lab shows that product direction:

- first-principles-inspired models for stability, reaction conversion, crystallization, and dissolution
- active-learning experiment recommendation over sparse historical data
- reinforcement-learning policy training against a simulator-backed digital twin
- QbD/FMEA-style risk register linking CPPs to CQAs
- typed state, audit events, tool provenance, and human-review boundaries

### Why It Matters

The system is built for the part of AI product work that is easy to underestimate: translating a
scientific workflow into software that can be inspected, evaluated, and trusted. It is not just a
model call. It is a product architecture for choosing what to run, when to stop, what to ask a
scientist to review, and how to leave an audit trail.

### Representative Workflow

1. Parse a process-development question into QTPP, CQAs, CPPs, constraints, and workflow mode.
2. Select the appropriate tools for the scientist's goal.
3. Run mechanistic simulators or a simulator-backed RL policy.
4. Recommend a constrained experiment batch.
5. Generate risk controls and an auditable technical memo.

### Open-Source Simulator Roadmap

The local implementation runs anywhere through built-in transparent simulators. The adapter
roadmap targets PharmaPy, IDAES/Pyomo, Cantera, DWSIM, and Thermo/Chemicals for higher-fidelity
process simulation.
