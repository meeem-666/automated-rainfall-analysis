# Automated Rainfall Analysis Project
โปรเจกต์วิเคราะห์ข้อมูลน้ำฝนและจำลองภัยพิบัติฉบับเริ่มต้น
- พัฒนาโดย: นักศึกษาโยธา ปี 4 อายุ 28 ปี (มุ่งสู่สายน้ำ)
- เครื่องมือที่ใช้: Python, Google Colab

  
# 🌊 Automated Rainfall Analysis & Flash Flood Predictive System

A Python-based hydrological analysis and early warning framework designed to calculate peak runoff and estimate flash flood risks in urbanized catchments under extreme weather conditions.

---

## 📌 Project Overview
As climate change intensifies global precipitation patterns, traditional static engineering metrics are becoming obsolete. This repository showcases an automated engineering tool designed for **Disaster Mitigation and Water Resources Management**. 

By integrating **Statistical Hydrology** with **Computational Automation**, this project processes rainfall data to calculate peak discharge, evaluate drainage capacity boundaries, and instantly broadcast critical status alerts.

---

## 🛠️ Tech Stack & Engineering Core
*   **Language:** Python 3 (Google Colab / Jupyter Notebook)
*   **Core Libraries:** Pandas (Data Engineering), Matplotlib & Seaborn (Hydrological Visualization)
*   **Hydrological Framework:** Rational Method (\(Q = \frac{CIA}{360}\)), Gumbel Distribution Frequency Analysis

---

## 📂 Repository Structure
```text
automated-rainfall-early-warning/
│
├── data/
│   ├── raw/                 # Historical rainfall data (.csv) from TMD/HII
│   └── shapefiles/          # Catchment delineation GIS boundary layers
│
├── notebooks/
│   └── early_warning.ipynb  # Main Google Colab execution script for peak flow computation
│
└── README.md                # Project documentation and engineering framework
```

---

## 🚀 Hydrological Computation Engine (Sample Code)
The calculation core utilizes the **Rational Method** to convert rainfall intensity into peak runoff discharge:

```python
def calculate_peak_runoff(c, i, a):
    """
    Computes peak discharge (Q) in m³/s
    C : Runoff Coefficient (dimensionless)
    I : Rainfall Intensity (mm/hr)
    A : Catchment Area (Hectares)
    """
    return round((c * i * a) / 360, 3)
```

---

## 📈 Engineering Implications & Next Steps
*   **GIS Integration:** Next phase will map boundary inundations using QGIS and HEC-RAS 2D modeling.
*   **Geotechnical Coupling:** Integrating slope stability algorithms (Factor of Safety estimation) to predict concurrent landslide risks triggered by saturation.

---

## 👤 Developer
*   **Name:** Civil Engineering Student (Senior Year)
*   **Focus:** Water Resources Engineering & Climate Disaster Mitigation
*   **Current Goal:** Seeking Undergraduate Internship in Water Resources Consultation / Preparing for Master of Engineering Track.
