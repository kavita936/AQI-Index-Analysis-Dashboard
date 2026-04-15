# 🌫️ AQI Index Analysis Dashboard

> An interactive Power BI dashboard for analyzing Air Quality Index (AQI) trends across Indian cities, states, and years — enabling data-driven insights into air pollution patterns.

---

##  Short Description

The **AQI Index Analysis Dashboard** is a Power BI project that visualizes and analyzes Air Quality Index data across major Indian cities and states from 2018 to 2024. It enables users to explore pollution trends, identify high-risk regions, compare seasonal patterns, and understand the distribution of AQI categories — all through an interactive and intuitive interface.

Whether you're a researcher, policy analyst, student, or concerned citizen, this dashboard provides a clear window into India's air quality landscape.

---

## Tech Process

The dashboard was built using the following workflow:

**1. Data Collection**
- Raw AQI data collected from CPCB (Central Pollution Control Board) open data portal
- Data spans multiple years, cities, states, and pollutant categories

**2. Data Cleaning & Transformation**
- Cleaned and normalized using **Power Query (M Language)** inside Power BI
- Handled missing values, standardized city/state names, and converted date formats
- Created calculated columns for AQI category buckets (Good / Moderate / Unhealthy / Hazardous)

**3. Data Modeling**
- Star schema model with a central fact table (AQI readings) and dimension tables (Date, City, State, Category)
- Relationships established between tables for cross-filtering

**4. DAX Measures**
- Custom DAX measures for: Average AQI, Year-over-Year change, Rank by City/State, and Rolling Monthly Average

**5. Visualization & Publish**
- Interactive visuals built using Power BI Desktop
- Published to Power BI Service for sharing and embedding

---

## 🗃️ Data Sources

| Source | Description | Format |
|--------|-------------|--------|
| [CPCB Open Data](https://cpcb.nic.in) | Central Pollution Control Board — official AQI station data | CSV |
| [data.gov.in](https://data.gov.in) | India Open Government Data Portal — historical air quality records | CSV / Excel |
| Kaggle AQI Datasets | Supplementary cleaned datasets for historical trends | CSV |

> **Note:** Data covers the years **2018–2024** across **250+ cities** and **28+ states** in India.

---

## Features

###  Interactive Visualizations
- **AQI Trend Line Chart** — Year-over-year AQI trends for selected cities/states
- **Top 10 Polluted Cities Bar Chart** — Dynamic ranking of most polluted cities
- **Monthly AQI Heatmap** — State-wise seasonal pollution patterns across all 12 months
- **AQI Category Donut Chart** — Distribution across Good / Moderate / Unhealthy / Hazardous buckets
- **India Geo Map** — Color-coded city-level AQI map for spatial analysis

###  KPI Summary Cards
- Average AQI across filtered selection
- Total cities tracked
- Worst pollution month/season
- Best-performing (cleanest) state

###  Filter Panel (Slicers)
- **Year** — Filter by specific year or range (2018–2024)
- **State** — Drill into any Indian state
- **City** — Focus on a specific city
- **AQI Category** — Toggle between pollution severity levels

###  Dynamic Cross-Filtering
- All visuals respond interactively — clicking any chart element filters the entire dashboard
- Drill-through pages for city-level deep dives

###  Responsive Layout
- Optimized for both desktop and Power BI mobile app viewing

---

## 📸 Screenshot

![AQI Index Analysis Dashboard](AQI%20DATA.jpeg)


---

## 📖 AQI Scale Reference

| AQI Range | Category | Health Impact |
|-----------|----------|---------------|
| 0 – 50 | ✅ Good | Minimal impact |
| 51 – 100 | 🟡 Satisfactory | Minor breathing discomfort for sensitive people |
| 101 – 200 | 🟠 Moderate | Breathing discomfort for asthma/lung disease patients |
| 201 – 300 | 🔴 Poor | Breathing discomfort for most people on prolonged exposure |
| 301 – 400 | 🟣 Very Poor | Respiratory illness on prolonged exposure |
| 401 – 500 | ⚫ Severe / Hazardous | Health impacts even on light physical activity |

---
