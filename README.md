# Troop 3A Tactical Traffic Analysis

**Author:** Justynn Hammond  
**Role Frame:** Senior Data Analyst  
**Scope:** Colorado State Patrol – Vehicular Crimes Analysis Unit (VCAU)  
**Dataset:** Q2 Crash Data (April–June) | 2021–2025  

---

## Executive Overview

This project analyzes 1,909 crash records across a five-year period to support **tactical traffic enforcement decisions** for Troop 3A.

My objective was not only to identify where crashes are occurring, but to distinguish between:

- **High-volume crash environments**
- **High-severity (fatal/injury) risk environments**
- **Time-based risk windows**
- **Segment-level enforcement opportunities**

The analysis is structured to inform **real-world deployment strategy**, not just descriptive reporting.

---

## Key Findings

### 1. Volume vs. Severity Are Different Problems
- **I-25** drives the majority of crash volume (751 crashes)
- **Highway 85, Highway 392, I-76, and Highway 14** show higher fatal/injury rates

 This indicates different enforcement strategies are required per corridor.

---

### 2. Crash Burden Is Increasing
- Crash volume increased from **336 (2021)** to **438 (2025)**  
- Represents a **30% increase over the study period**

---

### 3. High-Risk Time Windows
- **Peak crash volume:** 1600–1700 (PM traffic)
- **Highest severity rates:** Overnight hours (00:00–04:00)
- **Highest activity days:** Thursday and Friday

---

### 4. Hotspot Concentration
- **I-25 MP 230–254** is the most concentrated crash cluster
- Multiple 5-mile segments in this range dominate the dataset

---

### 5. Causal Factor Separation
- **Following too closely** → primary volume driver
- **Impaired driving** → strongest severity driver
- **Right-of-way violations** → key factor on non-interstate roads

---

## Visual Analysis

### Corridor Analysis
![Corridors](charts/02_top_corridors.png)

---

### Hotspot Segments
![Hotspots](charts/04_hotspots.png)

---

### Hourly Risk Profile
![Hourly](charts/03_hour_profile.png)

---

### Crash Drivers (Causal Factors)
![Causal](charts/05_causal_factors.png)

---

### Day/Hour Heatmap
![Heatmap](charts/06_heatmap.png)

---

## Tactical Recommendations

### A. Volume Suppression Strategy
Focus on:
- **I-25 MP 230–254**
- Afternoon enforcement windows (1400–1800)

Recommended actions:
- Following distance enforcement
- Lane discipline visibility
- Targeted saturation patrols

---

### B. High-Severity Reduction Strategy
Focus on:
- Highway 85  
- Highway 392  
- I-76  
- Highway 14  

Recommended actions:
- DUI enforcement emphasis
- Right-of-way enforcement at intersections
- Night/overnight deployment
- Fatigue-related enforcement (I-76)

---

### C. Low-Cost Enhancements
- Portable speed feedback trailers
- Dynamic message boards
- Rotating hotspot-based enforcement
- Quarterly refresh of hotspot watchlists

---

## Analytical Constraints

This analysis is based solely on the provided dataset.

- It identifies **patterns and correlations**, not causal proof
- It supports **operational targeting**, not guaranteed outcomes
- Additional data (traffic volume, weather, road design) would further strengthen conclusions

---

## Technical Approach

The analysis was performed using:

- **Python (Pandas, NumPy)**
- **Matplotlib (custom executive styling)**
- Data cleaning for inconsistent roadway naming
- Feature engineering:
  - Severity classification
  - 5-mile segment grouping
  - Hour-based risk modeling

---

## Project Structure
troop3A_analysis/
├── notebook/
│   └── troop3A_tactical_analysis.ipynb
├── charts/
│   ├── 01_year_trend.png
│   ├── 02_top_corridors.png
│   ├── 03_hour_profile.png
│   ├── 04_hotspots.png
│   ├── 05_causal_factors.png
│   └── 06_heatmap.png
├── report/
│   └── Troop3A-Analysis_JH2026.pdf
├── data/ (excluded from repo)
└── README.md

## Data Access

The dataset used in this analysis is not included in this repository.

To reproduce:
1. Place the source Excel file in the `/data` directory
2. Update the path in the notebook if necessary

---

## Final Note

This project demonstrates how I approach:

- Translating raw data into **operational insight**
- Separating **signal from noise**
- Designing analysis that directly informs **real-world decision-making**

The goal is not just to analyze data, but to **improve outcomes through actionable intelligence**.
