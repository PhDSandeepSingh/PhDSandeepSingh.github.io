---
title: "Airshed Intelligence: Five-State Spatio-Temporal ML+DL and Policy Optimization Across Northern India"
collection: publications
type: "Doctoral Thesis Project — In Preparation"
permalink: /publication/2026-airshed-cpcb-harmonization
excerpt: "A five-state air quality forecasting and policy-optimization framework covering Punjab, Haryana, Himachal Pradesh, Uttar Pradesh, and Delhi across 115–126 CPCB stations (~20.1M 15-minute records / 50,377 hourly intervals)."
date: 2026-10-01
venue: "Springer Nature / Scientific Reports (Q1/Q2 Target)"
citation: "Sandeep Singh, Ashok Pal, Sumita, et al. (2026)."
---

**Authors:** Sandeep Singh, Ashok Pal, Sumita, et al.  
**Affiliation:** Department of Mathematics, Chandigarh University, Mohali, Punjab – 140413, India

### Abstract
Reliable regional air quality forecasting and control-policy optimization across the Indo-Gangetic Plain require continuous, harmonized multi-state monitoring data. This doctoral thesis research builds a five-state spatio-temporal ML+DL framework spanning **Punjab, Haryana, Himachal Pradesh, Uttar Pradesh, and Delhi**, integrating **115–126 CPCB continuous monitoring stations** and approximately **20.1 million 15-minute resolution records** (harmonized onto a canonical 50,377-hour panel from 2021–2026).

### Key Technical & Scientific Contributions
* **Production-Grade Multi-Agency Infrastructure:** Engineered a unified station registry, standardized constants module, and multi-tier data loader with SHA-256 checksums and Apache Parquet serialization.
* **Data-Quality & Unit-Consistency Auditing:** Identified and corrected critical anomalies invisible in raw agency archives, including:
  * A $\text{NO}_x$ unit inconsistency requiring a $\times 2.05$ conversion factor.
  * Network-wide Haryana 2025 sensor outage detection and handling.
  * DPCC Delhi stations reporting at effective 1-hour (rather than 15-minute) resolution.
  * Inverted file-numbering conventions across state pollution control boards.
* **Multi-City, Multi-Horizon Deep Learning Pipeline:** Architected and audited LSTM, GRU, and Bi-LSTM forecasting pipelines across Punjab and Northern India, ensuring strict callback verification (Early Stopping, Learning Rate Reduction, and Model Checkpointing).
