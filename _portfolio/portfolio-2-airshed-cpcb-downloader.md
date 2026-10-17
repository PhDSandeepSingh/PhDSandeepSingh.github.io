---
title: "Airshed Intelligence: Five-State Spatio-Temporal ML+DL & CPCB Data Infrastructure"
excerpt: "Production-grade data infrastructure and LSTM/GRU/Bi-LSTM forecasting across 115–126 CPCB stations (~20.1M 15-minute records / 50,377 hourly intervals) spanning 5 Northern Indian states.<br/><img src='https://img.shields.io/badge/Records-20.1M+-orange.svg'> <img src='https://img.shields.io/badge/Models-LSTM%20%7C%20GRU%20%7C%20Bi--LSTM-purple.svg'>"
collection: portfolio
---

## Architecture & Doctoral Thesis Pipeline
A five-state air quality forecasting and control-policy optimization framework covering **Punjab, Haryana, Himachal Pradesh, Uttar Pradesh, and Delhi**, integrating **115–126 CPCB continuous monitoring stations** and approximately **20.1 million 15-minute resolution records** (harmonized onto a 50,377-hour canonical panel).

### Core Engineering & Auditing Milestones
* **Unified Multi-Agency Infrastructure:** Built a standardized station registry, constants module, and multi-tier downloader (CPCB CCR portal, Open Government Data `data.gov.in`, and OpenAQ v3) serialized to Apache Parquet with SHA-256 integrity verification.
* **Cross-Agency Data-Quality Auditing:** Detected and corrected critical raw-record anomalies:
  * Resolved a $\text{NO}_x$ unit inconsistency requiring a $\times 2.05$ conversion factor.
  * Handled a network-wide Haryana 2025 sensor outage.
  * Harmonized DPCC Delhi stations reporting at effective 1-hour (rather than 15-minute) resolution.
  * Corrected inverted file-numbering conventions across pollution control boards.
* **Deep Learning Forecasting Pipeline:** Audited and corrected multi-city, multi-horizon Punjab forecasting architectures (LSTM, GRU, Bi-LSTM), fixing validation-data callback wiring to restore Early Stopping, Learning Rate Reduction, and Model Checkpointing across all training runs.
