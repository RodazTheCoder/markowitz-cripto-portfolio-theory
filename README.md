# Markowitz-Quant-Crypto: MPT Portfolio Optimization

## Project Description
This repository implements a **Modern Portfolio Theory (MPT)** framework to identify optimal cryptocurrency allocations. Unlike traditional "buy and hold" strategies, this project uses a statistical approach to balance the high volatility of crypto assets.

By leveraging a **1,000,000-iteration Monte Carlo simulation**, the engine explores the risk-return landscape of a multi-asset portfolio (BTC, SOL, DOGE, XRP) to find the **Efficient Frontier**.

### Key Technical Features:
* **Statistical Modeling:** Calculates annualized mean returns and the Asset Covariance Matrix to account for inter-token correlations.
* **Risk Management:** Implements a **40% Concentration Limit** constraint, simulating institutional risk-parity standards to prevent single-asset dependency.
* **Optimization Metrics:** Identifies the **Maximum Sharpe Ratio** portfolio (highest efficiency) and the **Global Minimum Variance** portfolio (lowest risk).
* **High-Scale Simulation:** Brute-force optimization via NumPy-accelerated matrix operations.
