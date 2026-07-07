---
layout: page
title: BioGraph Agent
permalink: /biograph-agent/
---

## BioGraph Agent

**A decision-grade target diligence workbench for translational AI.**

The point of this project is simple: AI is already good at generating code and fluent summaries. What stands out now is the ability to design the right product surface for a high-stakes scientific workflow.

BioGraph Agent asks a more useful question:

> For this EHR + omics cohort, which molecular target should we prioritize, what evidence supports it, what does sequence-level modeling add, and what experiment should we run next?

<p><a class="btn" href="https://github.com/KewalMishra/bionemo-langgraph-agent-framework">Open GitHub repo</a></p>

### What It Does

- Translates cohort criteria into normalized FHIR/OMOP-like concepts with lineage.
- Scores targets across clinical fit, variant evidence, pathway biology, tractability, and BioNeMo-style sequence evidence.
- Ranks molecular targets and explains the evidence balance, rationale, and risks.
- Proposes next-best experiments for computational biology, clinical data science, wet lab, and product teams.
- Emits audit controls for intended use, model provenance, cohort lineage, human review, and clinical decision-support risk.
- Runs benchmark scenarios with expected top-target rankings.
- Generates Markdown dossiers and static HTML dashboards.

### Why It Is More Than A Demo

Most agent projects stop at planner, tool call, and summary. This one is organized around the pieces that matter in healthcare and life sciences adoption:

- **Decision artifact:** the output is a target diligence dossier, not a chatbot answer.
- **Governance:** intended use, human review, and model provenance are first-class state.
- **Evaluation:** benchmark scenarios assert expected rankings and audit behavior.
- **Integration boundary:** BioNeMo is isolated behind an adapter so local demos and GPU-backed runs use the same graph contract.
- **Product thinking:** the project includes success metrics, roadmap, and adoption risks.

### Stack

<div class="pill-row">
	<span>LangGraph</span>
	<span>NVIDIA BioNeMo / Evo2 adapter</span>
	<span>Pydantic</span>
	<span>FHIR/OMOP-style cohort semantics</span>
	<span>Pytest + CI</span>
	<span>Static HTML dossier</span>
</div>

### Evidence Of Substance

The repository includes two repeatable scenarios:

- **IBD target validation:** ranks NOD2, IL23R, and ATG16L1 for a Crohn's disease EHR + omics cohort.
- **Precision oncology BRCA review:** ranks BRCA1 and TP53 for hereditary breast and ovarian cancer variant triage, including a clinical decision-support warning.

The benchmark runner currently passes both expected-ranking scenarios and the GitHub Actions workflow runs lint and tests on every push.

### Why I Built It This Way

HCLS AI products need to connect multiple worlds at once: biological evidence, clinical workflow, model inference, regulatory posture, and product adoption. BioGraph Agent is a small but concrete way to show that I can design across those boundaries.
