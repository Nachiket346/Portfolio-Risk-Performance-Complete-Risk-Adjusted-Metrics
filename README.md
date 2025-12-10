Objective:
Analyze the risk and performance of an equal-weighted portfolio of AAPL, JPM, and PG compared to the S&P 500 benchmark (^GSPC), using key risk-adjusted metrics and visualizations. The goal is to quantify both absolute and risk-adjusted performance while understanding drawdowns, volatility, and market sensitivity.

Process:
Data Collection: Historical price data downloaded via yfinance for portfolio assets and benchmark.
Portfolio Construction: Computed daily returns and constructed an equal-weighted portfolio.
Risk-adjusted metrics used in this project:
Sharpe Ratio
Sortino Ratio
Max Drawdown
Treynor Ratio
Information Ratio
M² (Modigliani risk-adjusted return)



Techstack:Numpy,Pandas,Matplotlib,Yfinance.

Future Enhancements:
Implement dynamic allocation strategies (risk parity, mean-variance optimization).
Add multi-factor risk decomposition (market, sector, style factors).
Incorporate Monte Carlo simulations for stress testing and scenario analysis.
Build an interactive Streamlit dashboard for live portfolio tracking.
Support multi-portfolio comparison and risk budgeting analysis.
