---
layout: archive
title: "Curriculum Vitae"
permalink: /cv/
author_profile: true
redirect_from:
  - /cv
---

{% include base_path %}

> **Download Official PDF:** [**Download Sandeep Singh's Full CV (PDF)**]({{ base_path }}/files/Sandeep_Singh_CV.pdf)  
> **Affiliation:** Department of Mathematics, Chandigarh University, Mohali, Punjab – 140413, India  
> **Residence:** Ferozepur, Punjab – 152022, India &middot; **Email:** [sandeepsinghprs@gmail.com](mailto:sandeepsinghprs@gmail.com)

## Professional Summary
PhD candidate in Mathematics & Data Science at Chandigarh University, currently in the third semester of doctoral research, building large-scale machine learning and deep learning systems for applied data science projects. Author of research manuscripts at the under-review, under-revision, and in-preparation stages targeting Springer Nature and *Scientific Reports* (Q1/Q2) journals, spanning air quality nowcasting, biomedical diagnostics, and cybersecurity detection. One year of experience teaching Applied Mathematics to B.E. Computer Science & Engineering students, including lecture planning, tutorial delivery, assessment design, and examination evaluation.

---

## Education

* **Ph.D. — Mathematics & Data Science** &middot; *Chandigarh University, Mohali, Punjab, India (140413)*  
  *2025 – Present (Currently 3rd Semester) &middot; Supervisor: Prof. Ashok Pal*
  * **Doctoral Thesis:** *"Airshed Intelligence: Five-State Spatio-Temporal ML+DL and Policy Optimization"* — air quality forecasting and control-policy modeling across Punjab, Haryana, Himachal Pradesh, Uttar Pradesh, and Delhi.
  * **Focus Areas:** Spatio-temporal machine learning, deep learning, statistical modeling, environmental data science, biostatistics, policy optimization.
  * **Doctoral Output Target:** 3–4 publications in Springer Nature Q1/Q2 journals.

* **M.Sc. — Data Science** &middot; *Chandigarh University, Mohali, Punjab, India*  
  *Completed June 2025 &middot; GPA: 7.4 / 10*
  * Advanced coursework in machine learning, deep learning, health data analytics, and statistical inference.
  * **Capstone Project:** Developed a predictive modeling solution addressing real-world business and health data challenges.
  * Presented research on machine learning techniques at the university's annual Data Science Symposium.

* **B.Sc. — Information Technology** &middot; *Maharaja Ranjit Singh Punjab Technical University (MRSPTU)*  
  *Completed December 2019 &middot; GPA: 7.09 / 9*
  * **Core Coursework:** Python, Java, C++, Data Management, Cybersecurity.

---

## Research & Professional Experience

* **PhD Research Scholar & Mathematics Faculty** &middot; *Department of Mathematics, Chandigarh University, Mohali, Punjab*  
  *2025 – Present*
  * Conducting doctoral research building spatio-temporal ML/DL forecasting systems across a five-state, 115–126 station, ~20.1-million-record air quality dataset (2021–2026).
  * Taught **Applied Mathematics** to B.E. Computer Science & Engineering students (1 year) — planned lectures, conducted tutorials, developed assessments, and evaluated examinations.
  * Designing and validating ML/DL forecasting and diagnostic models; preparing manuscripts for peer-reviewed Q1/Q2 journals.
  * Built two reusable AI-assisted research tools: a structured three-pass manuscript peer-review pipeline (editorial desk-reject check, methodology critique, and response-letter drafting) grounded in COPE, ICMJE, and Springer publishing guidelines, and a scientific writing tool for manuscript and report drafting.
  * Performing literature reviews, large-scale data engineering, and quantitative analysis aligned with doctoral research objectives.

* **Business Analyst Intern** &middot; *KultureHire*  
  *Sep 2024 – Nov 2024*
  * Analyzed large datasets to identify trends, supporting strategic and operational decision-making.
  * Developed MIS dashboards and visualizations using Tableau and Excel for stakeholder presentations.
  * Collaborated cross-functionally to gather data requirements and align analytical outputs with project goals.

* **Data Analyst Intern** &middot; *KultureHire*  
  *Jun 2024 – Aug 2024*
  * Translated client business requirements into actionable data insights for development and strategy teams.
  * Conducted market research using SQL and Python; segmented customer demographics to support strategic recommendations.
  * Delivered data-driven dashboards summarizing findings for senior stakeholders.

* **Operations Manager** &middot; *MS Royal Recency (Luxury Resort)*  
  *Nov 2021 – Feb 2023*
  * Managed daily operations, overseeing 13+ staff and executing data-driven marketing strategies that increased occupancy by 15%.

---

## Manuscripts & Publications
<ul>{% for post in site.publications reversed %}
  {% include archive-single-cv.html %}
{% endfor %}</ul>

---

## Research & Technical Projects

* **Airshed Intelligence: Five-State Spatio-Temporal ML+DL and Policy Optimization** *[In Preparation — Doctoral Thesis Project]*
  * Building a five-state air quality forecasting and policy-optimization framework covering Punjab, Haryana, Himachal Pradesh, Uttar Pradesh, and Delhi, integrating 115–126 CPCB monitoring stations (~20.1 million 15-minute records and 50,377 hourly intervals).
  * Engineered a production-grade data infrastructure (station registry, standardized constants module, unified data loader) and resolved critical raw data anomalies ($\times 2.05$ $\text{NO}_x$ unit conversion factor, Haryana 2025 network sensor outage, DPCC Delhi 1-hour resolution harmonization, and inverted agency file numbering).
  * Debugged and corrected a multi-city, multi-horizon Punjab forecasting pipeline (LSTM, GRU, Bi-LSTM), restoring deep learning training callbacks (Early Stopping, Learning Rate Reduction, Model Checkpointing).

* **Hourly $\text{PM}_{2.5}$ and $\text{PM}_{10}$ Nowcasting Across 24 Haryana Cities** *[In Preparation — Manuscript Finalised for Submission]*
  * Developed an hourly $\text{PM}_{2.5}/\text{PM}_{10}$ nowcasting system across 24 Haryana cities using six ML/DL models trained on CPCB/HSPCB monitoring data, including a fourth deep learning architecture (Bi-GRU).
  * Resolved cross-architecture hyperparameter sharing bugs, added a persistence baseline with statistical significance testing, and prepared a Springer Nature (`sn-jnl`) LaTeX manuscript targeting a Q1/Q2 journal.

* **Glioma Grade Prediction — ML Pipeline with SHAP & Clinical Threshold Optimization** *[Under Revision / Review]*
  * Built an end-to-end ML diagnostic pipeline on the UCI/TCGA Glioma Grading Dataset ($n = 839$ patients, 20 somatic mutation markers + 3 clinical variables) classifying Low-Grade Glioma (LGG) vs. Glioblastoma Multiforme (GBM).
  * Implemented fold-safe SMOTE strictly inside training partitions; achieved $\text{ROC-AUC} = 0.931$ on sealed holdout under nested cross-validation (and $\text{ROC-AUC} = 0.926$, $\text{MCC} = 0.738$, $\text{Brier} = 0.102$ across ensemble evaluations).
  * Used SHAP TreeExplainer to confirm `IDH1` ($\bar{\phi} = 0.207$) and `Age` as dominant predictors aligned with WHO 2021 CNS criteria, and designed a clinical cost-matrix threshold optimization framework ($C_{\text{FN}} = 10, C_{\text{FP}} = 2$, shifting $\tau^* = 0.200$ for 97.1% GBM sensitivity and a 24% clinical cost reduction).

* **Phishing & Android Malware Detection System** *[Under Review]*
  * Built an automated detection system achieving 99.9% accuracy using machine learning and heuristic analysis, validated with adversarial robustness testing.

* **AI Diagnostic Model — Bone Fracture & Gallstone Detection**
  * Led development of deep learning computer vision models across CT, X-ray, and ultrasound modalities, validated on 1,000+ clinical images with a 20% improvement in diagnostic accuracy.

* **Gen-Z Career Aspirations & Customer Demography Analysis**
  * Designed and executed an end-to-end survey-to-dashboard analytics pipeline using SQL, Python, and Tableau to segment demographics and correlate career preference trends.

---

## Technical Skills

* **Programming:** Python (Pandas, NumPy, Polars, Scikit-learn, XGBoost, LightGBM, SHAP, TensorFlow, Keras, PyTorch), R, SQL (MySQL, PostgreSQL), Bash
* **Machine Learning & Deep Learning:** LSTM, GRU, Bi-LSTM, Bi-GRU, Ensemble Methods (Voting, Stacking), Time-Series Forecasting, Computer Vision, NLP, Imbalanced-Learn
* **Data Engineering & Geospatial:** Large-scale multi-source pipelines (20M+ records), multi-agency data harmonization, unit-consistency auditing, GeoPandas, Xarray, Parquet, NetCDF, Open-Meteo ERA5 API, NASA FIRMS API
* **Statistics:** Biostatistics, Statistical Modeling, Hypothesis Testing, Statistical Significance Testing, Regression Analysis, Survival Analysis
* **Explainability & Clinical Decision Analysis:** SHAP TreeExplainer, LIME, Feature Importance, Decision Curve Analysis (DCA), Clinical Cost-Matrix Threshold Optimization
* **Academic Writing & Publishing:** Springer Nature LaTeX (`sn-jnl`, `svjour3`), Quarto, peer-review response drafting, COPE/ICMJE guideline compliance, scientific reporting register
* **Data & MIS:** Advanced Excel (Pivot Tables, Macros, Dashboards), Tableau, Power BI
* **Databases:** MySQL, MongoDB, data extraction & query optimization
* **Teaching:** Lecture planning, tutorial delivery, assessment design, examination evaluation

---

## Certifications

* **How to Write and Publish a Scientific Paper (Project-Centered Course)** — *École Polytechnique, via Coursera* *(Feb 2026)*
* **Mindshift: Break Through Obstacles to Learning and Discover Your Hidden Potential** — *McMaster University, via Coursera* *(Feb 2026)*
* **Foundations of Teaching for Learning: Introduction** — *Commonwealth Education Trust, via Coursera* *(Jan 2026)*
* **Numerical Methods for Engineers** — *The Hong Kong University of Science and Technology, via Coursera* *(Dec 2025)*
* **University Teaching** — *The University of Hong Kong, via Coursera* *(Dec 2025)*
* **Google Data Analyst Certificate** — *Coursera*
* **Data Mining, Data Analytics & Computer Vision** — *NPTEL*
* **Python, AI & IoT** — *Chandigarh University*
* **Excel, MySQL & Machine Learning** — *KultureHire*

---

## Talks & Teaching
<ul>{% for post in site.talks reversed %}
  {% include archive-single-talk-cv.html %}
{% endfor %}</ul>

<ul>{% for post in site.teaching reversed %}
  {% include archive-single-cv.html %}
{% endfor %}</ul>

---

## Additional Information
* **Languages:** English, Hindi, Punjabi
