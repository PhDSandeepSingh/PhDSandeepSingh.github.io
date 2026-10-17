---
layout: archive
title: "Curriculum Vitae"
permalink: /cv/
author_profile: true
redirect_from:
  - /cv
---

{% include base_path %}

> **Download Full CV:** [Download PDF Curriculum Vitae]({{ base_path }}/files/Sandeep_Singh_CV.pdf) *(Upload `Sandeep_Singh_CV.pdf` to the `files/` directory to activate this link)*

## Research Summary
PhD researcher and data scientist in the **Department of Mathematics, Chandigarh University, Mohali, India (140413)**, with specialized expertise in medical machine learning (oncology triage, leakage-aware validation) and environmental big data systems (multi-state air quality networks, ERA5 reanalysis, NASA FIRMS satellite data).

---

## Education
* **Ph.D. in Mathematics / Data Science & Machine Learning** *(Year – Present)*  
  *Department of Mathematics, Chandigarh University, Mohali, India, 140413*  
  * **Thesis / Focus:** Clinical Machine Learning & Environmental Spatiotemporal Intelligence
  * **Supervisor / Advisor:** [Advisor Name]
* **Master's Degree (M.Sc. / M.Tech.)** *(Year – Year)*  
  *University / Institution Name, Location*
* **Bachelor's Degree (B.Sc. / B.Tech.)** *(Year – Year)*  
  *University / Institution Name, Location*

---

## Academic & Research Appointments
* **Doctoral Researcher** | *Department of Mathematics, Chandigarh University, Mohali, India, 140413* *(Year – Present)*
  * Designing leakage-free clinical machine learning pipelines and multi-sensor environmental forecasting benchmarks.
* **Research / Teaching Assistant** | *Department of Mathematics, Chandigarh University* *(Year – Present)*
  * Supporting laboratory workshops in scientific Python, statistical modeling, and reproducible machine learning.

---

## Publications & Manuscripts
<ul>{% for post in site.publications reversed %}
  {% include archive-single-cv.html %}
{% endfor %}</ul>

---

## Research Software & Data Engineering Projects
* **Glioma Histological Grading ML Triage Pipeline:** Developed a leakage-free nested cross-validation pipeline classifying LGG vs. GBM with minimal 4-biomarker panels ($\text{AUC} = 0.931$).
* **Northern India Air Shed Downloader & Spatial Pipeline:** Automated ingestion and canonical hourly harmonization across 126 CAAQMS stations spanning 5 states/UTs ($50,377$ consecutive hourly observations).
* **ERA5 & NASA FIRMS Spatiotemporal Feature Engine:** Harmonized 10 boundary-layer meteorology variables and radial/upwind-sector satellite active fire radiative power (FRP) metrics with strict 1-day lag constraints.

---

## Technical Expertise
* **Languages & Environments:** Python, R, Bash, SQL, Git, Linux
* **Machine Learning & Deep Learning:** Scikit-Learn, XGBoost, LightGBM, PyTorch, TensorFlow, SHAP, Imbalanced-Learn
* **Data Engineering & Geospatial:** Pandas, Polars, GeoPandas, Xarray, Parquet, NetCDF, Open-Meteo API, NASA FIRMS API
* **Workflow & Reproducibility:** JupyterLab, Google Colab Pro+, Conda, Docker, Quarto, LaTeX, Jekyll

---

## Honors, Fellowships & Grants
* **[Fellowship / Award Title]** — *Awarding Body / Institution* *(Year)*
* **[Research Grant / Scholarship]** — *Funding Agency* *(Year)*

---

## Talks & Teaching
<ul>{% for post in site.talks reversed %}
  {% include archive-single-talk-cv.html %}
{% endfor %}</ul>

<ul>{% for post in site.teaching reversed %}
  {% include archive-single-cv.html %}
{% endfor %}</ul>

---

## Academic Service & Peer Review
* Participant in peer-review responses, reproducible audit reporting, and open-source scientific software releases on GitHub and Zenodo.
