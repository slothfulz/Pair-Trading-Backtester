# Pair Trading Backtester

A Python-based statistical arbitrage project that identifies cointegrated asset pairs and evaluates a mean-reversion pair trading strategy through historical backtesting. The project combines statistical testing with rolling regression and z-score-based signal generation to assess the viability of market-neutral trading strategies.

## Features

* **Cointegration Analysis**

  * Identifies statistically related asset pairs using the Engle-Granger cointegration test.
  * Evaluates whether pairs exhibit long-term equilibrium relationships suitable for pair trading.

* **Rolling OLS Hedge Ratios**

  * Computes dynamic hedge ratios using rolling Ordinary Least Squares regression.
  * Allows hedge ratios to adapt as market relationships change over time.

* **Z-Score Trading Signals**

  * Constructs the spread between paired assets.
  * Computes rolling z-scores.
  * Generates long and short positions using configurable entry and exit thresholds.

* **Historical Backtesting**

  * Simulates trades over historical price data.
  * Tracks cumulative portfolio performance throughout the testing period.

* **Performance Evaluation**

  * Cumulative returns
  * Sharpe ratio
  * Maximum drawdown
  * Trade statistics
  * Equity curve visualization

---

## Repository Structure

```text
pair-trading-backtester/
│
├── cointegration.py     # Pair selection and statistical testing
├── backtest.py          # Trading strategy simulation and performance evaluation
└── README.md
```

---

## Workflow

1. Load historical price data.
2. Identify cointegrated asset pairs.
3. Estimate rolling OLS hedge ratios.
4. Calculate the spread and rolling z-score.
5. Generate entry and exit signals.
6. Simulate trades using historical data.
7. Evaluate strategy performance using risk and return metrics.

---

## Technologies

* Python
* Pandas
* NumPy
* Statsmodels
* SciPy
* Matplotlib


---

## Disclaimer

This project is intended for educational and research purposes only. It is not financial advice, and historical performance does not guarantee future results.
