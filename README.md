# 🛒 Migros Store Locations

An interactive **Location Intelligence** and **Business Intelligence** application developed to identify the most promising municipality for opening a new **Migros** store in the Canton of Lausanne, Switzerland.

The project combines **geospatial analytics**, **demographic information**, **socioeconomic indicators**, and **competitive landscape analysis** into a single decision-support framework. Rather than relying on intuition alone, the application evaluates multiple factors simultaneously to recommend the municipality with the highest market potential.

---

## 📖 Project Overview

Choosing the location of a new retail store is a strategic decision involving far more than simply finding an available area. Market saturation, purchasing power, population characteristics, and nearby competitors all influence the long-term success of a new store.

This project simulates a real-world consulting engagement where the objective is to identify the municipality offering the strongest business opportunity for Migros while allowing decision-makers to dynamically adjust the importance of different socioeconomic factors.

The final result is an interactive dashboard that recommends the **optimal municipality ("Champion Location")** based on customizable business priorities.

---

## 🎯 Business Objective

Identify the municipality within the Canton of Lausanne that offers the highest potential for opening a new Migros supermarket by considering:

* Existing Migros store density
* Competitor presence (Coop and Lidl)
* Population distribution
* Purchasing power
* Demographic characteristics
* Market saturation
* Socioeconomic indicators

Unlike static analyses, the application allows users to adjust weighting factors and immediately observe how recommendations change.

---

## 🗺️ Data Sources

The analysis combines multiple heterogeneous datasets, including:

### Retail Locations

* Migros stores
* Coop stores
* Lidl stores

Store locations were collected using the **Google Maps API**.

### Geographic Data

* Municipal boundaries (GeoJSON)
* Administrative regions
* Spatial reference data

### Demographic & Socioeconomic Data

* Population density
* Median income
* Age distribution
* Percentage of foreign residents
* Household size
* Additional municipality-level statistics

These datasets are integrated into a unified geospatial analysis pipeline.

---

## 🧠 Methodology

Rather than applying machine learning, this project focuses on a transparent, explainable business intelligence approach.

The location recommendation combines multiple analytical components:

* Spatial analysis of existing Migros locations
* Competitor density analysis
* Population coverage
* Purchasing power estimation
* Socioeconomic scoring
* Market saturation assessment
* Ordinary Least Squares (OLS) modelling
* User-defined weighted scoring system

The weighted scoring approach enables users to explore different business strategies depending on their priorities.

Examples include:

* Prioritizing purchasing power
* Targeting younger populations
* Focusing on municipalities with larger households
* Expanding into underserved regions
* Balancing market potential against competitive pressure

---

## 📊 Dashboard Features

The Streamlit application provides an interactive interface featuring:

* Interactive Folium maps
* Choropleth visualizations
* Municipality comparison
* Dynamic opportunity scoring
* Adjustable weighting of socioeconomic variables
* Competitive landscape visualization
* Population and demographic analysis
* Champion municipality recommendation

Changing the weighting of the evaluation criteria immediately recalculates the overall opportunity score and may produce a different recommended location.

---

## 🏆 Final Output

The primary outcome of the analysis is the identification of the **Champion Municipality** for a potential new Migros store.

The recommendation is based on a balanced evaluation of:

* Existing market saturation
* Competitor concentration
* Population characteristics
* Purchasing power
* Socioeconomic attractiveness
* User-defined business priorities

This makes the application suitable as a decision-support tool rather than a fixed recommendation engine.

---

## 💻 Technologies Used

* Python
* Streamlit
* Pandas
* NumPy
* Plotly
* Folium
* GeoPandas
* Google Maps API
* GeoJSON

---

## 📂 Project Structure

```text
migros-store-locations/
│
├── app.py
├── data/
├── geojson/
├── assets/
├── requirements.txt
└── README.md
```

---

## 🚀 Running the Project

Clone the repository:

```bash
git clone https://github.com/YOUR_USERNAME/migros-store-locations.git
cd migros-store-locations
```

Install the required dependencies:

```bash
pip install -r requirements.txt
```

Launch the Streamlit application:

```bash
streamlit run app.py
```

---

## 📸 Dashboard Preview

*Screenshots of the application can be found below.*

Suggested images:

* Executive dashboard
* Interactive choropleth map
* Opportunity score visualization
* Champion municipality recommendation
* Adjustable weighting interface

---

## 💼 Business Value

This project demonstrates how data-driven decision making can support retail expansion strategies by integrating multiple sources of information into a single analytical framework.

Rather than producing a fixed answer, the application allows decision-makers to explore alternative scenarios by adjusting the relative importance of demographic and socioeconomic factors, making the recommendation process transparent and adaptable.

---

## 🔮 Future Improvements

Potential extensions include:

* Drive-time and accessibility analysis
* Public transport accessibility
* Consumer mobility patterns
* Integration of additional competitors
* Machine learning-based demand forecasting
* Scenario simulation for future demographic changes
* Automated data updates via APIs

---

## ⚠️ Disclaimer

This project was developed for educational and portfolio purposes. The analyses and recommendations are based on publicly available geographic and socioeconomic information combined with user-defined weighting strategies and should not be interpreted as official business recommendations for Migros.

---

## 👤 Author

**Alexandros Milousis**

This project forms part of a data science and business intelligence portfolio demonstrating expertise in geospatial analytics, interactive dashboards, and data-driven decision support systems.

