Objective
The objective is to develop an investment risk and performance analytics framework to evaluate an equal-weighted equity portfolio (AAPL, JPM, PG) relative to the S&P 500 benchmark, focusing on absolute returns, downside risk, drawdowns, and risk-adjusted performance. The objective is to assess portfolio efficiency, market sensitivity, and consistency of excess returns using industry-standard risk metrics applied in investment risk and portfolio oversight roles.

Process

Data Collection & Preprocessing:
Retrieved historical daily price data for AAPL, JPM, PG, and ^GSPC using yfinance.
Computed daily log returns, equal-weighted portfolio returns, and cumulative performance.

Portfolio Construction:
Constructed a static equal-weighted portfolio to isolate asset selection effects.
Used the S&P 500 as the market benchmark for relative risk and performance evaluation.

Risk & Performance Measurement
Calculated portfolio and benchmark metrics commonly used by investment risk teams, PM oversight, and performance attribution:
Sharpe Ratio (total risk-adjusted return).
Sortino Ratio (downside risk-adjusted return).
Maximum Drawdown (tail loss and capital impairment).
Treynor Ratio (systematic risk efficiency).
Information Ratio (consistency of active returns).
M² (Modigliani Risk-Adjusted Return) for volatility-scaled comparison.

Results

| **Metric**            | **Portfolio** | **Benchmark (S&P 500)** |
| --------------------- | ------------- | ----------------------- |
| **Annual Return**     | **0.186239**  | **0.128169**            |
| **Annual Volatility** | **0.18594**   | **0.17351**             |
| **Sharpe Ratio**      | **1.001606**  | **0.738684**            |
| **Sortino Ratio**     | **1.325546**  | **0.909671**            |
| **Max Drawdown**      | **–0.322658** | **–0.339250**           |
| **Treynor Ratio**     | **0.199161**  | **0.128137**            |
| **Information Ratio** | **0.634019**  | **NaN**                 |
| **M² (Modigliani)**   | **0.173789**  | **0.128169**            |



Interpretation

Higher Absolute Returns with Comparable Risk:
The portfolio generated an 18.6% annualized return, outperforming the benchmark by approximately +580 bps, while maintaining similar volatility. This indicates improved return efficiency without materially increasing total risk.

Superior Risk-Adjusted Performance:
Higher Sharpe (1.00 vs 0.74) and Sortino (1.33 vs 0.91) ratios demonstrate that the portfolio delivered stronger returns per unit of both total volatility and downside risk, aligning with investment risk performance objectives.

Efficient Systematic Risk Exposure:
A Treynor ratio of 0.199 versus 0.128 for the benchmark indicates more efficient compensation for market (beta) risk, suggesting effective equity exposure rather than excess leverage.

Consistent Active Outperformance:
A positive Information Ratio (0.63) confirms persistent excess returns relative to the benchmark, while the higher M² (17.38% vs 12.82%) validates superior performance after volatility normalization.

Tech Stack:Python, NumPy, Pandas, Matplotlib, Yfinance.

Future Enhancements
Implement dynamic allocation frameworks (risk parity, mean-variance optimization).
Add multi-factor risk decomposition (market, sector, style factors).
Incorporate Monte Carlo simulations for stress testing and tail-risk assessment.
Build an interactive Streamlit dashboard for real-time risk and performance monitoring.
Extend to multi-portfolio comparison and risk budgeting analysis.

Note on Volatility & Diversification:
Portfolio volatility closely tracks the benchmark because AAPL, JPM, and PG are large-cap S&P 500 constituents with high market correlation. As a result, diversification benefits are limited, keeping volatility within ~1% of benchmark levels despite asset-level diversification.

Key Insights:
Asset selection added meaningful alpha without increasing total or systematic risk.
Risk-adjusted metrics consistently favor the portfolio, indicating efficient risk taking.
Drawdown behavior is marginally better than the benchmark, supporting capital preservation objectives.
The framework demonstrates practical application of performance measurement, benchmark-relative risk, and portfolio efficiency analysis, directly relevant to investment risk and portfolio oversight roles.
