Objective:
Analyze the risk and performance of an equal-weighted portfolio of AAPL, JPM, and PG compared to the S&P 500 benchmark (^GSPC), using key risk-adjusted metrics and visualizations. The goal is to quantify both absolute and risk-adjusted performance while understanding drawdowns, volatility, and market sensitivity.

Process:
Collected historical daily price data for AAPL, JPM, PG, and S&P 500 (benchmark).
Computed daily returns, portfolio returns (equal-weighted), and cumulative returns.
Calculated both portfolio & benchmark risk-adjusted metrics:
Sharpe Ratio
Sortino Ratio
Max Drawdown
Treynor Ratio
Information Ratio
M² (Modigliani risk-adjusted return)

Results:

| **Metric**            | **Portfolio** | **Benchmark** |
| --------------------- | ------------- | ------------- |
| **Annual Return**     | **0.186239**  | **0.128169**  |
| **Annual Volatility** | **0.18594**   | **0.17351**   |
| **Sharpe Ratio**      | **1.001606**  | **0.738684**  |
| **Sortino Ratio**     | **1.325546**  | **0.909671**  |
| **Max Drawdown**      | **–0.322658** | **–0.339250** |
| **Treynor Ratio**     | **0.199161**  | **0.128137**  |
| **Information Ratio** | **0.634019**  | **NaN**       |
| **M² (Modigliani)**   | **0.173789**  | **0.128169**  |

Intepretation:
Higher Returns With Similar Volatility:
The portfolio generated 18.62% annual return, outperforming the benchmark’s 12.82% by +5.8%, while maintaining similar volatility (18.59% vs 17.35%).

Superior Risk-Adjusted Performance:
Sharpe (1.00 vs 0.74) and Sortino (1.33 vs 0.91) ratios show that the portfolio achieved better returns per unit of both total and downside risk.

More Efficient Market Exposure:
With a Treynor ratio of 0.199 compared to the benchmark’s 0.128, the portfolio delivered higher return per unit of systematic (beta) risk.

Consistent Benchmark Outperformance:
The portfolio holds a positive Information Ratio of 0.634, reflecting consistent excess returns, while a higher M² (17.38% vs 12.82%) confirms superior risk-adjusted performance even after scaling volatility.

Techstack:Numpy,Pandas,Matplotlib,Yfinance.

Future Enhancements:
Implement dynamic allocation strategies (risk parity, mean-variance optimization).
Add multi-factor risk decomposition (market, sector, style factors).
Incorporate Monte Carlo simulations for stress testing and scenario analysis.
Build an interactive Streamlit dashboard for live portfolio tracking.
Support multi-portfolio comparison and risk budgeting analysis.

Note: The portfolio’s volatility aligns closely with the benchmark because all three assets—AAPL, JPM, and PG—are highly correlated S&P 500 constituents with similar exposure to market-wide systematic factors. As a result, the diversification benefit is modest, keeping annualized volatility within ~1% of benchmark levels.


