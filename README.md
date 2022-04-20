# 📈 Optimizing A Portfolio
### Course: Python for Data Analysis II
### Task:
Perform a basic exploratory analysis of some historical financial data and decide the best investment strategy.
1. **Load the data and rearrange it as a pandas DataFrame with the following structure**:
  * One column per stock and concept: Open, High, Low, Close, Volume
  * Date as index (properly parsed)
  * Rows sorted by date, ascending
Be ready for dealing with errors in the names and some missing values.

2. **Visualize the data as follows**:
* Create a 2x2 grid of plots in which you plot the "Open" in green and "Close" in red for each stock.
* Repeat the 2x2 grid but resampling with the weekly average of "Open" and "Close".
* Add meaningful visualizations of your choice.


3. **Create a function that calculates the Return of Investment (ROI)**. Let's suppose you buy one stock one day, you hold it for N days (lookback period) and after N days you sell it. Create a function in Python that receives as parameters the following:
* lookback: the number of days you hold the stock
* name: the name of the stock, using the "Close" value of the stock
* data: the dataframe with the stock data.

4. **Apply the ROI function to the portfolio**. Create as many ROI columns as different stocks you have in the portfolio and plot them, representing for each stock:
* ROI after holding the stock for 365 days (red, dashed line)
* ROI after holding the stock for 180 days (blue, dotted line)
* ROI after holding the stock for 90 days (green, solid line)

5. The average ROI is a single number that comes from computing the overall mean of the ROI over the whole period of the series. **Given these two portfolios, which one has the best average ROI, with a lookback of 365 days?** 
* *Portfolio 1: AAPL 40%, GOOG 30%, MSFT 20%, AMZN 10%*
* *Portfolio 2:AAPL 30%, GOOG 20%, MSFT 10%, AMZN 40%*.

6. **Find a better combination in your portfolio**. The new combination should beat the best portfolio that you found in the previous exercise.
