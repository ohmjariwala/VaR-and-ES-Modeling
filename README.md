# VaR-and-ES-Modeling

This project shows how to measure Value at Risk (VaR) and Expected Shortfall (ES) for a portfolio in three different ways:

- Parametric (Variance-Covariance)
- Monte Carlo Simulation
- GARCH (Time-Varying Volatility)



  
What Are VaR and ES?
  -VaR tells you how much you could lose, with a certain confidence (like 95%), under “normal” conditions.
  -ES (Expected Shortfall) tells you how bad the loss could be on average if you exceed that VaR threshold.



1. Parametric (Variance-Covariance)
Assumes returns follow a normal distribution with a steady mean and variance.

Steps:
Calculate the mean and covariance from historical returns.
Combine them with your portfolio weights to find a single overall mean and volatility for the portfolio.
Use simple normal distribution formulas to find VaR and ES.




2. Monte Carlo Simulation
Generates many possible future outcomes by simulating random returns, then checks which outcomes are worst.

Steps:
Estimate mean and covariance from history.
Simulate a large number of random return scenarios.
Sort the simulated returns to find the worst losses for VaR, and then average those losses for ES.


3. GARCH (Time-Varying Volatility)
Risk/Vol changes over time. A GARCH model captures those changing ups and downs.

Steps:
Fit a GARCH(1,1) model to your daily returns.
Forecast how volatile the next day(s) might be.
Compute VaR and ES using this forecasted volatility instead of a constant volatility.


# Skills Used
- Risk Analytics
- Data Manipulation and Visualization
- Volatility Modeling
- Parameter Estimation
