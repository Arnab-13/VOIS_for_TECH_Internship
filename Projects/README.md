# 🚗 Used Vehicle Market Trends & Depreciation Analysis

An end-to-end Exploratory Data Analysis (EDA) and pricing insights project developed as part of the **_VOIS Data Analytics Internship (August 2026 Batch)**, conducted by **Vodafone Intelligent Solutions (_VOIS)** & **Vodafone Idea Foundation** in collaboration with **Edunet Foundation** and **AICTE**.

---

## 📌 Table of Contents
- [Project Overview](#-project-overview)
- [Problem Statement](#-problem-statement)
- [Key Business Questions Answered](#-key-business-questions-answered)
- [Dataset Summary](#-dataset-summary)
- [Tech Stack & Libraries](#-tech-stack--libraries)
- [Key Insights & Findings](#-key-insights--findings)
- [How to Run](#-how-to-run)
- [Author & Acknowledgments](#-author--acknowledgments)

---

## 📖 Project Overview
Determining the fair market value of pre-owned vehicles is a major challenge in the automotive resale industry. This project applies statistical analysis and data visualization on transaction records to understand patterns in cost depreciation, brand value retention, fuel-type dynamics, mileage impact, and vehicle segment performance (Cars vs. Two-Wheelers).

---

## 🎯 Problem Statement
Setting or accepting a price for a pre-owned vehicle often suffers from subjective pricing and lack of market transparency. Both buyers and sellers struggle to quantify how multi-variable factors—such as vehicle age, kilometers driven, transmission type, fuel type, and brand equity—impact real resale value.

This project delivers a data-backed baseline to understand fair secondary market values, quantify depreciation rates, and assess resale performance across different market segments.

---

## 🔍 Key Business Questions Answered
The project analyzes **25 specific analytical questions**, including:
1. **Manufacturing Range:** Timeline spanning vehicle models from 2003 to 2018.
2. **Pricing Extremes:** Identifying lowest (₹0.10 Lakhs) and highest (₹35.00 Lakhs) resale transactions.
3. **Data Quality:** Completeness and integrity validation across all 301 records.
4. **Market Composition:** Breakdown of Fuel types (Petrol, Diesel, CNG), Transmission (Manual vs. Automatic), and Seller channels (Dealer vs. Individual).
5. **Depreciation Drivers:** Correlation between vehicle age, kilometers driven, present showroom price, and resale value.
6. **Brand Resilience:** Benchmarking value retention percentages across manufacturers (e.g., Royal Enfield, Hyundai, Maruti, Toyota).
7. **Segment Deep-Dives:** Isolated analysis of **101 Two-Wheelers** and **200 Four-Wheelers/Cars**, identifying oldest/newest models and standout deals.

---

## 📊 Dataset Summary
- **Source File:** `Car Market Trends Analysis with Car Dekho Data.csv`
- **Total Records:** 301
- **Total Features:** 9 original features + 4 engineered metrics

### Feature Attributes:
| Feature | Type | Description |
| :--- | :--- | :--- |
| `Car_Name` | Categorical | Model name / make of the vehicle |
| `Year` | Numerical | Year of manufacturing (2003 – 2018) |
| `Selling_Price` | Numerical | Price at which vehicle was sold (in ₹ Lakhs) |
| `Present_Price` | Numerical | Current ex-showroom price (in ₹ Lakhs) |
| `Kms_Driven` | Numerical | Total distance covered (in Kilometers) |
| `Fuel_Type` | Categorical | Petrol / Diesel / CNG |
| `Seller_Type` | Categorical | Dealer / Individual |
| `Transmission` | Categorical | Manual / Automatic |
| `Owner` | Numerical | Count of previous owners (0 = Single/First Owner) |

### Engineered Metrics:
- `Cost_Depreciation`: `Present_Price` - `Selling_Price`
- `Depreciation_Pct`: `(Cost_Depreciation / Present_Price) * 100`
- `Retention_Pct`: `(Selling_Price / Present_Price) * 100`
- `Vehicle_Type`: Classified into `Car` or `Two-Wheeler`
- `Brand`: Extracted make/manufacturer

---

## 🛠️ Tech Stack & Libraries
- **Language:** Python 3.x
- **Environment:** Google Colaboratory / Jupyter Notebook
- **Data Manipulation:** `pandas`, `numpy`
- **Data Visualization:** `matplotlib`, `seaborn`

---

## 💡 Key Insights & Findings
- **High Retention in Two-Wheelers:** Premium two-wheelers (e.g., Royal Enfield Classic/Thunder series) retain over 85–92% of their showroom value when mileage is low (<5,000 km).
- **Depreciation Leaders:** Luxury utility vehicles (e.g., Toyota Land Cruiser) experience the highest absolute value drop (losing up to ₹57.6 Lakhs), while budget commuter bikes lose the least absolute value.
- **Top Depreciation Determinants:** Vehicle Age ($r \approx 0.58$) and Showroom Present Price ($r \approx 0.88$) have the strongest correlation with resale value reduction.
- **Dominant Segments:** Over 79% of vehicles in the dataset are Petrol-powered, and 96.3% are single-owner vehicles (`Owner = 0`).

---

## 🚀 How to Run

1. Open the notebook (`.ipynb` file) directly in **Google Colaboratory** or **Jupyter Notebook**.
2. Upload `Car Market Trends Analysis with Car Dekho Data.csv` to the session storage.
3. Run all cells sequentially to reproduce the analytics, data frames, and visualizations.

---

## 👤 Author & Acknowledgments

- **Intern / Author:** Arnab Chowdhury
- **Internship Program:** _VOIS Data Analytics Internship (August 2026 Batch)
- **Organized By:** Vodafone Intelligent Solutions (_VOIS) & Vodafone Idea Foundation
- **In Collaboration With:** Edunet Foundation & AICTE (All India Council for Technical Education)
