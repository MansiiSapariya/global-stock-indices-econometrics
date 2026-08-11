# Global Stock Indices Econometrics

## Overview

This repository contains an econometric analysis of global stock market indices conducted as part of the **Econometrics (MDS531A)** course.

The analysis examines the behavior and interdependence of major global stock indices using **stationarity testing, first-order differencing, regression analysis, and Granger causality analysis**. The study focuses on understanding whether movements in international stock markets provide predictive information about the **NIFTY 50**.

The analysis was performed using **EViews**, and the complete methodology, outputs, interpretations, and screenshots are documented in the accompanying PDF report.

## Objectives

The main objectives of the analysis are to:

* Examine the stationarity of global stock index price series.
* Identify unit roots using the **Augmented Dickey-Fuller (ADF) test**.
* Transform non-stationary price series using first-order differencing.
* Verify stationarity after transformation.
* Analyze relationships between global stock market movements.
* Examine short-term predictive relationships using **Granger causality**.
* Determine whether movements in international indices help predict NIFTY 50 returns.

## Dataset

The analysis uses daily data for **12 global stock market indices** covering the period:

**April 2009 – December 2011**

The dataset contains **433 daily observations** and includes both price and return series. The indices covered include:

* ADX
* BOVESPA
* CAC 40
* DAX
* FTSE 100
* NASDAQ
* NIFTY 50
* NIKKEI
* SHANGAI
* TA 35
* TASI
* TSX

The dataset was provided as part of the econometrics coursework and imported into EViews. 

## Methodology

### 1. Stationarity Testing

The **Augmented Dickey-Fuller (ADF) test** was applied to the price series to determine whether they contained unit roots.

The null hypothesis states that the series contains a unit root and is therefore non-stationary.

At the 5% significance level:

* `p-value > 0.05` → Fail to reject the null → Non-stationary
* `p-value < 0.05` → Reject the null → Stationary

The initial results showed that **11 of the 12 indices were non-stationary at level**, while TASI was stationary. 

### 2. First-Order Differencing

The non-stationary series were transformed using first-order differencing.

The ADF test was then repeated on the transformed series. The results reported in the analysis showed that the differenced series achieved stationarity, making them suitable for further econometric analysis. 

### 3. Return Analysis

Return series were used for the Granger causality analysis because the model requires stationary time-series data.

The analysis examines whether past returns of global indices contain information that helps predict movements in NIFTY 50 returns. 

### 4. Granger Causality Analysis

Granger causality tests were conducted to examine short-term predictive relationships between the global indices and NIFTY 50.

The analysis specifically investigates whether past movements in each global market help predict NIFTY 50 returns.

## Key Findings

The analysis reported the following findings:

* Most global stock index price series were non-stationary at their levels.
* First-order differencing successfully produced stationary series.
* Global stock returns showed synchronized movements and responses to common market shocks.
* **8 of the 11 tested global indices showed statistically significant Granger causality with NIFTY 50 returns.**
* Significant relationships were reported for:

  * BOVESPA
  * CAC 40
  * DAX
  * FTSE 100
  * NASDAQ
  * TA 35
  * TASI
  * TSX
* No significant Granger causality was reported for:

  * ADX
  * NIKKEI
  * SHANGAI 

The report interprets these findings as evidence of short-term information transmission between several international markets and the Indian stock market. 

## Tools Used

* **EViews**
* Econometric time-series analysis
* Augmented Dickey-Fuller (ADF) testing
* First-order differencing
* Granger causality testing
* Financial time-series analysis

## Repository Structure

```text
global-stock-indices-econometrics/
│
├── README.md
├── .gitignore
│
└── docs/
    └── Lab03_Econometrics.pdf
```

## Documentation

The `docs` folder contains the complete coursework report, including:

* Data collection
* Stationarity testing
* First-order differencing
* Return analysis
* Graphical analysis
* Granger causality testing
* EViews outputs
* Interpretations
* Conclusions

## Note

This repository contains the **available coursework documentation and EViews outputs**. The original EViews workfile and underlying dataset are not included because they are not part of the available project files.

**Course:** Econometrics
**Student:** Mansi Sapariya

