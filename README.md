# Bitcoin vs. S&P 500: An Investment Portfolio Analysis

This project conducts a comprehensive analysis of a dollar-cost averaging (DCA) investment strategy applied to Bitcoin (BTC) and the S&P 500 index (^GSPC). The analysis covers data collection, exploratory data analysis, investment simulation, and predictive modeling to provide a holistic view of the risks and rewards associated with each asset.

## Project Goal

The primary goal of this project is to compare and contrast the performance of Bitcoin and the S&P 500 as investment assets under a consistent, long-term DCA strategy. It aims to fulfill the following objectives:

*   **Simulate Real-World Investing**: Use real market data to simulate monthly investments over a multi-year period.
*   **Analyze and Visualize Performance**: Go beyond simple returns to analyze portfolio growth, risk-adjusted returns (Sharpe Ratio), and drawdowns.
*   **Explore Predictive Modeling**: Build and evaluate machine learning models (Random Forest and LSTM) to forecast future returns, and critically assess their effectiveness.

## Project Structure

The project is organized into four distinct Jupyter notebooks, each focusing on a specific stage of the analysis pipeline.

### 1. Data Loading and Cleaning (`01_data_loading_and_cleaning.ipynb`)

*   **Objective**: To fetch, clean, and prepare the dataset for analysis.
*   **Process**:
    *   Downloads historical daily price data for `BTC-USD` and `^GSPC` from 2015 to 2024 using the `yfinance` API.
    *   Handles missing values resulting from non-trading days using a forward-fill strategy.
    *   Saves the cleaned, processed data to `data/processed/btc_sp500_data.csv` for use in subsequent notebooks.

### 2. Exploratory Data Analysis (`02_exploratory_data_analysis.ipynb`)

*   **Objective**: To understand the statistical properties and historical behavior of the assets.
*   **Analysis**:
    *   Calculates and visualizes daily returns to understand volatility.
    *   Plots normalized price evolution to compare long-term growth.
    *   Examines the distribution of returns to identify risk profiles.
    *   Computes a correlation matrix to assess the diversification potential between the two assets.

### 3. Investment Simulation (`03_investment_simulation.ipynb`)

*   **Objective**: To simulate and evaluate a monthly dollar-cost averaging (DCA) strategy.
*   **Simulation**:
    *   Simulates a $100 monthly investment into both Bitcoin and the S&P 500.
    *   Tracks and visualizes the growth of each portfolio against the total capital invested.
    *   Calculates and visualizes portfolio drawdowns to quantify risk.
    *   Computes the Sharpe Ratio to measure risk-adjusted returns.

### 4. Predictive Analysis (`04_predictive_analysis.ipynb`)

*   **Objective**: To build and evaluate machine learning models for forecasting future returns.
*   **Models**:
    *   **Random Forest Regressor**: An ensemble model trained on lagged returns and rolling statistics.
    *   **LSTM Network**: A deep learning model designed for time-series data.
*   **Evaluation**:
    *   Both models are trained and evaluated on their ability to predict the next day's returns.
    *   Performance is measured using Root Mean Squared Error (RMSE) and R-squared (R²) scores.
    *   The notebook concludes with a critical discussion of the models' effectiveness and the inherent difficulty of predicting financial markets.

## How to Run This Project

1.  **Clone the repository:**
    ```bash
    git clone <repository-url>
    cd bitcoin_sp500_proj
    ```

2.  **Install the dependencies:**
    Make sure you have Python 3 installed. Then, install the required libraries using pip:
    ```bash
    pip install -r requirements.txt
    ```

3.  **Run the Jupyter notebooks:**
    Launch Jupyter and run the notebooks in sequential order (01 to 04) to replicate the full analysis.
    ```bash
    jupyter notebook
    ```

## Key Findings

*   **High Risk, High Reward**: The DCA simulation shows that Bitcoin offered significantly higher returns than the S&P 500 over the analysis period, but also exposed the portfolio to much deeper and more frequent drawdowns.
*   **Superior Risk-Adjusted Returns**: Despite its volatility, Bitcoin's high returns resulted in a better Sharpe Ratio, indicating strong performance even when accounting for risk.
*   **The Challenge of Prediction**: Both the Random Forest and LSTM models were unable to reliably predict future returns, yielding R² scores close to zero. This outcome highlights the efficiency of financial markets and the difficulty of forecasting using historical price data alone.