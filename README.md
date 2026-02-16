# 📈 NVIDIA Sales Revenue Forecasting  
### Segment-Specific Time Series Modeling with ARIMA, ARIMAX & XGBoost  

**Course:** OPIM 5671 – Data Mining and Time Series Forecasting  
**University:** University of Connecticut  
---

## 🔍 Project Overview

This project develops a **robust, segment-specific time series forecasting framework** to predict NVIDIA’s Sales Revenue across multiple regions and product categories.

Instead of applying a single global model, we implemented a **dynamic model selection strategy**, choosing the best-performing model for each Region–Product combination based on out-of-sample performance.

Three model classes were rigorously compared:

- **ARIMA (2,1,0)** – Autoregressive statistical baseline  
- **ARIMAX (2,1,0)** – Incorporating Marketing Spend as an exogenous variable  
- **XGBoost** – Machine learning approach capturing nonlinear patterns  

---

## 🎯 Objectives

- Forecast NVIDIA Sales Revenue
- Quantify the impact of Marketing Spend
- Compare statistical vs machine learning approaches
- Deliver actionable business insights
- Perform segment-level model optimization

---

## 📊 Dataset Description

The dataset simulates historical ERP transactional records (1993 onward), including:

- Date
- Product Category
- Region
- Sales Revenue (Target Variable)
- Marketing Spend (Exogenous Variable)
- Customer & product-level attributes

Each Region–Product combination was modeled as an independent time series, resulting in a panel of segment-level forecasts.

---

## 🧹 Data Preparation & Feature Engineering

- Daily data aggregated to **monthly frequency**
- Log transformation of Sales Revenue (variance stabilization)
- Standardization (Z-score) of Marketing Spend
- Chronological 12-month out-of-sample test split
- Creation of lag features for ML modeling

---

## ⚙️ Modeling Framework

| Model | Type | Strength |
|-------|------|----------|
| ARIMA (2,1,0) | Statistical | Captures autocorrelation |
| ARIMAX (2,1,0) | Causal Statistical | Quantifies marketing impact |
| XGBoost | Machine Learning | Handles nonlinear interactions |

---

## 📈 Model Evaluation

Performance was evaluated using:

- MAE (Primary selection metric)
- RMSE
- MAPE
- AIC / BIC (for ARIMA & ARIMAX)
- Ljung-Box test for residual diagnostics

Final model selection was based on **lowest out-of-sample MAE**, supported by stability diagnostics.

---

## 🏆 Key Findings

✔ No single model dominates across all segments  
✔ ARIMAX outperformed in marketing-sensitive regions  
✔ XGBoost excelled in nonlinear demand patterns  
✔ ARIMA performed best in stable historical-demand segments  

The results confirm that **forecasting performance is segment-dependent**, validating the need for a dynamic selection strategy.

---

## 📊 Business Impact

- Quantified marginal return on marketing investment (β coefficient)
- Enabled scenario-based budget simulations
- Provided segment-level revenue planning insights
- Delivered executive-ready forecasting tool

---

## 🛠 Technologies Used

- Python
- Pandas
- NumPy
- Statsmodels
- Scikit-learn
- XGBoost
- Matplotlib / Seaborn

---


---

## 📌 Skills Demonstrated

- Time Series Modeling
- ARIMA / ARIMAX
- Machine Learning Forecasting
- Feature Engineering
- Causal Inference
- Model Diagnostics
- Business Interpretation of Analytics
- Segment-Level Optimization

---

## 📎 Notes

Outputs have been cleared in the notebook to reduce file size.  
Please run all cells to reproduce results.

---

## 👨‍💻 Author

Vikram Krishnareddy  
MS Business Analytics & Project Management  
University of Connecticut


