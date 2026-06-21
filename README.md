
# AAPL Quantitative Trading Strategy

## Overview

This project develops a systematic trading strategy using Apple Inc. (AAPL) historical stock data. The strategy uses technical indicators, portfolio backtesting, risk analysis, transaction cost modeling, and walk-forward validation to evaluate quantitative trading performance.

The goal of this project was to simulate the process used by quantitative analysts when researching and evaluating systematic investment strategies.

---

## Strategy

The trading model uses a **50-day and 200-day moving average crossover strategy**:

- Buy signal: 50-day moving average crosses above the 200-day moving average
- Sell signal: 50-day moving average crosses below the 200-day moving average

The strategy was evaluated using historical AAPL price data from 2015–2024.

---

## Features

- Historical market data collection
- Moving average crossover signal generation
- Portfolio backtesting with $10,000 starting capital
- Buy-and-hold benchmark comparison
- Performance metrics:
  - Total Return
  - CAGR
  - Volatility
  - Sharpe Ratio
  - Maximum Drawdown
- Transaction cost modeling
- Walk-forward validation using unseen market data

---

## Backtesting Results

Full-period backtest results:

| Metric | Result |
|---|---:|
| Total Return | 407.27% |
| CAGR | 19.28% |
| Volatility | 24.63% |
| Sharpe Ratio | 0.84 |
| Maximum Drawdown | ~-45% |

---

## Out-of-Sample Validation

To reduce overfitting, the strategy was trained on data from 2015–2020 and tested on unseen data from 2021–2024.

Results:

| Metric | Result |
|---|---:|
| Total Return | 35.96% |
| CAGR | 8.00% |
| Volatility | 21.29% |
| Sharpe Ratio | 0.47 |

The strategy remained profitable during the validation period, demonstrating that it was able to generate returns on unseen market data.

---

## Tools Used

- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Yahoo Finance API

---

## Key Findings

The moving average crossover strategy successfully identified long-term market trends and generated positive returns. However, the strategy did not consistently outperform a passive buy-and-hold approach.

The results demonstrate the importance of out-of-sample testing, risk management, and evaluating strategies based on risk-adjusted returns rather than returns alone.

---

## Future Improvements

Potential improvements include:

- Adding additional technical indicators
- Incorporating fundamental factors
- Implementing machine learning-based signals
- Optimizing portfolio allocation
- Testing across multiple assets

---

## Author

Sean Coughlin
