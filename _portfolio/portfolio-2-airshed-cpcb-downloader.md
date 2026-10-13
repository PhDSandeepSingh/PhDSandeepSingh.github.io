---
title: "Air Shed Data Pipeline: 126 Northern India CAAQMS Stations"
excerpt: "Automated scraper and harmonization engine capturing 50,377 hourly intervals across 5 states.<br/><img src='https://img.shields.io/badge/Data-CPCB%20CCR-orange.svg'> <img src='https://img.shields.io/badge/Format-Parquet-purple.svg'>"
collection: portfolio
---

## Architecture & Pipeline Design
A continuous data engineering pipeline designed to ingest, validate, and structure atmospheric monitoring data from the Central Pollution Control Board (CPCB) network.

### Specifications
* **Target States:** Delhi ($n=40$), Uttar Pradesh ($n=41$), Haryana ($n=31$), Punjab ($n=9$), Himachal Pradesh ($n=5$).
* **Temporal Grid:** 1 January 2021 to 1 October 2026 (50,377 continuous hours).
* **Multi-Tier Download Engine:**
  * Mode A: Dynamic CPCB CCR portal scraper with automatic chunking (90-day windows) and exponential backoff.
  * Mode B: Automated failover to Open Government Data (`data.gov.in`) and OpenAQ v3 historical APIs.
  * Mode C: Raw archive parser harmonizing records onto canonical hourly timestamps.
* **Storage & Integrity:** Serialized to Apache Parquet with station-level SHA-256 checksums and automated missingness audit reports.

### Notebooks & Scripts
* `CPCB_Historical_Data_Downloader.ipynb`: Google Colab Pro+ compatible notebook for interactive execution.
* `create_cpcb_downloader_nb.py`: Programmatic script for generator pipeline creation.
