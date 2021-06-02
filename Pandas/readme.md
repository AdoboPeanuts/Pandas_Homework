# Pandas

## Key Objectives:

```

# 1. Read in and wrangle returns data

# 2. Determine success of each portfolio

# 3. Choose and evaluate a custom portfolio


# Instructions

# Files:

Whale Analysis Starter Code

algo_returns.csv

otex_historical.csv

sp_tsx_history.csv

l_historical.csv

shop_historical.csv

whale_returns.csv

# Prepare the Data

First, read and clean several CSV files for analysis. The CSV files include whale portfolio returns, algorithmic trading portfolio returns, and S&P TSX 60 Index historical prices. Use the starter code to complete the following steps:

Use Pandas to read the following CSV files as a DataFrame. Be sure to convert the dates to a DateTimeIndex.

whale_returns.csv: Contains returns of some famous "whale" investors' portfolios.

algo_returns.csv: Contains returns from the in-house trading algorithms from Harold's company.

sp_tsx_history.csv: Contains historical closing prices of the S&P TSX 60 Index.

Detect and remove null values.

If any columns have dollar signs or characters other than numeric values, remove those characters and convert the data types as needed.

The whale portfolios and algorithmic portfolio CSV files contain daily returns, but the S&P TSX 60 CSV file contains closing prices. Convert the S&P TSX 60 closing prices to daily returns.

Join Whale Returns, Algorithmic Returns, and the S&P TSX 60 Returns into a single DataFrame with columns for each portfolio's returns.

returns-dataframe.png

# Conduct Quantitative Analysis

Analyze the data to see if any of the portfolios outperform the stock market (i.e., the S&P TSX 60).

## Performance Analysis

Calculate and plot daily returns of all portfolios.

Calculate and plot cumulative returns for all portfolios. Does any portfolio outperform the S&P TSX 60?

## Risk Analysis

Create a box plot for each of the returns.

Calculate the standard deviation for each portfolio.

Determine which portfolios are riskier than the S&P TSX 60

Calculate the Annualized Standard Deviation.

## Rolling Statistics

Calculate and plot the rolling standard deviation for all portfolios using a 21-day window.

Calculate and plot the correlation between each stock to determine which portfolios may mimick the S&P TSX 60.

Choose one portfolio, then calculate and plot the 60-day rolling beta for it and the S&P TSX 60.

## Rolling Statistics Challenge: Exponentially Weighted Average

An alternative method to calculate a rolling window is to take the exponentially weighted moving average. This is like a moving window average, but it assigns greater importance to more recent observations. Try calculating the ewm with a 21-day half-life.

# Sharpe Ratios
Investment managers and their institutional investors look at the return-to-risk ratio, not just the returns. After all, if you have two portfolios that each offer a 10% return, yet one is lower risk, you would invest in the lower-risk portfolio, right?

1 .Using the daily returns, calculate and visualize the Sharpe ratios using a bar plot.

2. Determine whether the algorithmic strategies outperform both the market (S&P TSX 60) and the whales portfolios.

# Create a Custom Portfolio

Harold is ecstatic that you were able to help him prove that the algorithmic trading portfolios are doing so well compared to the market and whales portfolios. However, now you are wondering whether you can choose your own portfolio that performs just as well as the algorithmic portfolios. Investigate by doing the following:

1. Visit Google Sheets and use the built-in Google Finance function to choose 3-5 stocks for your portfolio.

2. Download the data as CSV files and calculate the portfolio returns.

3 .Calculate the weighted returns for your portfolio, assuming equal number of shares per stock.

4. Add your portfolio returns to the DataFrame with the other portfolios.

5. Run the following analyses:

    Calculate the Annualized Standard Deviation.

    Calculate and plot rolling std with a 21-day window.

    Calculate and plot the correlation.

    Calculate and plot the 60-day rolling beta for your portfolio compared to the S&P 60 TSX.

    Calculate the Sharpe ratios and generate a bar plot.

6 How does your portfolio do?

```
