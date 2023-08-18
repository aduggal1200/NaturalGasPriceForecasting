# Natural Gas Price Prediction Using SARIMA

In this repository, we delve into the prediction of natural gas prices utilizing the SARIMA (Seasonal AutoRegressive Integrated Moving Average) model. Through a meticulous data analysis process, we aim to understand the historical trends and forecast future prices.

![Initial Natural Gas Prices Over Time](./Model%20Images/initial_gas_prices_over_time.png)

## Table of Contents

1. [Introduction](#introduction)
2. [Exploratory Data Analysis](#exploratory-data-analysis)
3. [Time Series Decomposition](#time-series-decomposition)
4. [Autocorrelation and Partial Autocorrelation](#autocorrelation-and-partial-autocorrelation)
5. [Modeling and Prediction](#modeling-and-prediction)
6. [Forecast](#forecast)

## Introduction

Natural gas is a vital energy source, and understanding its price fluctuations is crucial for stakeholders involved in energy markets, policymakers, and even consumers. The above graph represents the trend of natural gas prices over the years.

## Exploratory Data Analysis

To commence our analysis, we first observed the initial natural gas prices over a span of time. This provided a visual representation of price fluctuations, helping us discern noticeable patterns and irregularities.

![Initial Natural Gas Prices Over Time](./Model%20Images/initial_gas_prices_over_time.png)

## Time Series Decomposition

Decomposing time series data can unveil hidden patterns. By breaking the data into its four primary components—Trend, Seasonal, Residual, and Observed—we gain clearer insights into the underlying structure of the time series.

![Time Series Decomposition](./Model%20Images/time_series_decomposition.png)

The decomposition diagram above helps in understanding the inherent seasonality, the general trend, and other irregular factors that might affect the gas prices.

## Autocorrelation and Partial Autocorrelation

Autocorrelation and partial autocorrelation plots are instrumental in understanding the time series data's internal structure. They help in identifying the order of the ARIMA model that can be fitted to the data.

![ACF and PACF Plot](./Model%20Images/acf_pacf_plot.png)

The above graph showcases the ACF and PACF plots, guiding the parameter selection for our SARIMA model.

## Modeling and Prediction

With a chosen model in place, we predicted natural gas prices. The graph below contrasts the actual prices with those predicted by our SARIMA model, offering a visualization of the model's accuracy.

![Actual vs Fitted Natural Gas Prices](./Model%20Images/actual_vs_fitted_prices.png)

The closeness of the actual and fitted curves suggests the robustness of the prediction model.

## SARIMA Model Results

We fit a SARIMA model with orders `(p=1, d=1, q=1)` and seasonal orders `(P=1, D=1, Q=1, S=12)` to the data. Below are the detailed results from the model fitting:

![SARIMA Model Results](./Model%20Images/SARIMAX_results.png)


These results offer insights into the performance of the SARIMA model, the significance of various parameters, and the model's overall fit to the data.


## Forecast

Armed with a calibrated model, we proceeded to forecast natural gas prices for the foreseeable future.

![Natural Gas Prices Forecast](./Model%20Images/gas_prices_forecast.png)

The above graph provides a glimpse of potential future prices, with the shaded region indicating the prediction's confidence interval.

---

Thank you for visiting this repository! 
