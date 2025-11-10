# 🌍 Earthquake Data Analysis (2001–2022)

_Exploratory Data Analysis (EDA) of global earthquakes to understand seismic trends, tsunami causes, and geographic risk zones using Python._

---

## 📌 Table of Contents
- [Overview](#overview)
- [Objective](#business-objective)
- [Dataset](#dataset)
- [Tools & Technologies](#tools--technologies)
- [Project Structure](#project-structure)
- [Data Preparation](#data-preparation)
- [Analysis & Visuals](#analysis--visuals)
- [Key Findings](#key-findings)
- [Insights & Interpretation](#insights--interpretation)
- [Applications & Impact](#business-impact)
- [How to Run](#how-to-run)
- [Author & Contact](#author--contact)

---

## Overview

The **Earthquake Data Analysis (2001–2022)** project focuses on identifying patterns and behaviors of earthquakes worldwide.  
The analysis distinguishes between **tsunami** and **non-tsunami** events, explores **magnitude-depth relationships**, and visualizes **geographic clustering** using Python-based EDA techniques.  

This project helps in understanding how **earthquake magnitude, depth, and location** relate to the occurrence of **tsunamis** and **impact significance**.

---

## Objective

The main goal is to:
- Analyze global earthquake trends from **2001–2022**.  
- Identify **key seismic parameters** leading to tsunamis.  
- Compare **tsunami vs. non-tsunami** earthquake characteristics.  
- Support **disaster preparedness** and **geophysical research** with clear data insights.

---

## Dataset

- **File Name:** `dc77e95e-ef74-4936-811d-e7d3bc2cd504.csv`  
- **Records:** 782  
- **Columns:** 13  
- **Source:** USGS (United States Geological Survey) dataset  

| Column | Description |
|--------|--------------|
| `magnitude` | Earthquake magnitude on the Richter scale |
| `depth` | Depth of the earthquake (in km) |
| `latitude`, `longitude` | Geographic coordinates |
| `Year`, `Month` | Time of occurrence |
| `tsunami` | 1 = Tsunami occurred, 0 = No tsunami |
| `sig` | Significance score (impact measure) |
| Other fields | `gap`, `mmi`, `cdi`, `nst`, etc. (technical attributes) |

---

## Tools & Technologies

- **Python 3.x** — Data processing & visualization  
- **Pandas** — Data manipulation and cleaning  
- **Matplotlib & Seaborn** — Visual analytics and plotting  
- **FPDF** — Automated PDF report generation  
- **GitHub** — Version control and sharing  

---

## Project Structure

```bash
earthquake-data-analysis/
│
├── README.md
├── Earthquake_Analysis_Report.pdf
├── dc77e95e-ef74-4936-811d-e7d3bc2cd504.csv
│
├── notebooks/
│   └── earthquake_eda.ipynb
│
└── images/
    ├── time_trend.png
    ├── magnitude_depth.png
    ├── geographic_distribution.png
    └── tsunami_comparison.png
```

---

## Data Preparation

Performed detailed cleaning and transformation before visualization:

- Removed missing and duplicate records.  
- Converted categorical values (`tsunami` → Yes/No).  
- Created new derived features:
  - **Yearly earthquake counts**  
  - **Average magnitude per year**  
  - **Depth categories** (Shallow, Intermediate, Deep)  

---

## Analysis & Visuals

The EDA includes multiple visual perspectives of the data:

- **📈 Time Trend Charts:** Yearly earthquake & tsunami frequencies  
- **📊 Distribution Plots:** Magnitude and depth histograms  
- **🗺️ Scatter Maps:** Geographic distribution using latitude-longitude  
- **📦 Boxplots:** Comparison between tsunami and non-tsunami events  
- **🔥 Density Maps:** Hexbin & KDE heatmaps for tsunami clustering  

![Earthquake Geographic Distribution](images/geographic_distribution.png)

---

## Key Findings

1. **Tsunami events** are less frequent but correspond to **higher magnitudes (≥7.0)**.  
2. **Shallow-focus quakes (<100 km)** are most likely to generate tsunamis.  
3. Major activity is concentrated along the **Pacific Ring of Fire**.  
4. **Significance (sig)** scores are notably higher for tsunami-related events.  
5. Earthquake frequency fluctuates annually, peaking post-2010.

---

## Insights & Interpretation

- **Magnitude drives energy release**, while **depth determines surface impact**.  
- Tsunami generation depends on **strong (≥7) shallow earthquakes** under the ocean.  
- The **Pacific Rim, Indonesia, and Chile** show repeated high-impact activity.  
- The correlation between **shallow depth**, **large magnitude**, and **tsunami occurrence** is evident.

---

## Applications & Impact

This project supports:
- **Disaster preparedness** through early warning model inputs.  
- **Risk mapping** for vulnerable coastal zones.  
- **Academic research** in geophysics and seismic behavior.  
- **Data-driven decision-making** in disaster management agencies.

---

## How to Run

1. **Clone this repository:**
```bash
   git clone https://github.com/karangadhave/earthquake-data-analysis.git
```

2. **Run the Jupyter Notebook:**
```bash
   notebooks/earthquake_eda.ipynb
```

3. **View the PDF Report:**
   Open `Earthquake_Analysis_Report.pdf` for a summary of insights.

---

## Author & Contact

**Karan Gadhave**  
📧 Email: karangadhave28@gmail.com  
💻 Field: Computer Science & Data Analysis (CSMS Student)  

🔗 [GitHub](https://github.com/karangadhave28/Earthquake-Data-Analysis) | [LinkedIn](https://www.linkedin.com/in/karan-gadhave-860299378/)

---

## 📜 License

This project is open-source under the **MIT License**.  
Feel free to use, modify, and share with proper credit.

---

### 📎 PDF Report
A detailed report of this analysis is available in:  
**`Earthquake_Analysis_Report.pdf`**
