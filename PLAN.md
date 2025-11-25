# Bitcoin vs. S&P 500 Analysis Plan

## Goals
- Quantify the historical correlation between Bitcoin (BTC-USD) and the S&P 500 (^GSPC).
- Evaluate whether Bitcoin behaves like a higher-volatility proxy for the S&P 500 during market drawdowns.
- Explore a data-driven approach (e.g., machine learning or rule-based signals) to identify attractive Bitcoin dip-buying opportunities.

## Project Structure
- `data/`: data storage
  - `raw/`: downloaded datasets (e.g., historical prices)
  - `processed/`: cleaned and feature-engineered datasets
- `notebooks/`: exploratory analysis and experimentation
- `reports/figures/`: generated plots and analysis artifacts
- `src/` (future): reusable Python modules for data processing, feature engineering, and modeling
- `README.md`: project overview and quickstart

## Milestones
1. **Data Acquisition & EDA (current)**
   - Download daily historical prices for BTC-USD and ^GSPC (matching date ranges).
   - Assess missing values, coverage, summary statistics, and basic correlations.
   - Visualize price trajectories and returns distribution.
2. **Hypothesis Exploration**
   - Define "large dip" thresholds (e.g., rolling drawdown percentiles or peak-to-trough drops).
   - Compare recovery behaviors of BTC vs. S&P 500 following dips; evaluate if BTC acts as a leveraged proxy.
3. **Signal Development**
   - Engineer features (returns, volatility, drawdowns, macro proxies if available).
   - Prototype rule-based and ML-based dip-buy signals; evaluate precision/recall or profit-and-loss metrics.
4. **Backtesting & Evaluation**
   - Design a simple backtesting harness for strategy comparisons.
   - Track performance, drawdowns, and risk-adjusted metrics (e.g., Sharpe/Sortino).
5. **Reporting & Next Steps**
   - Summarize findings in a report with visuals.
   - Identify data gaps, model improvements, and risk considerations.

## Reproducibility Checklist
- Maintain environment dependencies (e.g., `requirements.txt` or `environment.yml`).
- Prefer deterministic data pulls (fixed start dates, documented sources).
- Save intermediate datasets to `data/processed/` for reusability.
- Capture key analyses in notebooks with clear markdown explanations.
- Strip notebook outputs before committing to limit merge conflicts and rely on deterministic code to regenerate figures.
