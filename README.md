# UK Renewable Infrastructure: A Multi-Scalar Geovisualisation

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Geopandas](https://img.shields.io/badge/Geopandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![HoloViews](https://img.shields.io/badge/HoloViews-blue?style=for-the-badge)
![Panel](https://img.shields.io/badge/Panel-HoloViz-orange?style=for-the-badge)

## 📌 Context & Problem: The Spatial Inequality of the UK Energy Transition
While the UK is committed to Net Zero 2050, the transition is not geographically equitable. This project identifies the **"Renewable Gap"** between high-demand urban centers and industrial "Energy Hubs." Using the **Q4 2025 Renewable Energy Planning Database (REPD)**, this tool visualizes the clustering of high-capacity infrastructure and distinguishes between "Operational Reality" and the "Planning Pipeline."

## 🛠️ Technical Pillars
This project involved advanced geospatial processing steps:
- **Coordinate Transformation:** Converting REPD data from British National Grid (EPSG:27700) to WGS84 for web mapping.
- **Spatial Clipping:** Clipping national datasets to England & Wales boundaries using a dissolved LSOA polygon.
- **Spatial Joins:** Joining 13,970 infrastructure points to 35,672 LSOA polygons to calculate neighborhood-level intensity.
- **Zonal Broadcast:** Aggregating hyper-local LSOA data up to Borough/City levels for hierarchical visualization.

## 📊 The "Maturity Index"
The core analytical component of this dashboard is the **Infrastructure Maturity Index**. It calculates the ratio of capacity that is "Operational" vs. "In Planning" for every district, identifying "Mature Hubs" versus "Emerging Hubs."

## 🖥️ Dashboard Features
- **Drill-Down UX:** Select a city to instantly update the satellite map and statistical profile.
- **Technology Mix:** Donut charts showing the energy portfolio (Solar, Wind, Battery, etc.).
- **Neighborhood Leaderboard:** Identifying the specific LSOAs driving a city's total capacity.
- **Cumulative Transition:** A line chart showing the growth path of renewable assets from 2001 to 2025.
