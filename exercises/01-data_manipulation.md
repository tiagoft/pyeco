# Exercises – yfinance & Downloading Financial Data

## Part 1: Downloading & Plotting Financial Data

1. **Recall:** What is the purpose of the `yfinance` library? What type of object does `yf.download()` return?

2. **Recall:** What is the difference between `"Close"` and `"Adj Close"` in downloaded financial data? Why is one generally preferred for return calculations?

3. **Understand (Output Prediction):** What does the following code produce? Describe the structure (index and columns) of `data`.

   ```python
   import yfinance as yf
   data = yf.download("AAPL", period="1y")
   print(data.head())

4. **Analyse:** What error occurs if we try to plot a column that does not exist (e.g., df["Price"])? Why does this error occur? Identify the specific exception type.

5. **Application:** Download 5 years of daily adjusted close data for AAPL and a very low-priced stock (for example, SIRI). Normalize both price series so they start at 1 (divide each data series by its first value). Plot both normalized series on the same graph. Based on the graph, determine which stock would have been more profitable under a buy-and-hold strategy over the period. Explain why comparing raw price levels (without normalization) can be misleading when evaluating profitability.

6. **Solve a problem:** Write a script that downloads 5 years of a given set of tickers (choose 10 that you like), shows in a graph which stock would have been more profitable under a buy-and-hold strategy over the period, and displays which one would be this more profitable stock.

