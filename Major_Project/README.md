# 🌾 Seasonal Agriculture Performance Analysis

An end-to-end Exploratory Data Analysis (EDA) and econometric assessment project developed for the **_VOIS Data Analytics Internship (Aug_Batch 2026–2027)**, conducted by **Vodafone Intelligent Solutions (_VOIS)** and **Vodafone Idea Foundation** in collaboration with **Edunet Foundation** and **AICTE**.

---

## 📌 Table of Contents
- [Project Overview](#-project-overview)
- [Problem Statement](#-problem-statement)
- [Key Business Questions Answered](#-key-business-questions-answered)
- [Dataset Summary](#-dataset-summary)
- [Tech Stack & Libraries](#-tech-stack--libraries)
- [Analytical Modules & Findings](#-analytical-modules--findings)
- [Strategic Policy Recommendations](#-strategic-policy-recommendations)
- [How to Run](#-how-to-run)
- [Author & Acknowledgments](#-author--acknowledgments)

---

## 📖 Project Overview
Agricultural productivity and farm financial outcomes in India depend heavily on seasonal dynamics across **Kharif**, **Rabi**, and **Zaid**[cite: 1]. This project evaluates farm-level microclimates, agronomic crop yields, irrigation efficiency, chemical input intensity, and profit-and-loss distributions across 4,000 agricultural records spanning 8 major Indian states.

---

## 🎯 Problem Statement
Agricultural activities are heavily influenced by seasonal variations in weather, resource availability, and market dynamics[cite: 1]. Raw farm data does not directly convey how crop yield and economic returns fluctuate across seasons, often leading to misallocated resources, over-reliance on inefficient irrigation systems, and unexpected financial losses for farmers. 

This project explores these seasonal variations to identify patterns, quantify resource efficiencies, and deliver evidence-based recommendations for sustainable agricultural planning.

---

## 🔍 Key Business Questions Answered
The study investigates **24 distinct analytical questions** categorized into 6 modules:
1. **Data Integrity & Imputation:** Stratified missing value handling across microclimatic and yield variables.
2. **Seasonal Microclimate Patterns:** Variations in precipitation, ambient temperature, atmospheric humidity, and soil moisture.
3. **Agronomic Productivity:** Seasonal yield per hectare benchmarks, crop suitability matrices, and seed quality correlations.
4. **Resource & Water Efficiency:** Efficiency across Drip, Sprinkler, Flood, and Rainfed irrigation methods, plus pest vulnerability cycles.
5. **Techno-Economic Viability:** Seasonal net profit distributions, operating cost drivers, and farm loss rates.
6. **Cross-Regional Diagnostics:** State-wise profitability differences and structural risk profiles of distressed farms.

---

## 📊 Dataset Summary
- **Source File:** `seasonal_agriculture_performance_dataset.csv`
- **Total Records:** 4,000 observations
- **Features Analyzed:** 28 core parameters + 5 engineered analytical metrics
- **Geographic Coverage:** 8 Indian States (Andhra Pradesh, Gujarat, Karnataka, Madhya Pradesh, Maharashtra, Punjab, Tamil Nadu, Telangana)
- **Crops Analyzed:** Rice, Wheat, Maize, Cotton, Pulses, Groundnut, Chilli, Sugarcane
- **Seasons:** Kharif (1,779 farms), Rabi (1,627 farms), Zaid (594 farms)

### Engineered Analytical Features:
* `Profit_Margin_pct`: `(Profit_INR / Revenue_INR) * 100`
* `NPK_Total_kg_ha`: Sum of Nitrogen, Phosphorus, and Potassium inputs applied
* `Cost_per_Hectare`: Total operational expenditure normalized by farm size
* `Profit_per_Hectare`: Net financial returns normalized by farm size
* `Is_Profitable`: Binary indicator classifying profitable vs. loss-making farms

---

## 🛠️ Tech Stack & Libraries
- **Language:** Python 3.x
- **Development Environment:** Google Colaboratory / Jupyter Notebook.
- **Data Wrangling:** `pandas`, `numpy`
- **Visualization & Statistical Modeling:** `matplotlib`, `seaborn`.

---

## 💡 Analytical Modules & Findings

* **Climatic Extremes:** Kharif exhibits peak precipitation (averaging 852.1 mm) and high humidity (71.8%), driving high soil moisture but elevating pest/disease risk above 50% across all crops. Zaid experiences low rainfall (299.4 mm) and high thermal stress (31.0°C).
* **Crop Economics:** Commercial crops like Sugarcane and Chilli generate high profit margins (>₹90,000/ha), whereas cereal staples (Wheat, Rice, Maize) often generate negative median net profits due to uncalibrated operational expenses.
* **Irrigation Water Efficiency:** Drip systems deliver 6.27 t/1,000 m³ and Sprinklers provide 4.67 t/1,000 m³, compared to Flood irrigation which consumes the highest volume (8,026 m³) while yielding low water efficiency (3.44 t/1,000 m³).
* **Seasonal Vulnerability:** Loss-making farm rates rise from 42.2% in Kharif to 51.1% in Rabi, and reach 64.5% during Zaid.

---

## 🏛️ Strategic Policy Recommendations
1. **Transition to Micro-Irrigation:** Restrict water-intensive flood irrigation during dry Rabi and Zaid seasons, providing targeted subsidies for Drip and Sprinkler installations.
2. **Calibrated Input Distribution:** Move away from blanket chemical fertilizer use toward soil-test-based NPK application to curb excessive operational costs per hectare.
3. **Legume & Pulse Crop Rotations:** Promote drought-tolerant pulses during water-scarce periods to reduce input costs while preserving baseline soil fertility.

---

## 🚀 How to Run

1. Open the project notebook (`.ipynb`) in **Google Colaboratory** or **Jupyter Notebook**.
2. Upload `seasonal_agriculture_performance_dataset.csv` to the working directory.
3. Run the cells sequentially to reproduce the data cleaning pipeline, summary statistics, and visual plots.

---

## 👤 Author & Acknowledgments

- **Intern / Author:** Arnab Chowdhury.
- **Internship Program:** _VOIS Data Analytics Internship (Aug_Batch 2026–2027)
- **Organized By:** Vodafone Intelligent Solutions (_VOIS) & Vodafone Idea Foundation
- **In Collaboration With:** Edunet Foundation & AICTE (All India Council for Technical Education)
