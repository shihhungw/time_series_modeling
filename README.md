# Empirical Time-Series Modeling of Mortgage Rates Using ARIMAX

This project implements an ARIMAX model to analyze and forecast Taiwan benchmark mortgage rates using macroeconomic indicators as external regressors. The objective is to construct a transparent and reproducible time-series modeling pipeline that integrates economic variables into forecasting.

## 🔍 Motivation

Understanding the relationship between interest rates and housing markets is critical for mortgage risk assessment, homebuyer behavior, and macroeconomic planning. By forecasting long-term mortgage rates, we can better assess the sensitivity of housing markets to monetary policy shifts.

## 🧠 Model

The core model used is **ARIMAX (AutoRegressive Integrated Moving Average with eXogenous variables)**, implemented with:

- **Pmdarima**: for automated model selection and diagnostics
- **Statsmodels**: for transparent modeling and statistical inspection

### Features

- Target: Mortgage Rates of New Housing Loans of 5 Major Government-owned Banks
- Exogenous regressors: macroeconomic indicators (e.g., CPI, Discount Rate)

### Workflow

1. Data preprocessing and alignment
2. Stationarity checks (ADF test)
3. Model selection with `auto_arima()`
4. Forecasting mortgage rates

## 📈 Results

- The ARIMAX model provided accurate short-horizon forecasts with interpretable coefficients.

## 🧩 Dataset

The data used in this project are publicly available from:

- Mortgage Rates of New Housing Loans of 5 Major Government-owned Banks
- Macroeconomic indicators published by Central Bank of the Republic of China

## 🧠 Reflection

This project deepened my understanding of dynamic time series modeling with external factors. ARIMAX provided a good compromise between transparency and performance, which is especially useful for financial forecasting tasks that require explainability. 

## 📌 Requirements

- Python 3.7+
- `pmdarima`
- `statsmodels`
- `pandas`, `numpy`, `matplotlib`

Install via:

```bash
pip install -r requirements.txt
