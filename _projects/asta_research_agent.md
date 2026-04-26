---
layout: page
title: LLM RESEARCH AGENT (SPIN)
description: A verifiable literature retrieval system using Criteria-Driven RAG and Evidence-to-Generate (E2G) pipelines.
img: assets/img/asta_pipeline.jpg
importance: 3
category: work
github: https://github.com/Beichen-H/Research-Agent
---

This project was developed as a technical evaluation of **Asta**, an AI-driven literature search agent. I architected a Python prototype that shifts from traditional retrieve-and-rank methods to a **Criteria-Driven RAG pipeline**, ensuring every academic claim is grounded in verifiable evidence.

<div class="row justify-content-sm-center mt-4">
    <div class="col-sm-12 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/asta_pipeline.jpg" title="SOTA RAG Synthesis Pipeline" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    <b>System Architecture:</b> Implementing E2G (Evidence Extraction), TRACE (Reasoning Chains), and AGREE (Self-Verification) to eliminate hallucinations in academic literature retrieval.
</div>

## Technical Innovations

* **Intent Decomposition:** Translates natural language queries into 3 structured screening criteria and expanded API search terms.
* **Multi-Agent Ensemble Evaluator:** A hybrid scoring system that blends **Vector Cosine Similarity (40%)**, **LLM-as-a-Judge (40%)**, and **Bibliometric Impact (20%)** to rank papers by relevance and authority.
* **TRACE Reasoning Chains:** Autoregressively constructs Knowledge Graph (KG) triples to map how specific sentences in an abstract support a research claim.
* **Faithfulness Self-Audit:** An independent LLM auditor performs a final consistency check to ensure the generated report does not exaggerate the original paper's findings.

<div class="row justify-content-sm-center mt-5">
    <div class="col-sm-auto">
        <a href="https://github.com/Beichen-H/Research-Agent" target="_blank" class="btn btn-outline-primary btn-lg">
            <i class="fab fa-github"></i> View Source Code
        </a>
    </div>
    <div class="col-sm-auto">
        <a href="{{ '/assets/pdf/report-BeichenHu.pdf' | relative_url }}" target="_blank" class="btn btn-outline-danger btn-lg">
            <i class="fas fa-file-pdf"></i> View Research Report
        </a>
    </div>
</div>

## Technical Stack
**Frameworks:** RAG, TRACE, AGREE, E2G  
**Tools:** Python, OpenAI API, Sentence-Transformers, Semantic Scholar API  
**Methodology:** Semantic Search, Intent Translation, Multi-Agent Ensemble
