# 🌍 Distribution of Ozone Levels in California  
### 📊 Spatial, Statistical & AI-Based Analysis of Air Quality Data

![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-orange)
![GeoPandas](https://img.shields.io/badge/GeoPandas-Geospatial-green)
![Plotly](https://img.shields.io/badge/Plotly-Interactive%20Visualization-purple)
![Seaborn](https://img.shields.io/badge/Seaborn-Statistical%20Visualization-teal)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Machine%20Learning-yellow)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

---

## 📌 Overview
This project explores the distribution of ozone (O₃) levels across various local areas and monitoring sites in California using **data analysis, geospatial visualization, and machine learning techniques**.

Ground-level ozone is a harmful air pollutant that affects both human health and the environment. This project aims to uncover spatial patterns, identify high-risk areas, and detect anomalies in ozone concentrations.

---

## 🎯 Objectives
- Analyze daily ozone concentration levels  
- Identify spatial distribution patterns across locations  
- Visualize ozone data using interactive maps  
- Detect abnormal ozone levels using machine learning  
- Provide insights for environmental risk analysis  

---

## 🖼️ Visualization Preview

### 🌐 Spatial Distribution Map
Geographical distribution of ozone levels using Plotly:

![Ozone Map Preview](https://raw.githubusercontent.com/ririhadis/Distribution-of-ozone-levels-in-California-local-areas-and-sites/main/assets/map_preview.png)

---

### 🔥 Spatial Heatmap
Density visualization of ozone concentration:

![Heatmap Preview](https://raw.githubusercontent.com/ririhadis/Distribution-of-ozone-levels-in-California-local-areas-and-sites/main/assets/heatmap_preview.png)

---

### 📈 Monthly Trend
Monthly variation of ozone levels:

![Monthly Trend](https://raw.githubusercontent.com/ririhadis/Distribution-of-ozone-levels-in-California-local-areas-and-sites/main/assets/monthly_trend.png)

---

## 📊 Dataset
- ~50,000+ observations  
- Geographic coordinates (latitude & longitude)  
- Daily ozone concentration values  
- Monitoring site information  

---

## 🛠️ Tech Stack

| Category          | Tools |
|------------------|------|
| Data Processing  | pandas, numpy |
| Visualization    | matplotlib, seaborn, plotly |
| Geospatial       | geopandas |
| Machine Learning | scikit-learn |
| Environment      | Jupyter Notebook |

---

## 🔍 Analysis

### 📍 Spatial Visualization (Plotly)
```python
fig = px.scatter_mapbox(
    ozone,
    lat="site_latitude",
    lon="site_longitude",
    color="daily_ozone_concentration",
    size="daily_ozone_concentration",
    size_max=15,
    zoom=5,
    mapbox_style="carto-positron"
)

🔥 Density Heatmap

sns.kdeplot(
    x=gdf.geometry.x,
    y=gdf.geometry.y
)