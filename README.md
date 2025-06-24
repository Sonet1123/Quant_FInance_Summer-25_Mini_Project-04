
# Delta Hedging Under Non-Constant Volatility

This project explores the profit distribution of a delta-hedged short call position when the underlying asset exhibits **non-constant volatility**. We analyze three distinct volatility models:

- **Custom Regime-Based Volatility**: Daily volatility switches among predefined levels.
- **Heston Stochastic Volatility Model**: Mean-reverting variance driven by a correlated Brownian motion.
- **GARCH(1,1) Model**: Captures volatility clustering via lagged squared returns.

## Objective
To understand how drift (`μ`) and volatility dynamics affect the hedging performance and profitability of a short European call position, delta-hedged daily.

## Methodology
- Simulate stock paths under each model.
- Apply **Black-Scholes delta hedging**.
- Compare P&L distributions using different drift values.
- Evaluate metrics: mean profit, maximum loss, profit probability, and standard error.
- Compare performance under **Black-Scholes premium vs. model-specific premium**.

## Key Insights
- Drift has a strong impact: bearish drift improves profitability for call sellers.
- Using a Black-Scholes premium under stochastic volatility can lead to overestimated profits.
- Even with daily hedging, significant losses may occur due to volatility shocks.

## Technologies
- Python (NumPy, Matplotlib, SciPy)
- Jupyter Notebook

## Files
- `Mini Project 4.ipynb`: Full implementation
- `Report_Mini_Project-04.pdf`: full pdf report
- `functions.py`: Supporting functions for simulation and pricing

---


