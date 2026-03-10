# Simple Portfolio Optimizer

This project uses **Modern Portfolio Theory** to find the best stock allocations from the S&P 500. I used this code for my MPT presentation during APF - UJ Financial Mathematics Society science trip.

## How it works
1. Scrapes S&P 500 tickers from Wikipedia.
2. Downloads historical price data via Yahoo Finance.
3. Runs a Monte Carlo simulation to find the portfolio with the highest **Sharpe Ratio** (best risk-adjusted return).

## Downsides
1. Classic MPT has a lot of drawbacks, such as: const. volatility and correlations, assuming normal distribution of returns.
2. In my optimizer I had to skim down to 50 top performing stocks in the S&P 500 in order for the simulation to run.
3. My model assumes no short selling, transaction costs etc.
4. Wikipedia sometimes changes the format of the site, so the dataframe index may vary.

## Setup
1. Install requirements: `pip install -r requirements.txt`

2. Run the tool: `python optimizer.py`

