# 🌐 California Ozone Level Analysis – Data & AI Project

[![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python&logoColor=white)](https://www.python.org/) 
[![Pandas](https://img.shields.io/badge/Pandas-Data%20Manipulation-brightgreen?logo=pandas&logoColor=white)](https://pandas.pydata.org/) 
[![NumPy](https://img.shields.io/badge/NumPy-Numerical%20Computing-orange?logo=numpy&logoColor=white)](https://numpy.org/) 
[![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-red?logo=matplotlib&logoColor=white)](https://matplotlib.org/) 
[![Seaborn](https://img.shields.io/badge/Seaborn-Visualization-blueviolet?logo=seaborn&logoColor=white)](https://seaborn.pydata.org/) 
[![Plotly](https://img.shields.io/badge/Plotly-Interactive%20Charts-lightgrey?logo=plotly&logoColor=white)](https://plotly.com/python/) 
[![GeoPandas](https://img.shields.io/badge/GeoPandas-Geospatial-teal?logo=geopandas&logoColor=white)](https://geopandas.org/) 

---

## 🚀 Project Overview
This project analyzes **ozone (O₃) levels across California** using real-world air quality datasets.  
It demonstrates a **full data engineering and exploratory analysis workflow**, highlighting skills relevant for **AI & Data Engineering roles**, without predictive modeling.

**Key focus areas for AI/Data Engineer portfolio:**
- Data preprocessing & cleaning  
- Feature engineering  
- Exploratory data analysis (EDA)  
- Interactive and geospatial visualizations  

---

## 🔑 Skills & Techniques Highlighted
- **Data Engineering:** Cleaning, merging, and transforming multi-source datasets  
- **Feature Engineering:** Handling date, location, and air quality variables  
- **EDA & Visualization:**  
  - Static plots with `matplotlib` & `seaborn`  
  - Interactive charts with `plotly.express`  
  - Geospatial mapping of monitoring sites using `geopandas` & `shapely`  
- **Python Workflow:** Structured, reproducible notebook using Jupyter  

---

## 📊 Dataset Description
The dataset contains **air quality measurements** from multiple monitoring sites in California:

| Feature | Description |
|---------|-------------|
| Date | Observation date |
| Source | Data source (EPA AQS or AirNow) |
| Site ID / POC | Monitoring site and monitor IDs |
| Daily Max 8-hour Ozone Concentration | Max ozone concentration (ppm) |
| Units | Measurement units (ppm) |
| Daily AQI Value | Air Quality Index (0–500) |
| Local Site Name | Monitoring site name |
| Daily Obs Count | Number of daily observations |
| Percent Complete | Percentage of expected samples collected |
| Method Code | Sampling method ID |
| CBSA Code / CBSA Name | Core Base Statistical Area ID and name |
| State FIPS / State | State code and name |
| County FIPS / County | County code and name |
| Site Latitude / Longitude | Geographic coordinates of the monitoring site |

---

## 🔍 Analysis Workflow

### 1. Data Preprocessing
- Merge and clean multiple data sources (EPA AQS & AirNow)  
- Convert `Date` to datetime objects  
- Handle missing or incomplete observations  
- Encode categorical variables (State, County, CBSA)  
- Engineer new features: day of week, month, season, location points  

### 2. Exploratory Data Analysis (EDA)
- Distribution analysis of ozone levels using **histograms & boxplots** (`matplotlib`, `seaborn`)  
- Trend analysis of AQI values by **state, county, and site**  
- Correlation analysis among air quality features  
- Geospatial visualization of ozone levels by site using **`geopandas` & `shapely`**  
- Interactive plots for deeper insights using **`plotly.express`**  

### 3. Monthly Maximum Ozone Analysis
- Identify the **Local Site with the highest ozone concentration for each month**  
- Display results in a **table** in the notebook  
- Visualize with **interactive bar charts** to show site rankings per month  
- Optional: Map site locations on a **geospatial map** for high-risk areas  

**Example insights:**
- Which sites consistently record the highest ozone levels  
- Seasonal patterns in ozone peaks across California  
- Identification of **high-risk areas** for poor air quality  

---

## 📈 Key Insights
- 🌡️ Ozone levels show **seasonal and temporal variation**  
- 🌬️ Wind and location influence ozone concentration patterns  
- ⚠️ Distribution is **right-skewed**, with occasional high ozone days  
- Geospatial visualization helps identify **high-risk areas**  

---

## 🧰 Tech Stack & Libraries
- Python 3.x  
- **Data Manipulation:** `pandas`, `numpy`  
- **Visualization:** `matplotlib`, `seaborn`, `plotly.express`  
- **Geospatial Analysis:** `geopandas`, `shapely`  
- **Workflow:** Jupyter Notebook  

```python
import pandas as pd
import numpy as np
import seaborn as sns
import matplotlib.pyplot as plt
import geopandas as gpd
from shapely.geometry import Point
import plotly.express as px
```
---

## 📁 Project Structure

├── notebook.ipynb   # Full data cleaning & visualization workflow

├── ozone.csv   # Dataset
├── README.md        # Project documentation

---

## ⚙️ Installation & Setup

1. Clone this repository:
git clone https://github.com/yourusername/california-ozone-analysis.git
cd california-ozone-analysis

2. Create and activate a Python virtual environment:
python -m venv venv
source venv/bin/activate  # Linux/Mac
venv\Scripts\activate     # Windows