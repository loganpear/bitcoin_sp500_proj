# Bitcoin vs. S&P 500 Analysis

This project explores how Bitcoin behaves relative to the S&P 500, focusing on:
- Historical correlation between Bitcoin and the S&P 500.
- Whether Bitcoin can act as a higher-volatility proxy during equity drawdowns.
- Building data-driven signals to time Bitcoin dip-buying opportunities.

## Current Status
- Project structure established (`data/`, `notebooks/`, `reports/`).
- Planning document added in `PLAN.md`.
- A synthetic dataset (`data/raw/synthetic_btc_sp500.csv`) is generated to prototype the workflow because outbound data downloads are blocked in this environment. Once network access is available, replace it with real market data pulls.
- Initial exploratory analysis is captured in `notebooks/01_data_collection_eda.ipynb` and summarized in `reports/figures/eda_summary.txt`.


# Project Plan: Bitcoin vs S&P 500 Portfolio Analysis

## Objective
Analyze and compare the risk, return, and correlation of monthly investments in Bitcoin and the S&P 500. Simulate dollar-cost averaging (DCA) strategies and explore predictive modeling for future returns.

## Chronological Increments

### 1. Data Collection & EDA (Complete)
- Download real daily price data for Bitcoin and S&P 500 using Yahoo Finance (`yfinance`).
- Save to CSV and perform basic exploratory data analysis (EDA).

### 2. Investment Simulation
- Simulate monthly investments ($100/month) in each asset.
- Calculate and visualize portfolio growth, drawdowns, and volatility.
- Compare performance between Bitcoin and S&P 500 DCA strategies.

### 3. Advanced Statistical Analysis
- Compute rolling correlations, Sharpe ratios, and other risk metrics.
- Visualize and interpret results.

### 4. Machine Learning (Optional)
- Build and evaluate simple ML models to predict future returns or price movements.
- Discuss model performance and limitations.

### 5. Reporting & Presentation
- Summarize findings in markdown and visualizations.
- Write a clear conclusion and recommendations.
- Polish README and notebook documentation for portfolio presentation.

---

## Current Status
- Data collection and basic EDA are complete in `notebooks/01_data_collection_eda.ipynb`.
- Next: Simulate monthly investments and analyze portfolio performance.
