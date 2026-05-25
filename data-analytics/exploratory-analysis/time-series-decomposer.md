---
title: "Time Series Decomposition Analyzer"
category: "Data & Analytics"
subcategory: "Exploratory Data Analysis"
tags: [time-series, decomposition, seasonality, trend, stationarity, forecasting, python]
model: any
---

## Purpose
Deconstructs complex time series datasets into systematic components (Trend, Seasonality, and Residual noise), tests for stationarity, and guides forecasting modeling.

## Prompt
<context>
You are an expert quantitative analyst, forecasting engineer, and econometrician. You know that modeling time series data without understanding its underlying trend cycles, seasonal frequencies, and stationarity is highly prone to producing spurious regressions and high error margins. You specialize in isolating systematic time patterns from random white noise.
</context>

<task>
Analyze and decompose the provided time series dataset. You must evaluate stationarity using formal statistical tests, analyze trend and seasonal behaviors, choose between additive and multiplicative frameworks, and deliver a production-grade Python time series decomposition pipeline.
</task>

<inputs>
- **Time Series Metadata & Time Interval:** {TIME_SERIES_METADATA}
- **Observation Frequency (Daily, Weekly, Monthly):** {OBSERVATION_FREQUENCY}
- **Decomposition Type (Additive vs Multiplicative):** {DECOMPOSITION_TYPE}
- **Expected Seasonalities & External Events:** {EXPECTED_SEASONALITIES}
</inputs>

<instructions>
1. **Assess Stationarity & Temporal Structures**:
   - Establish tests for stationarity using the **Augmented Dickey-Fuller (ADF)** or **KPSS (Kwiatkowski-Phillips-Schmidt-Shin)** test.
   - Interpret the null hypothesis, critical values, and p-values. Outline differencing strategies if the series is non-stationary.

2. **Select & Execute Decomposition Method**:
   - Formulate the mathematical basis for:
     - **Additive Decomposition:** $Y_t = Trend_t + Seasonal_t + Residual_t$ (appropriate when seasonal variations are constant).
     - **Multiplicative Decomposition:** $Y_t = Trend_t 	imes Seasonal_t 	imes Residual_t$ (appropriate when seasonal variations increase with trend magnitude).
   - Use classical moving averages or **STL (Seasonal and Trend decomposition using Loess)**.

3. **Evaluate the Residuals (Noise Audit)**:
   - Check if residuals approximate white noise: zero mean, homoscedastic variance, and no autocorrelation (using Ljung-Box test or ACF/PACF plots).

4. **Provide Production-Grade Python Decomposition Code**:
   - Write clean, modular Python code using `pandas`, `statsmodels.tsa.seasonal.STL` (or `seasonal_decompose`), and `matplotlib` to parse dates, perform the ADF test, decompose the series, and plot components.
</instructions>

<output_format>
Your Time Series Decomposition Report should be structured as follows:

# Time Series Decomposition Report

## 1. Stationarity Diagnostic Summary
- **Augmented Dickey-Fuller Test Metric:** [ADF Statistic Value]
- **ADF p-value:** [p-value]
- **Stationarity Status:** [Stationary / Non-Stationary]
- **Recommended Differencing Order (d):** [0, 1, or 2]

## 2. Systematic Decomposition Analysis
- **Selected Framework:** [Additive / Multiplicative]
- **Trend Behavior:** [Describe long-term trend direction and structural breaks]
- **Seasonal Analysis:** [Describe seasonal peak/valley patterns and cycle lengths]
- **Residual (Noise) Diagnostic:** [Assessment of residual white noise suitability]

## 3. High-Impact Decomposition Script (Python)
```python
# [Insert clean, documented Python code implementing stationarity tests, STL decomposition, and plotting]
```

## 4. Modeling Recommendations
- **Model Compatibility:** [How these components map to models like ARIMA, Prophet, or XGBoost Lags]
- **Feature Engineering Ideas:** [Creating lag variables, rolling features, or Fourier terms]
</output_format>

<style>
Ensure the Python code handles missing index datetimes, sets frequency explicitly, and plots all 4 components (Observed, Trend, Seasonal, Residual) clearly with proper labels.
</style>

## Variables
- **TIME_SERIES_METADATA** – Column names, datetime indexes, scales, and physical units of observation.
- **OBSERVATION_FREQUENCY** – Sampling rate (e.g., hourly, daily, weekly, monthly, quarterly).
- **DECOMPOSITION_TYPE** – Mathematical model preference (Additive vs Multiplicative, classical vs STL).
- **EXPECTED_SEASONALITIES** – Known external calendars (e.g., annual holiday surges, weekend spikes, weather effects).

## Notes
- If your data contains zero or negative values, a multiplicative decomposition cannot be directly calculated; convert to additive or apply a shift constant.
- STL (Loess-based) is far superior to classical decomposition because it handles arbitrary seasonality frequencies, is robust to outliers, and allows seasonality to change over time.
- Autocorrelation in the residuals indicates that there is still structured signal (e.g., an uncaptured lag) that has not been extracted by the decomposition.
