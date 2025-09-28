# 🗺️ Urbanity & Mountain Altitude — Quito Real Estate Analysis  

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)  
[![Python](https://img.shields.io/badge/python-3.9%2B-blue)](https://www.python.org/)  
[![GeoPandas](https://img.shields.io/badge/GeoPandas-0.14+-orange)](https://geopandas.org/)  

## Overview  
This project explores the relationship between **altitude**, **population density**, and **real estate prices** in **Quito, Ecuador**. By integrating geographic and housing data, it produces interactive 3D maps that reveal how elevation may influence housing values and urban settlement patterns.  

The methodology is designed to be **replicable** across multiple Latin American cities, forming a blueprint for comparative urban research.  

🔗 **Live project:** [Properati Blog](https://blog.properati.com.ec/altura-sobre-nivel-del-mar-y-viviendas-en-quito/)  
🔗 **Repository Demo:** [Demo](nicolevasos.github.io/elevation_quito/)  

---

## Objectives  
- Analyze correlations between **altitude** and **price per m²**.  
- Visualize **population density, elevation, and prices** in parallel maps.  
- Provide a **reusable workflow** for urban spatial analysis.  

---

## Data Sources  
- **Elevation:** Google Maps API  
- **Population:** INEC + Quito municipality datasets  
- **Real estate prices:** Properati listings database  

---

## Methodology  

1. **Spatial Grid Creation**  
   - Quito was divided into **500 m × 500 m cells** (250,000 m² each).  
   - Aggregated data points into uniform bins → easier pattern detection.  

2. **Data Integration**  
   - Assigned each cell:  
     - Mean **elevation**  
     - **Population count**  
     - Mean **price per m²**  

3. **Processing & Modeling**  
   - Conducted in **Python** using:  
     - `geopandas` — spatial processing  
     - `pydeck` — 3D visualization  
     - `itertools` — data handling  
   - Styling and layout managed in **HTML**  

4. **Visualization & Deployment**  
   - Interactive and 3D maps created  
   - Hosted on **GitHub**  
   - Published on **Properati Blog**  

---

## Key Findings  
- **Lower altitude** areas (Tumbaco, Cumbayá) often show **higher housing prices**.  
- Some **high-altitude zones** (near Pichincha) maintain **moderate-to-high prices**.  
- **Population density** varies widely: from >3,700 residents per cell to <635 in rural edges.  
- Relationship between **altitude & price is non-linear**, influenced by accessibility, desirability, and infrastructure.  

---

## Usage & Reproducibility  
Clone the repository and install dependencies:  

```bash
git clone https://github.com/yourusername/urbanity-altitude-quito.git
cd urbanity-altitude-quito
pip install -r requirements.txt
```
Run the notebooks or scripts to reproduce the workflow:

```bash
jupyter notebook analysis.ipynb
```

## Future Directions

- Apply methodology to **additional Latin American cities**.  
- Add new variables: **transport networks, land use, environmental risks**.  
- Experiment with **variable grid sizes** for finer resolution.  
- Develop **comparative dashboards** for multi-city analysis.  

---

## Credits

- **Research & Development:** Nicole Salazar-Cuellar  
- **Data:** INEC, Google Maps API, Properati dataset  
- **Dissemination:** Properati Blog  

