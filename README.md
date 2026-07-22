#Pair Trading Backtester

A Python-based statistical arbitrage project that identifies cointegrated asset pairs and evaluates a mean-reversion pair trading strategy through historical backtesting. The project combines statistical testing with rolling regression and z-score-based signal generation to assess the viability of market-neutral trading strategies.

Features
Cointegration Analysis
Identifies statistically related asset pairs using the Engle-Granger cointegration test.
Evaluates whether pairs exhibit long-term equilibrium relationships suitable for pair trading.
Rolling OLS Hedge Ratios
Computes dynamic hedge ratios using rolling Ordinary Least Squares regression.
Allows hedge ratios to adapt as market relationships change over time.
Z-Score Trading Signals
Constructs the spread between paired assets.
Computes rolling z-scores.
Generates long and short positions using configurable entry and exit thresholds.
Historical Backtesting
Simulates trades over historical price data.
Tracks cumulative portfolio performance throughout the testing period.
Performance Evaluation
Cumulative returns
Sharpe ratio
Maximum drawdown
Trade statistics
Equity curve visualization
