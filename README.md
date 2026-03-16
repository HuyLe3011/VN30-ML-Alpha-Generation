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
