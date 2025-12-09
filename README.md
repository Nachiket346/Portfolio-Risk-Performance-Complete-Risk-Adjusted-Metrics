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

Results:

| Metric                | Portfolio | Benchmark (^GSPC) |
| --------------------- | --------- | ----------------- |
| Annual Return (%)     | 28.5      | 15.2              |
| Annual Volatility (%) | 20.1      | 18.5              |
| Sharpe Ratio          | 1.42      | 0.82              |
| Sortino Ratio         | 2.10      | 1.25              |
| Max Drawdown (%)      | -19.8     | -14.3             |
| Treynor Ratio         | 1.56      | 0.88              |
| Information Ratio     | 0.68      | -                 |
| M² (%)                | 22.5      | 15.2              |

Interpretation:
Achieved 28.5% annualized return, outperforming the benchmark (15.2%) with moderate additional volatility (20.1% vs 18.5%).
Delivered superior risk-adjusted performance: Sharpe (1.42 vs 0.82) and Sortino (2.10 vs 1.25) ratios indicate efficient reward per unit of total and downside risk.
Managed systematic risk effectively: Treynor ratio (1.56) and positive Information Ratio (0.68) show consistent outperformance relative to benchmark.
Strong overall risk-adjusted return (M² = 22.5%) confirms outperformance when scaled to benchmark volatility, despite slightly higher drawdown (-19.8% vs -14.3%).

Techstack:Numpy,Pandas,Matplotlib,Yfinance.

Future Enhancements:
Implement dynamic allocation strategies (risk parity, mean-variance optimization).
Add multi-factor risk decomposition (market, sector, style factors).
Incorporate Monte Carlo simulations for stress testing and scenario analysis.
Build an interactive Streamlit dashboard for live portfolio tracking.
Support multi-portfolio comparison and risk budgeting analysis.
