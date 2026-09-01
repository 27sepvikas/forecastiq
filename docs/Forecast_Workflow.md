# Forecast Workflow

## Overview

ForecastIQ follows a structured forecasting workflow that transforms raw historical business data into accurate, explainable, and actionable forecasts.

The workflow ensures that every forecasting model is evaluated fairly before selecting the best-performing model.

---

# End-to-End Forecast Workflow

```mermaid
flowchart LR

A[Business Understanding]

--> B[Data Collection]

--> C[Data Validation]

--> D[EDA]

--> E[Feature Engineering]

--> F[Train / Validation / Test Split]

--> G[Model Training]

--> H[Model Evaluation]

--> I[Champion Model Selection]

--> J[Forecast Generation]

--> K[What-if Simulation]

--> L[Business Dashboard]

--> M[Business Decision]
```

---

# Step 1 — Business Understanding

Define:

- Business Objective
- KPI
- Forecast Horizon
- Granularity
- Business Constraints

Example

Forecast weekly Cases Created for the next 12 weeks.

---

# Step 2 — Data Collection

Typical Inputs

- Week End Date
- Sales Forecast
- Cases Created
- Contact Ratio
- Promotions
- Holiday Calendar
- Weather
- Region

---

# Step 3 — Data Validation

ForecastIQ validates:

- Missing Values
- Duplicate Records
- Invalid Dates
- Outliers
- Frequency

---

# Step 4 — Exploratory Data Analysis

EDA includes:

- Trend Analysis
- Seasonality
- Rolling Mean
- Rolling Standard Deviation
- Correlation Matrix
- Distribution
- ACF
- PACF

---

# Step 5 — Feature Engineering

Generated Features

- Lag1
- Lag2
- Lag4
- Lag8
- Rolling Mean
- Rolling Std
- Week Number
- Month
- Quarter
- Promotion Flag
- Holiday Flag

---

# Step 6 — Data Split

Time-based split

Example

Training

Week 1 → Week 100

Validation

Week 101 → Week 112

Testing

Week 113 → Week 124

No random shuffling is used.

---

# Step 7 — Model Training

ForecastIQ supports multiple forecasting approaches.

## Statistical Models

- ARIMA
- SARIMA
- SARIMAX
- ETS
- TBATS

## Machine Learning

- XGBoost
- LightGBM
- CatBoost
- Random Forest

## Foundation Models

- TimesFM
- Chronos
- TimeGPT

---

# Step 8 — Model Evaluation

Models are compared using:

- MAPE
- RMSE
- MAE
- SMAPE
- R²
- AIC
- AICc
- BIC

---

# Step 9 — Champion Model Selection

ForecastIQ automatically identifies the best model using

- Lowest Forecast Error
- Stability
- Explainability
- Business Performance

---

# Step 10 — Forecast Generation

Outputs include

- Point Forecast
- Prediction Interval
- Confidence Interval

---

# Step 11 — What-if Simulation

Business users can simulate

- Sales Increase
- Promotion Changes
- Contact Ratio
- Holiday Impact

without retraining the model.

---

# Step 12 — Dashboard

Final outputs include

- KPI Cards
- Forecast Chart
- Model Comparison
- Forecast Table
- Download Report

---

# Final Output

ForecastIQ transforms raw historical business data into explainable forecasts that support strategic business decisions.
