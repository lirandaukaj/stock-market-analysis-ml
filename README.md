#Stock Price Predictor

Predicting Apple (AAPL) stock prices using Machine Learning and historical market data.

## Project Overview
This project explores whether machine learning can predict stock price movements
using historical price and volume data. It compares classification (direction prediction)
vs regression (price prediction) approaches.

## Results
| Metric | Value |
|--------|-------|
| Model | Random Forest Regressor |
| Stock | Apple (AAPL) 2019–2024 |
| MAE | $6.58 avg error per day |
| R² Score | 0.645 |
| Training days | 966 |
| Testing days | 242 |

## Key Findings
- **Daily return** is the strongest predictor of next-day price
- **Short-term direction** (up/down) is extremely difficult to predict — consistent with the Efficient Market Hypothesis
- **Regression** (predicting exact price) outperforms classification for this problem
- The model captures the overall trend well but struggles during high-volatility periods

## Technologies Used
- Python, Jupyter/Google Colab
- yfinance — data collection
- pandas, numpy — data processing
- matplotlib, seaborn — visualization
- scikit-learn — machine learning

## Features Used
- Moving Averages (10-day, 50-day)
- Daily Return & Volatility
- Lagged Returns (1-day, 2-day)
- 5-day Momentum
- Price vs Moving Average ratio

## How to Run
1. Open the notebook in Google Colab
2. Run all cells in order
3. Results and charts will generate automatically

## What I Learned
- Full ML pipeline: data collection → EDA → feature engineering → modeling → evaluation
- Why stock prediction is hard (Efficient Market Hypothesis)
- Difference between classification and regression problems
- How to handle time series data (no shuffling in train/test split)
