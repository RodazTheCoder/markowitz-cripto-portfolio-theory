# Markowitz Portfolio Optimization

## About
This project applies Modern Portfolio Theory to find efficient asset allocations. It works with any ticker available on Yahoo Finance, including crypto and B3 stocks, so it can be used to build a crypto portfolio, a basket of Brazilian equities, or a mix of both.

A Monte Carlo simulation generates 100,000 random portfolios to map the risk-return space and locate the efficient frontier.

This project started as a crypto only analysis, but the underlying math doesn't care what kind of asset it's looking at, so it was later generalized to accept any ticker. The same notebook can now be used to analyze stocks, crypto, or a mix of both.

### Key features
* Calculates annualized mean returns and the covariance matrix between assets
* Applies a 40% concentration limit per asset to force diversification
* Identifies the portfolio with the highest Sharpe ratio
* Runs the simulation with NumPy vectorized operations
