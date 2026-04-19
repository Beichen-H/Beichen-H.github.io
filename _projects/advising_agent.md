---
layout: page
title: RAG Academic Advising Agent
description: An AI agent designed to automate complex academic advising inquiries at UIUC.
img: assets/img/7.jpg
importance: 1
category: Artificial Intelligence
---

Developed a **Retrieval-Augmented Generation (RAG)** prototype for the ATLAS Exploration Team at UIUC. The agent serves as an automated academic advisor, capable of answering complex degree requirements and logistical questions using high-precision semantic search.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/1.jpg" title="Pipeline Architecture" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/3.jpg" title="Semantic Search" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Left: An overview of the vector database pipeline ingesting PDF handbooks. Right: The high-precision semantic search mechanism in action. (Replace with actual system diagrams later).
</div>

## Key Technical Implementations

* **Vector Database Pipeline:** Engineered a robust pipeline to ingest and index unstructured administrative data, including official PDF handbooks and FAQs, enabling fast and context-aware retrieval.
* **Precision Semantic Search:** Implemented semantic search capabilities that allow the agent to navigate complex degree requirement hierarchies that traditional keyword search might miss.
* **Prompt Engineering & Hallucination Mitigation:** Developed specialized system prompts and quantitative evaluation metrics to ensure responses are grounded strictly in official documents.
* **Automated Logistics:** Designed the agent to handle repetitive student inquiries using Python, significantly reducing the manual workload for human advisors.

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/6.jpg" title="Performance Metrics" class="img-fluid rounded z-depth-1" %}
        <a href="https://github.com/Beichen-H/Advising-Agent" target="_blank" class="btn btn-outline-primary btn-lg">
            <i class="fab fa-github"></i> View Source on GitHub
    </div>
</div>
<div class="caption">
    Minimizing model hallucinations was a critical focus, achieved through rigorous quantitative evaluation metrics against human advisor standards.
</div>

This tool bridges the gap between static administrative handbooks and dynamic student needs, providing 24/7 accurate guidance on academic paths.
