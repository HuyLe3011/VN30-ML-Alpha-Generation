# 🚀 VN30 Alpha Generation: A Machine Learning Approach

## 📌 Project Overview
This repository contains the data and implementation for the research paper: *"A Machine Learning Approach to Portfolio Construction Using Predicted Financial Metrics of VN30 Firms"* (Presented at ECONVN 2026). 

The project introduces an adaptive systematic investment strategy using **Random Forest regression** to forecast the quarterly forward returns of VN30-listed companies. The predictions rely on accounting fundamentals, specifically firm size (SIZE) and return on assets (ROA). Predicted returns are standardized using Z-score normalization to generate Alpha scores, which dynamically dictate portfolio weightings.

## 🗂️ Project Structure
* `data/`: Contains fundamental financial ratios and historical price datasets (`Financial_ratios.csv`, `prices.csv`).
* `notebooks/`: 
  * `01_data_preprocessing_and_eda.ipynb`: Data cleaning, feature engineering, and preparation.
  * `02_random_forest_and_portfolio_optimization.ipynb`: Model training, Alpha score generation, and portfolio backtesting.

## 🚀 Key Technologies
* **Machine Learning:** Scikit-learn (Random Forest Regression)
* **Quantitative Finance:** Alpha Generation, Markowitz Mean-Variance Optimization, Backtesting
* **Data Processing & Visualization:** Pandas, NumPy, Matplotlib

## ⚙️ How to Run
1. Clone this repository:
```bash
git clone [https://github.com/HuyLe3011/VN30-ML-Alpha-Generation.git](https://github.com/HuyLe3011/VN30-ML-Alpha-Generation.git)
```

2. Install the required dependencies:
```bash
pip install -r requirements.txt
```

3. Open the `notebooks/` directory and execute the Jupyter notebooks in sequential order.

## ⚠️ Known Limitations & Future Work
While the Random Forest model shows promising risk-adjusted returns, future iterations will address the following quantitative modeling challenges:

* **Look-Ahead Bias:** Accounting fundamentals (e.g., ROA) are typically published weeks after the quarter ends. Future backtests will strictly apply lagging periods (e.g., 45-90 days) to fundamental features to simulate a realistic, point-in-time information flow.
* **Survivorship Bias:** The current universe relies on modern VN30 constituents. Future pipelines will dynamically reconstruct historical index constituents (including delisted or downgraded firms) to prevent the artificial inflation of out-of-sample performance.
* **Feature Expansion:** I plan to expand the feature space beyond basic financial ratios to include alternative data and macroeconomic indicators for more robust Alpha generation.
