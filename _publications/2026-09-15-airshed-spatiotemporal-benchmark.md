---
title: "Integrating ECMWF ERA5 Reanalysis and NASA FIRMS Active Fire Dynamics for Regional Air Quality Benchmarking"
collection: publications
type: "Manuscript in Preparation"
permalink: /publication/2026-airshed-spatiotemporal-benchmark
excerpt: "Harmonizing satellite fire radiative power and boundary layer atmospheric reanalysis with ground sensors to eliminate lookahead bias in regional particulate forecasting."
date: 2026-09-15
venue: "Environmental Informatics / Geo-Computation"
citation: "Sandeep Singh, Sumita, et al. (2026)."
---

**Authors:** Sandeep Singh, Sumita, et al.

### Abstract
Biomass burning and seasonal meteorology drive severe episodic particulate matter spikes across the Indo-Gangetic Plain. This study establishes a rigorous spatiotemporal benchmark integrating ground-level station observations with:
1. **ECMWF ERA5 Reanalysis:** 10 surface and boundary layer variables downloaded via Open-Meteo API.
2. **NASA FIRMS Active Fires:** VIIRS (375m) and MODIS satellite detections aggregated over 50 km, 100 km, and 200 km radial buffer zones and northwest upwind plume sectors ($270^\circ - 45^\circ$).
3. **Strict Lag Enforcement:** Implementation of 1-day temporal lags across external predictors to prevent data leakage and ensure realistic operational forecast validity.
