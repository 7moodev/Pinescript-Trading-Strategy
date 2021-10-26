# Pinescript-Trading-Strategy
A compilation of financial indicators that I wrote in pinescript.

The first script plots VWAPs (volume weighted average price) that are anchored at the start of every day, week, month, and year.
It also plots the VWAP of the previous day/week/month/year, plots rolling 7-day and 30-day VWAPs, and plots simple moving averages.

The second script plots the z-score of price in relation to the 7-day vwap (voume weighted average price over the last 7 days).
That is, it tells you how many sigmas price is distanced from where the average buyer or seller has traded over the last 7 days.
It converts this into bar format, showing the z-score high, low, open, and close for each bar.

TradingView only allows a lookback of 10000 bars, so the sript uses "securities" to maximize workable data.
This works by running calculations on the minimum bar timeframe that captures the necessary data in as close to 10000 bars as possible.

The scripts are useful in a mean reversion and momentum based trading strategy. 
