# SCLM-479---Rebisco-Demand-Forecasting
📊 Rebisco Vietnam Demand Forecasting (2026–2032)
📌 Overview

This project focuses on demand forecasting for Rebisco Vietnam to support strategic supply chain planning for the period 2026–2032. The goal is to develop and evaluate multiple forecasting models in order to identify the most accurate and reliable approach for predicting product demand.

The analysis is conducted at the SKU level, using historical sales data and time-series modeling techniques in Python.

🎯 Objectives
Forecast monthly demand for Rebisco products from 2027 to 2032
Identify trends, seasonality, and demand patterns
Compare multiple forecasting models
Select the most accurate model for supply chain decision-making
📂 Dataset
Time period: 2021 – 2026
Number of records: 1,656
Granularity: SKU-level (15 SKUs across 5 brands)
Frequency: Monthly
Unit: Metric Tons (MT)
Key Features:
Year & Month
Brand & Product Name
Pack Size
Sales Volume
⚙️ Data Preprocessing

The dataset was cleaned and prepared using Python:

Converted numeric formats (comma → decimal)
Created a unified Date column
Sorted data in chronological order
Aggregated demand by month
Ensured consistent time frequency (monthly time series)

These steps ensure the dataset is suitable for time-series forecasting models.

📈 Exploratory Data Analysis (EDA)

Key insights:

📊 Upward trend: Demand increased significantly from 2021 to 2026
🔁 Strong seasonality: Peaks in January & December, lows in mid-year
🧠 Pareto effect: ~80% of demand comes from top 6–7 SKUs
🏷️ Brand dominance: KrimStix and Doowee Donut contribute the majority of demand
🤖 Forecasting Models

The following models were implemented and evaluated:

1. Baseline Models
Naïve Forecast
Moving Average
2. Exponential Smoothing
Simple Exponential Smoothing (SES)
Holt’s Linear Trend
Holt–Winters (Triple Exponential Smoothing)
3. Advanced Models
Regression with Seasonal Dummies
SARIMAX
🧪 Model Evaluation

Models were evaluated using:

MAPE (Mean Absolute Percentage Error)
MAD (Mean Absolute Deviation)
MSE / RMSE
Bias
🏆 Best Model:

Holt–Winters (Multiplicative)

Lowest MAPE (~0.37%)
Captures both trend + seasonality
Stable and reliable for long-term forecasting
🔮 Forecast Results
Demand is expected to increase steadily
Forecast range:
~2,000 MT (2027)
~3,000 MT (2032)
Seasonal patterns remain consistent
🚚 Supply Chain Implications

The forecasting results help:

Optimize inventory management
Improve production planning
Reduce stockouts & overstock
Enhance logistics and transportation planning
Support long-term strategic decisions
🛠️ Tools & Technologies
Python
Pandas, NumPy
Statsmodels
Time-series forecasting techniques
👥 Team Members
Nguyen Tuan Vu
Huynh Thuy Bao Tram
Huynh Ngoc Anh Thu
Nguyen Nhat Mai Yen
📚 Course Information
Course: SCLM 479 – Integrated Logistics and Supply Management
Institution: Eastern International University – Becamex Business School
Lecturer: Mr. Le Hoang Hai
📌 Conclusion

This project demonstrates how data-driven forecasting can significantly improve supply chain efficiency. The selected Holt–Winters model provides accurate and practical insights, enabling Rebisco Vietnam to transition from reactive to proactive planning.
