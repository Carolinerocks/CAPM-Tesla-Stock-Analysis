# CAPM-Tesla-Stock-Analysis

## Project Overview
This project analyzes Tesla's stock performance using the **Capital Asset Pricing Model (CAPM)** to estimate its expected return based on market risk. By examining historical price data, we assess Tesla's risk-return profile and the effectiveness of CAPM in explaining its performance. The analysis also incorporates alternative models and metrics to provide a comprehensive evaluation of Tesla's stock.

## Introduction
The **Capital Asset Pricing Model (CAPM)** helps investors determine an asset's expected return based on its risk relative to the market. In this project, we apply CAPM to **Tesla Inc. (TSLA)** to:
- Estimate Tesla's risk profile (Beta, β).
- Calculate its expected return.
- Assess whether CAPM is a reliable tool for analyzing high-growth stocks like Tesla.


## Data Description
- **Source:** Yahoo Finance  
- **Period:** January 1, 2020 – February 1, 2025  
- **Assets:** Tesla Inc. (TSLA) and S&P 500 Index (^GSPC)  
- **Key Metrics:**  
  - Daily closing prices  
  - Daily and monthly returns  
  - Descriptive statistics (mean, median, standard deviation)  


## CAPM Model Overview
The CAPM formula is:  
**E(Ri) = Rf + βi * (E(Rm) - Rf)**  
Where:  
- **E(Ri):** Expected return of Tesla  
- **Rf:** Risk-free rate (assumed 2% annually)  
- **βi:** Beta of Tesla (systematic risk measure)  
- **E(Rm):** Expected market return  
- **(E(Rm) - Rf):** Market risk premium  


## Implementation in Python
Key steps:
1. **Data Collection:** Using `yfinance` to fetch historical prices.  
2. **Return Calculation:** Compute daily and monthly returns.  
3. **Beta Estimation:** Perform OLS regression to estimate Beta.  
4. **Expected Return:** Calculate using CAPM formula.  
5. **Validation:** Use alternative metrics (Sharpe Ratio, Jensen’s Alpha) for robustness.


## Results and Analysis
- **Beta (β):** 2.3364 — Tesla is more volatile than the market.  
- **Expected Monthly Return:** 2.55%  
- **Expected Yearly Return:** 30.56%  
- **Insights:**  
   - Tesla's high beta suggests significant risk and return potential.  
   - CAPM's limitations highlight the need for alternative models for accuracy.


## Limitations
- **Assumption of Market Efficiency:** Real markets often deviate.  
- **Beta Instability:** Beta varies over time.  
- **Exclusion of Specific Risks:** CAPM ignores company-specific risks affecting Tesla.


## Alternative Models
1. **Sharpe Ratio:** Evaluates risk-adjusted return.  
2. **Jensen’s Alpha:** Assesses if Tesla outperforms CAPM predictions.  
3. **Fama-French Model:** Considers size and value factors.  
4. **Monte Carlo Simulations:** Models multiple scenarios for Tesla's stock.


## Conclusion
CAPM provides a basic framework for analyzing Tesla’s stock but has limitations in capturing all risks. Integrating alternative models offers a more comprehensive view of Tesla’s risk-return profile, enhancing the reliability of investment decisions.
