# Apple-vs-microsoft-strategy
# Apple vs Microsoft: Moving Average Strategy Backtest

## Question
Would a moving average crossover strategy have beaten simply buying and holding Apple and Microsoft between 2020 and 2024?

## Method
- Downloaded daily price data using Python (`yfinance`)
- Built a 20/100-day moving average crossover signal
- Traded the day after each signal to avoid look-ahead bias
- Compared total return, maximum drawdown and Sharpe ratio against buy-and-hold
- Tested three window pairs (10/50, 20/100, 50/200) for robustness

## Key findings
- The strategy underperformed buy-and-hold on both stocks
- It did not reliably reduce risk
- No window setting beat buy-and-hold

| 20/100 window | Apple | Microsoft |
|---|---|---|
| Buy & hold return | 163.2% | 143.0% |
| Strategy return | 70.7% | 79.7% |

## Limitations
No transaction costs, only two stocks, a single bull-market period, and a warm-up period that disadvantages longer windows.

## Tools
Python, pandas, matplotlib, yfinance, Jupyter

## Files
`apple_vs_microsoft.ipynb` contains the full analysis with charts and commentary.
