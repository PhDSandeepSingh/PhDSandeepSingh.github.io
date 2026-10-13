---
title: "Satellite & Meteorological Feature Engine (ERA5 & NASA FIRMS)"
excerpt: "Multi-sensor spatiotemporal feature engineering for regional air pollution forecasting.<br/><img src='https://img.shields.io/badge/NASA-FIRMS-red.svg'> <img src='https://img.shields.io/badge/ECMWF-ERA5-blue.svg'>"
collection: portfolio
---

## System Description
This module bridges ground monitoring networks with earth observation satellites and numerical weather reanalysis models.

### Data Ingestion Modules
1. **ECMWF ERA5 Hourly Surface Meteorology:**
   * Ingests 10 boundary layer parameters: 2m temperature, relative humidity, dew point, surface pressure, precipitation, 10m wind speed, wind direction, U/V wind vectors, and surface solar radiation.
   * Auto-resuming extraction across 126 coordinates for 50,377 hours.
2. **NASA FIRMS Active Fire Dynamics:**
   * Ingests VIIRS 375m and MODIS active fire detections across the Northern India bounding box ($23.5^\circ - 33.5^\circ\text{N}$, $73.5^\circ - 84.8^\circ\text{E}$).
   * Generates radial buffer aggregations (50 km, 100 km, 200 km) for fire counts and Fire Radiative Power (FRP).
   * Computes northwest plume sector fire metrics ($270^\circ - 45^\circ$) with strict 1-day historical lag.
