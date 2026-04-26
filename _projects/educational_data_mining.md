---
layout: page
title: EDUCATIONAL DATA MINING
description: Identifying hidden student engagement patterns via clustering and dimensionality reduction.
img: assets/img/edm_tsne_final.png
importance: 2
category: work
github: https://github.com/Beichen-H/Educational_Data_Mining_project
---

This project focuses on the **xAPI-Edu-Data** dataset, tracking student interactions with an LMS to identify hidden behavioral patterns that correlate with academic success or failure, providing actionable insights for educational intervention.

<div class="row justify-content-sm-center mt-4">
    <div class="col-sm-12 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/edm_tsne_final.png" title="t-SNE Clustering Structure" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    <b>Clusterability Check:</b> t-SNE visualization confirms the dataset possesses clear, globular clustering structures, validating the use of density-based or medoid-based algorithms.
</div>

<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/edm_kdistance.png" title="k-Distance Plot" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/edm_dendrogram.png" title="Single Linkage Dendrogram" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    <b>Noise & Outlier Diagnostics:</b> Left - k-Distance graph used for DBSCAN parameter tuning. Right - Single Linkage Dendrogram revealing that "outliers" are actual students with unique habits rather than system noise.
</div>

## Research Motivation
By clustering students based on engagement metrics (e.g., hand-raising, resource visits) and family support levels, we help educators design targeted intervention strategies for "at-risk" learners who might otherwise be overlooked.

## Technical Methodology
* **Outlier Analysis:** Combined KNN Distance Plots and Single Linkage Dendrograms to ensure distinct behavioral signatures were preserved for intervention analysis.
* **Noise Identification:** Used **DBSCAN** as a diagnostic tool to confirm the absence of system-level noise.
* **Data Scaling:** Applied Z-score Standardization while maintaining categorical integrity for mixed-data algorithms.
* **Clustering Optimization:** Implemented **Gower Distance** for mixed-type data, followed by **K-Medoids (PAM)** and **K-Prototypes**.

<div class="row justify-content-sm-center mt-5">
    <div class="col-sm-auto">
        <a href="https://github.com/Beichen-H/Educational_Data_Mining_project" target="_blank" class="btn btn-outline-primary btn-lg">
            <i class="fab fa-github"></i> View Source on GitHub
        </a>
    </div>
</div>

## Technical Stack
**Algorithms:** K-Medoids, K-Prototypes, DBSCAN, t-SNE  
**Metrics:** Gower Distance, Z-score Standardization  
**Visualization:** Seaborn, SciPy, Matplotlib
```

{% endraw %}
