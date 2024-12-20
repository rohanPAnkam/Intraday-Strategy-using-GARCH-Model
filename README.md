Intraday Strategy Using GARCH Model
- Using simulated daily data and intraday 5-min data.
- Load Daily and 5-minute data.
- Define function to fit GARCH model on the daily data and predict 1-day ahead volatility in a rolling window.
- Calculate prediction premium and form a daily signal from it.
- Merge with intraday data and calculate intraday indicators to form the intraday signal.
- Generate the position entry and hold until the end of the day.
- Calculate final strategy returns.

1. Load Simulated Daily and Simulated 5-minute data.
- We are loading both datasets, set the indexes and calculate daily log returns.

2. Define function to fit GARCH model and predict 1-day ahead volatility in a rolling window.
- We are first calculating the 6-month rolling variance and then we are creating a function in a 6-month rolling window to fit a garch model and predict the next day variance.

3. Calculate prediction premium and form a daily signal from it.
- We are calculating the prediction premium. And calculate its 6-month rolling standard deviation.
- From this we are creating our daily signal.

4. Merge with intraday data and calculate intraday indicators to form the intraday signal.
- Calculate all intraday indicators and intraday signal.

5. Generate the position entry and hold until the end of the day.

6. Calculate final strategy returns.
