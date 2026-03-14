# Music Sentiment and Stock Market Returns

This project investigates whether **music sentiment from Spotify** can predict **daily stock market returns of the S&P 500**. The analysis replicates and extends the methodology of Edmans et al. (2022) using econometric and time-series techniques implemented in Python.

---

## Research Question

Does Spotify music sentiment (valence) have predictive power for daily S&P 500 stock returns?

---

## Methodology

The project applies several econometric techniques to test the relationship between music sentiment and financial market performance:

* Ordinary Least Squares (OLS) regression
* Lagged sentiment regression
* Newey–West HAC robust standard errors
* AR(1) models controlling for return persistence
* Bootstrap confidence intervals
* Residual diagnostic testing
* ARIMA modelling of residuals

These methods ensure that the results remain statistically valid under potential issues such as **heteroskedasticity, autocorrelation, and time-series dependence**.

---

## Data

The analysis combines two datasets:

**Spotify Sentiment Data**

* Daily music sentiment measured using Spotify **valence**
* Aggregated across songs to construct a daily sentiment index

**Financial Market Data**

* Daily closing prices of the **S&P 500 index**
* Log returns calculated using Python

S&P 500 data is retrieved using the **Yahoo Finance API (`yfinance`)**.

---

## Key Findings

The empirical analysis finds **no statistically significant relationship** between music sentiment and S&P 500 returns for the 2023 sample period.

Main conclusions:

* Sentiment coefficients are small and statistically insignificant
* Results remain robust across lagged regressions and AR(1) models
* Newey–West HAC corrections confirm inference robustness
* Bootstrap confidence intervals include zero
* Residual diagnostics indicate well-specified models

These findings suggest that **sentiment effects may be market-specific or limited in highly efficient markets such as the U.S. equity market**.

---

## Technologies Used

Python
Pandas
NumPy
Statsmodels
Matplotlib
Seaborn
yfinance
pmdarima

---

## Repository Structure

notebooks/
→ Econometric analysis notebook containing data processing, regression models, diagnostics, and visualisations

report/
→ Full research report for the Financial Econometrics project

requirements.txt
→ Python dependencies required to reproduce the analysis

---

## Project Components

📊 Econometric analysis notebook
📄 Full research report
📦 Python environment requirements

---

## Author

Shruti Avinash Punjabi

