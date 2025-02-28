# Portfolio Optimization with Stochastic Programming

## Project Overview
This repository contains the implementation of a two-stage stochastic optimization model for financial portfolio management. The model is designed to maximize the amount of money invested at the start of a future period while incorporating financial instruments such as stocks, call options, and futures contracts.

## Contents
- `Python_File.ipynb`: Jupyter Notebook containing the full implementation of the optimization model.
- `Stochastic_Portfolio_Optimization.pdf`: Document explaining the theoretical background, methodology, and analysis.

## Methodology
The project applies robust and stochastic optimization techniques, leveraging:
- **Markowitz Portfolio Optimization** to minimize variance and balance risk-return trade-offs.
- **Monte Carlo Simulations** to model the uncertainty of financial markets.
- **Conditional Value at Risk (CVaR)** to assess risk based on extreme loss scenarios.
- **Multi-stage decision making** to evaluate different risk aversion settings and investment scenarios.

The model determines optimal asset allocation by considering:
- Current and future stock prices.
- The use of derivatives (call options and futures contracts) to hedge risk.
- Different levels of risk aversion to explore optimal strategies for various risk profiles.

## Data and Implementation
- **Real-time Data:** Retrieved from Yahoo Finance via the `yfinance` Python library.
- **Simulated Data:** Used for controlled scenario analysis.
- **Optimization Solver:** Implemented using `cvxpy` for convex optimization problems.

## Important Notes
- **Dynamic Outputs:** Running the code will yield different outputs due to:
  - Changing market prices.
  - Monte Carlo simulations, which are stochastic and may vary in execution.
  - EVPI (Expected Value of Perfect Information) adjustments based on new simulations.
- **Reproducibility:** The model is seeded for Monte Carlo simulations, but due to computational complexity, exact replication may not always be feasible.

## Results and Analysis
- The model was tested with both real and simulated stock data.
- Scenarios with different probability distributions were analyzed.
- The impact of risk aversion on investment decisions was explored.
- The Expected Value of Perfect Information (EVPI) was computed to measure decision quality.

## Acknowledgments
- Data Source: Yahoo Finance.
- Optimization Libraries: `cvxpy`, `numpy`, `pandas`, `matplotlib`.



