# Electricity Demand Forecasting using Time Series Analysis

## Introduction

Electricity consumption is a primary concern for many countries as it is a vital energy source. Electricity demand forecasting predicts future electricity usage levels, helping utilities and businesses anticipate peak demand. With the rise of digitalization, electricity demand is constantly increasing, making it crucial for companies to analyze and forecast their electricity usage for risk management purposes.

**Time series analysis** is a valuable tool for understanding electricity demand characteristics and forecasting usage patterns. This project uses time series analysis to uncover hidden relationships in electricity production data, predict future demand, and identify trends. The analysis is performed using Pandas and SARIMAX machine learning in Python.

## Solution

- **Programming language:** Python
- **Tools:** Jupyter Notebook
- **Libraries:**
  - Pandas
  - Matplotlib
  - Statsmodels.Seasonal Decompose
  - Statsmodels.SARIMAX

## Exploratory Data Analysis

The raw data consists of a time series of monthly aggregated electricity amounts from January 1st, 1985 to January 1st, 2018.

A quick visualization using Matplotlib shows the electricity generation over the years.

The data exhibits periodicity and is clean, requiring minimal data cleaning.

## Time Series Analysis

Several approaches were used for the time series analysis:
- Seasonal Decompose (by Statsmodel)
  - Additive Decompose
  - Multiplicative Decompose
- SARIMAX

### Seasonal Decompose

A time series can be split into the following components: Base Level + Trend + Seasonality + Error.

- **Additive Time Series:** Value = Base Level + Trend + Seasonality + Error
- **Multiplicative Time Series:** Value = Base Level x Trend x Seasonality x Error

### SARIMAX

SARIMAX (Seasonal Auto-Regressive Integrated Moving Average with eXogenous factors) is an advanced version of the ARIMA model. It incorporates seasonal effects and exogenous factors along with autoregressive and moving average components.

## Conclusions

The model predicts values while accounting for seasonality effects and exogenous factors, maintaining the historical trend.

## Future Work

This project provides an initial exploration of the time series data for electricity production. Further work can deepen insights and improve prediction accuracy.

Future enhancements include:
- Performing regression on the trend for additive/multiplicative decomposition to predict future values.
- Making predictions using additive/multiplicative decomposition.
- Analyzing seasonality in more detail, such as calculating the frequency of seasonality.
- Tuning hyperparameters for the SARIMAX model to maximize accuracy.

## References

1. Data Source: Time series analysis - predicting the consumption of electricity in the coming future ([link](https://www.kaggle.com/datasets/kandij/electric-production))
2. Time Series Analysis in Python ([link](https://www.machinelearningplus.com/time-series/time-series-analysis-python/))
