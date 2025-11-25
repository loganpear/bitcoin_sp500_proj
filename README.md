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

## Next Steps
- Swap the synthetic data generation with real BTC-USD and ^GSPC historical prices when internet or a local data dump is available.
- Expand EDA with richer visuals once plotting libraries can be installed.
- Transition exploratory code into reusable modules (e.g., `src/`) for feature engineering and backtesting.
