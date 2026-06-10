# GIS portfolio
----
## Overview

Throughout my career I've worked on impact projects at the intersection of conservation, territorial governance, and community data — roles that demanded systems thinking as much as technical skill. That combination naturally pulled me toward MEL and, in parallel, toward GIS as a way to make complex spatial problems legible to the people living inside them.
This repository holds two projects that reflect that path: Google Earth Engine scripts for deforestation alerts in the Mapacho Basin and fire scar vectorization in Patagonia. Small samples of a longer journey.

## Project 1 - _Deforestation Alert Report — Mapacho Basin_
Multitemporal vegetation loss analysis using Sentinel-2 L2A (10 m) in Google Earth Engine, developed as an environmental compliance input for Indigenous community territories. Computed an NDVI baseline for 2024 and detected significant vegetation decline in 2025 using a ΔNDVI threshold of −0.25, applied only where vegetation was confirmed in the baseline year — filtering out phenological noise and temporary agricultural changes. Loss was quantified per community polygon in m² and hectares, then verified visually with RGB Sentinel-2 composites. Total detected loss: 0.14 ha, concentrated in two sub-watersheds (San Miguel and Sol Naciente) where low NDVI corresponded to road construction rather than deforestation. Results indicated no evidence of widespread forest loss within the study area.

## Project 2 - _Wildfire Burn Severity Assessment — North Patagonian Forests (2022 & 2025 events)_
Spatial and temporal analysis of two wildfire events in the Bariloche Department, Río Negro, using Sentinel-2 imagery and Google Earth Engine. The Bariloche area has lost an estimated 20,000 ha of forest over the past five years, yet precise open data on burn extent and severity remains scarce — limiting both scientific analysis and community-based monitoring.

The methodology centres on the differenced Normalized Burn Ratio (dNBR), computed from pre- and post-fire Sentinel-2 composites against a 2021 baseline, to classify burn severity across the Lakes Martín, Steffen, and Los Manzanos area. Results show the 2025 event produced higher overall severity than 2022, with the most intense patches concentrated along the El Manso river valley and the Los Manzanos–Martín corridor — areas where terrain channelled fire spread. Spatial overlap between both fire scars identifies zones of repeated disturbance, flagging elevated risk of long-term ecosystem degradation.

All outputs are published as an interactive, [open-access GEE web app]([https://santiagofernandezpena.users.earthengine.app/view/severidadsteffenymartin]), making burn severity maps and vectorised fire-scar boundaries available for restoration planning, conservation management, and public accountability.
