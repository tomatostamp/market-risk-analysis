# Market Risk Analysis using VaR, CVaR & SVaR

## Overview

This project implements a simple market risk analytics system to measure potential portfolio losses under normal and stressed market conditions.

It computes key risk metrics including:

* Value at Risk (VaR): Estimates the maximum expected loss under normal market conditions at a 95% confidence level
* Conditional Value at Risk (CVaR / Expected Shortfall): Measures the average loss beyond the VaR threshold (tail risk)
* Stressed Value at Risk (SVaR): Estimates risk under stressed or adverse market conditions

---

## Tech Stack

* Python [pandas, numpy, yfinance (data ingestion), matplotlib (visualization)]

---

## Methodology

1. **Data Collection**

   * Historical stock price data fetched using yfinance

2. **Data Processing**

   * Converted price data into daily returns
   * Applied data validation and cleaning

3. **Portfolio Construction**

   * Defined weighted portfolio across multiple equities

4. **Risk Metrics Calculation**

   * VaR computed using historical simulation (percentile method)
   * CVaR computed as average of losses beyond VaR
   * SVaR computed using stressed subset of returns

5. **Visualization & Reporting**

   * Distribution of returns plotted
   * Risk metrics exported to report files


