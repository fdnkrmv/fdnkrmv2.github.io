---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

[Download CV as PDF](/files/resume.pdf){: .btn .btn--primary}

Profile
======
Final-year PhD researcher at The University of Queensland specialising in AI, machine learning, and spatial-temporal data science. Concurrently serving as a Data Scientist and AI Engineer at Queensland Police Service, delivering production tools and analysis that directly support operational decision-making.

Research Interests
======
* Spatial-temporal learning
* Urban event forecasting
* Knowledge-guided machine learning
* Retrieval-augmented generation
* Remote sensing
* Explainable AI

Professional Experience
======
* Data Scientist and AI Engineer, Queensland Police Service
  * Build production-ready data science and AI tools for operational decision-making.
  * Develop analytical workflows that translate complex data into actionable insights.
  * Communicate technical findings to technical and non-technical stakeholders.

* PhD Researcher, The University of Queensland
  * Research machine learning approaches for context-aware urban event prediction.
  * Develop knowledge-guided and adaptive modelling approaches for dynamic environments.
  * Publish and present research at international AI venues.

Publications
======
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
Teaching
======
  <ul>{% for post in site.teaching reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
