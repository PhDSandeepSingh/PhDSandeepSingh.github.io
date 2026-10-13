---
title: "Air Shed: Automated Continuous Ingestion and Canonical Hourly Harmonization Across 126 Northern India CAAQMS Stations"
collection: publications
type: "Manuscript in Preparation"
permalink: /publication/2026-airshed-cpcb-harmonization
excerpt: "A high-throughput, rate-limit resilient data engineering engine compiling a verified 50,377-hour environmental master panel across 5 Northern Indian states."
date: 2026-10-01
venue: "Atmospheric Environment / Environmental Data Science"
citation: "Sandeep Singh, Sumita, et al. (2026)."
---

**Authors:** Sandeep Singh, Sumita, et al.

### Abstract
Reliable regional air quality modeling in Northern India requires high temporal resolution monitoring across diverse industrial, urban, and rural microclimates. This work presents an end-to-end automated data ingestion and harmonization system covering 126 continuous ambient air quality monitoring stations (CAAQMS) across five states/UTs: Delhi ($n=40$), Uttar Pradesh ($n=41$), Haryana ($n=31$), Punjab ($n=9$), and Himachal Pradesh ($n=5$).

The pipeline spans **1 January 2021 to 1 October 2026** (50,377 hourly intervals per station) capturing 23 criteria pollutants, trace gases, VOCs, and meteorological parameters. It incorporates multi-source fallback architectures (CPCB CCR portal, Open Government Data, and OpenAQ v3) alongside automated quality control manifests and SHA-256 data integrity verification.

### Key Deliverables
* Canonical hourly panel stored in optimized Apache Parquet format.
* Audit manifest tracking parameter availability per station and state.
* Comprehensive station metadata registry including verified geocoordinates and administrative identifiers.
