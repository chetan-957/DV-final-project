# US Mass Shootings Data Visualization Project

A comprehensive exploratory data analysis and visualization of mass shooting incidents in the United States from **1966 to 2017**. This project leverages advanced Python libraries to uncover spatial, temporal, and statistical patterns in the dataset, with the goal of informing evidence-based discussion and public safety insights.

## 🔗 Dataset

The dataset is sourced from Kaggle:

👉 https://www.kaggle.com/datasets/zusmani/us-mass-shootings-last-50-years

It contains **398 mass shooting incidents**, including counts of fatalities, injured victims, locations, dates, and socio-demographic information.

---

## 🧠 Motivation

Mass shootings have been a persistent and tragic part of U.S. history. By analyzing patterns over time and space, we aim to:

* Understand frequency and trends
* Highlight high-impact states and years
* Explore socio-economic and demographic contributors
* Provide visual storytelling that supports discussion and policy thinking

---

## 🚀 Key Contributions

This project delivers:

* **Cleaned and enriched dataset** with separated date and location fields  
* **Statistical summaries** of trends over time  
* **State-level aggregation** of total victims, injuries, and fatalities  
* Multiple **visualizations** highlighting key patterns  
* A reproducible notebook for exploratory data analysis

---

## 🧩 Data Description

Key features used:

| Column | Meaning |
|--------|---------|
| Location | City, State |
| Date | Incident date |
| Fatalities | Number of deaths |
| Injured | Number of non-fatal injuries |
| Total victims | Fatalities + Injured |
| Mental Health Issues | Whether perpetrator had mental health issues |
| Age, Race, Gender | Perpetrator characteristics |
| Cause | Reason/motivation reported |

Additional columns created programmatically:

* `Month`, `Day`, `Year`  
* `City`, `State` (split from Location)  

---

## 🛠️ Libraries Used

```python
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
import plotly.express as px
import geopandas as gpd
from shapely.geometry import Point
import folium
from folium.plugins import HeatMap
