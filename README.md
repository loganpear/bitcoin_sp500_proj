# Bitcoin vs. S&P 500 Analysis

This project explores the relationship between Bitcoin and the S&P 500, focusing on:
- Historical correlation between Bitcoin and the S&P 500.
- The viability of Bitcoin as a high-volatility investment alternative to traditional equities.
- The performance of a dollar-cost averaging (DCA) investment strategy in both assets.

## Project Structure

- `data/`: Holds raw and processed data. The project uses real daily price data for Bitcoin and the S&P 500 downloaded from Yahoo Finance (`yfinance`).
- `notebooks/`: Contains the Jupyter notebooks for the analysis.
  - `01_data_loading_and_cleaning.ipynb`: Loads and cleans the data from Yahoo Finance.
  - `02_exploratory_data_analysis.ipynb`: Performs exploratory data analysis, including correlation analysis.
  - `03_investment_simulation.ipynb`: Simulates a dollar-cost averaging investment strategy.
  - `04_predictive_analysis.ipynb`: Explores predictive modeling for future returns.
- `reports/`: Contains generated reports and figures.

## Analysis and Findings

The analysis is conducted in a series of Jupyter notebooks, each focusing on a specific aspect of the project:

1.  **Data Loading and Cleaning:** Raw daily price data for Bitcoin (BTC) and the S&P 500 (^GSPC) is fetched from Yahoo Finance for a specified date range. The data is then cleaned and prepared for analysis.

2.  **Exploratory Data Analysis:** This notebook investigates the statistical properties of the two assets. It includes visualizations of price movements over time and correlation analysis to understand how the two assets move in relation to each other, both over the entire time period and in more recent years.

3.  **Investment Simulation:** A dollar-cost averaging (DCA) investment strategy is simulated to compare the performance of regular, fixed investments in Bitcoin versus the S&P 500. The simulation calculates and visualizes portfolio growth, drawdowns, and risk-adjusted returns (Sharpe ratio).

4.  **Predictive Analysis:** This notebook explores the potential for building machine learning models to predict future returns or risk metrics.

## Usage

To run this analysis, you will need to have Python and the required libraries installed.

1.  Clone this repository.
2.  Install the dependencies:
    ```bash
    pip install -r requirements.txt
    ```
3.  Run the Jupyter notebooks in the `notebooks/` directory.