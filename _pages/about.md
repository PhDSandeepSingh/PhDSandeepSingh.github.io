---
permalink: /
title: "About Me"
excerpt: "Academic Portfolio and Research Profile of Sandeep Singh"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% include base_path %}

Welcome to my academic research and data science portfolio. I am a **Ph.D. Research Scholar & Mathematics Faculty** in the **Department of Mathematics, Chandigarh University, Mohali, India (140413)** (supervised by **Prof. Ashok Pal**), currently in my third semester of doctoral research.

My research builds large-scale machine learning and deep learning systems at the intersection of **spatio-temporal environmental intelligence**, **clinical machine learning & biomedical diagnostics**, and **cybersecurity detection**, targeting Springer Nature and *Scientific Reports* (Q1/Q2) journals. Alongside my doctoral work, I have taught **Applied Mathematics** to B.E. Computer Science & Engineering students at Chandigarh University.

> **Curriculum Vitae:** [Download Full PDF CV]({{ base_path }}/files/Sandeep_Singh_CV.pdf) &middot; **Contact:** [sandeepsinghprs@gmail.com](mailto:sandeepsinghprs@gmail.com)

---

## Primary Research Pillars

### 1. Environmental Spatiotemporal Intelligence & Policy Optimization (Doctoral Thesis)
* **Airshed Intelligence Across Five Northern Indian States:** Developing a five-state air quality forecasting and control-policy optimization framework across **Punjab, Haryana, Himachal Pradesh, Uttar Pradesh, and Delhi**—integrating **115–126 CPCB continuous monitoring stations** (~20.1 million 15-minute records and 50,377 canonical hourly intervals) with **ECMWF ERA5** meteorology and **NASA FIRMS** active fire radiative power (FRP).
* **Multi-Agency Data Quality & Unit-Consistency Auditing:** Engineered a unified data infrastructure that resolves raw cross-agency anomalies, including a $\times 2.05$ $\text{NO}_x$ unit conversion discrepancy, network-wide Haryana 2025 sensor outage handling, and DPCC Delhi 1-hour vs. 15-minute resolution harmonization.
* **Regional Particulate Nowcasting:** Built multi-horizon deep learning forecasting systems (LSTM, GRU, Bi-LSTM, Bi-GRU) for Punjab and across **24 Haryana cities** with persistence baselines and formal statistical significance testing.

### 2. Clinical Machine Learning, Neuro-Oncology & Medical Imaging
* **Leakage-Free Glioma Grading & Threshold Optimization:** Designed an audited machine learning pipeline on the UCI/TCGA Glioma Grading cohort ($n = 839$, 20 somatic mutations + 3 clinical variables) using fold-safe SMOTE, nested cross-validation ($\text{ROC-AUC} = 0.931$ on sealed holdout; $\text{ROC-AUC} = 0.926$, $\text{MCC} = 0.738$, $\text{Brier} = 0.102$ across ensemble benchmarks), SHAP TreeExplainer (`IDH1` $\bar{\phi} = 0.207$ and `Age`), and clinical cost-matrix threshold optimization ($C_{\text{FN}} = 10, C_{\text{FP}} = 2$, shifting $\tau^* = 0.200$ for 97.1% GBM sensitivity and a 24% clinical cost reduction).
* **Multi-Modal Medical Imaging Diagnostics:** Led development of deep learning computer vision models across CT, X-ray, and ultrasound modalities for bone fracture and gallstone detection, validated on 1,000+ clinical images with a 20% diagnostic accuracy improvement.

### 3. Cybersecurity ML & AI-Assisted Scientific Publishing Workflows
* **Phishing & Android Malware Detection:** Built an automated machine learning and heuristic detection pipeline achieving 99.9% accuracy under adversarial robustness testing.
* **Structured Scientific Peer-Review & Writing Tools:** Authored a three-pass manuscript peer-review pipeline (editorial desk-reject screening, methodology critique, and response-letter drafting) grounded in COPE, ICMJE, and Springer Nature (`sn-jnl` / `svjour3`) guidelines.

---

## Education Snapshot
* **Ph.D. in Mathematics & Data Science** — *Chandigarh University, Mohali, India* (2025 – Present, 3rd Semester &middot; Supervisor: Prof. Ashok Pal)
* **M.Sc. in Data Science** — *Chandigarh University, Mohali, India* (Completed June 2025 &middot; GPA: 7.4 / 10)
* **B.Sc. in Information Technology** — *Maharaja Ranjit Singh Punjab Technical University (MRSPTU)* (Completed December 2019 &middot; GPA: 7.09 / 9)
