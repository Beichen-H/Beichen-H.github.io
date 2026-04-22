---
layout: page
title: RAG Academic Advising Agent
description: An AI agent designed to automate complex academic advising inquiries at UIUC.
img: assets/img/rag_icons.jpg
importance: 1
category: work
github: https://github.com/Beichen-H/Advising-Agent
---

Developed a **Retrieval-Augmented Generation (RAG)** prototype for the ATLAS Exploration Team at UIUC. The agent serves as an automated academic advisor, capable of answering complex degree requirements and logistical questions using high-precision semantic search.

<div class="row justify-content-sm-center mt-4">
    <div class="col-sm-12 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/rag_dashboard.jpg" title="RAG Architecture Dashboard" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    System architecture pipeline: From PDF document ingestion and text chunking, to vector semantic search, and final LLM response generation with citations.
</div>

<div class="row justify-content-sm-center mt-4">
    <div class="col-sm-10 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/rag_icons.jpg" title="RAG Core Concepts" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Core mechanisms: Navigating the knowledge base, filtering for relevance, and quoting sources accurately to eliminate hallucinations.
</div>

## Key Technical Implementations

* **Vector Database Pipeline:** Engineered a robust pipeline to ingest and index unstructured administrative data (PDF handbooks, FAQs), enabling high-precision semantic search.
* **Precision Semantic Search:** Implemented capabilities to navigate complex degree requirement hierarchies that traditional keyword search might miss.
* **Prompt Engineering & Evaluation:** Developed specialized system prompts and quantitative evaluation metrics to minimize hallucinations, benchmarking accuracy against human advisor standards.
* **Automated Logistics:** Designed the agent to handle repetitive student inquiries using Python, significantly reducing manual workload.

<div class="row justify-content-sm-center mt-5">
    <div class="col-sm-auto">
        <a href="https://github.com/Beichen-H/Advising-Agent" target="_blank" class="btn btn-outline-primary btn-lg">
            <i class="fab fa-github"></i> View Source on GitHub
        </a>
    </div>
</div>

***
*Note: This project was developed as part of the ATLAS Exploration Team at the University of Illinois Urbana-Champaign.*
