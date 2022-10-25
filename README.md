# Green_Stock_Analysis_with_Matplotlib

Personal Project: Using Python and Matplotlib to produce a comprehensive data analysis on three energy-producer companies for September 2022. This analysis showcases the performance of each respective company's stock: Ameresco (AMRC), ON Semiconductor Corp (ON), and Stem,Inc. (STEM). Data visualizations are created from this stock analysis to help investors or traders make buying or selling decisions, thereby gaining an edge in the markets.

To put in simply, this analysis provides a quick and easy way to pull live and historical market data to compare different key indicators in a clean plot format. The code is customizable and buildable to one's desired set of stock tickers for comparison. 

Besides delivering financial news and reports, Yahoo Finance also provides current and historical stock data that analysts can extract via Pythonic code and perform analyses directly in their coding environments. Over a dozen data visualizations are created for this stock analysis by manipulating different stock metrics i.e. daily percentage change, cumulative return.

### Ameresco
is a renewable energy and energy efficiency company. Ameresco's portfolio consists of asset sustainability, renewable energy solutions, and infrastructure upgrades serving clients in North America and in Europe. Ameresco's project span from federal governemnt buildings, airports to hospitals and schools/ Ameresco focuses on building energy infrastructure and development. Ameresco also helps customers with financial operating solutions for establishing energy efficiency and renewable energy infrastructure.
* AMRC stood out to me as a company to invest in because of its strong energy sales in the past year, making it a top-performing stock in the energy sector. Sales soared 111% last quarter and its stock continues to rise.

### Onsemi 
is a leading semiconductor manufacturer that has achieved success in several technologies and markets. Rebranded as onsemi, the company has been rated as Barron’s 100 “Most Sustainable Companies” for four years in a row and in 2020, onsemi was named to Dow Jones Sustainability Index for the third year in a row.
* Onsemi has been accelerating change in megatrends such as vehicle electrification and safety, sustainable energy grids, industrial automation, and 5G and cloud infrastructure. It's projected towards $2.085 billion revenue by the end of 2022.

### Stem
provides clean energy solutions with "clean energy intelligence". Stem's AI-driven enterprise software platform, Athena, enables organizations to deploy and monoteizse utility scale systems. The majority of Stem's clients are mid-sized commercial and industrial businesses, including Fortune 500 companies, and utilies and independent power producers that are seeking ways to save on energy to meet their ESG goals and make a positive impact on the environment. Stem focuses on maximizing ROI by demonstrating the value of renewable assets with energy storage. 
* Stem stood out to me as a company I'd want to invest in because of its long-term software contracts and because it targets a market growing 25x to $1.2 trillion by 2050. 



### Tools:

Jupyter Notebook

### Language:

Python

### Libraries:

matplotlib.pyplot as plt, pandas, hvplot.pandas, pandas_datareader, numpy, datetime, yfinance as yf, scattermatrix, warnings, mplcyberpunk

### Database: N/A

### Dataset:

All financial data is extracted in code from Yahoo Finance via yfinance library (Python). 


# Data Extracting with Python

## Extracting data via web.DataReader

### Established date range of 09/15/21 to 09/15/22 for stock analyses. Pandas' datareader function is used to pull data from Yahoo.

<img src="https://github.com/katmarcin/Green_Stock_Analysis_with_Matplotlib/blob/0f56ed7087b80cf68a06abc3c4d760ce1f0fa3f9/images/extract.jpg" />

## Method 2: Extracting data via yf.Ticker module and history method

### Alternative method of extracting data 

<img src="https://github.com/katmarcin/Green_Stock_Analysis_with_Matplotlib/blob/0f56ed7087b80cf68a06abc3c4d760ce1f0fa3f9/images/extract_2.jpg" />


# Data Mining and Visual Representation of Data via Python

## Stock Open Prices
<img src="https://github.com/katmarcin/Green_Stock_Analysis_with_Matplotlib/blob/0f56ed7087b80cf68a06abc3c4d760ce1f0fa3f9/images/stock_open.jpg" />

## Stock Close Prices
<img src="https://github.com/katmarcin/Green_Stock_Analysis_with_Matplotlib/blob/0f56ed7087b80cf68a06abc3c4d760ce1f0fa3f9/images/stock_close.jpg" />

## Stock Volume

### Volume is used to measure the relative significance of a market move. The higher the volume during a price move, the more significant the move. Up volume indicates bullish trading and down volume indicates bearish trading.

<img src="https://github.com/katmarcin/Green_Stock_Analysis_with_Matplotlib/blob/0f56ed7087b80cf68a06abc3c4d760ce1f0fa3f9/images/volume.jpg" />

## Total Stock Traded 

### Total number of stocks traded over a period of time. When prices fall with the stock volume going up, it indicates that more investors are selling that particular stock. If the prices increases with the stock volume going down, more investors are buying the stock. 

<img src="https://github.com/katmarcin/Green_Stock_Analysis_with_Matplotlib/blob/0f56ed7087b80cf68a06abc3c4d760ce1f0fa3f9/images/tt.jpg" />

## Argmax

### The pandas' argmax function returns the index of the greatest number in the indicated row or column. Axis=0 is used to indicate the column and axis=1 is used to indicate the row. Pandas' iloc function is used to return the argmax index's row with all its corresponding information from the dataset. These dates produced below can be used to verify the graphs developed in the previous code.

<img src="https://github.com/katmarcin/Green_Stock_Analysis_with_Matplotlib/blob/0f56ed7087b80cf68a06abc3c4d760ce1f0fa3f9/images/argmax.jpg" />


## Moving Averages

### Moving average or rolling average is used as a technical analysis tool to smooth out price data. It's a fantastic method for eliminating noise that regular line graphs of stock data characteristically produce, especially when examining open and close prices. In pandas, the rolling function is applied to calculate the moving average of a series of observations (window). Mean is calculated using the mean function on the object of window obtained.

### Profitable trades require knowing the right times to make an entry and exit on a particular stock. Entry points indicate the price point that is appropriate for investing and the exit point is the ideal point to sell. Moving averages, among other technical indicators such as bollinger bands and MACD are used to identify these points and predict how an asset's price might move.  As long as the 50-day moving average of a stock price remains above the 200-day moving average, the stock is generally thought to be in a bullish trend. '

### As long as the 50-day moving average of a stock price remains above a 200-day moving average, the stock is generally thought to be in a bullish trend.

A short window (50) and long window (100) are used to compare the moving average outputs.

<img src="https://github.com/katmarcin/Green_Stock_Analysis_with_Matplotlib/blob/0f56ed7087b80cf68a06abc3c4d760ce1f0fa3f9/images/movingav.jpg" />

## Moving Averages - AMRC Plot
<img src="https://github.com/katmarcin/Green_Stock_Analysis_with_Matplotlib/blob/0f56ed7087b80cf68a06abc3c4d760ce1f0fa3f9/images/movingav_plot.jpg" />

### AMRC's 50 day moving average (pink line) follow a general downward trend for this past year with an upward tick for the month of September.

## Moving Averages - ON Plot
<img src="https://github.com/katmarcin/Green_Stock_Analysis_with_Matplotlib/blob/0f56ed7087b80cf68a06abc3c4d760ce1f0fa3f9/images/on_movingav.jpg" />

### ON's 50 day moving average (blue line) follow a general upward trend for this past year with a strong upward tick for the months of August and September. What's interesting to note in this graph and what makes it stand out from the other stocks in the comparison between MA50 and MA100's (yellow) line. At the interesection point between MA50 and MA100, we see both lines begin to grow strongly in opposite directions. Thus, it's important to examine both windows to solidify asset predictions.

## Moving Averages - STEM Plot
<img src="https://github.com/katmarcin/Green_Stock_Analysis_with_Matplotlib/blob/0f56ed7087b80cf68a06abc3c4d760ce1f0fa3f9/images/stem_movingav.jpg" />

### STEM's 50 day moving average (blue line) follow a general downward trend for this past year with a quick upward tick for the month of September.


## Method 2: Moving Average Visualization with HVPlot package

### The benefit to using the hvplot package for plotting moving averages is the ability to produce an interactive map. With this map, we are able to scroll over the points that indicate entry/exit positions over the total portfolio value for the investment. Each point is able to indicate the date and the porfolio total at that position. 

<img src="https://github.com/katmarcin/Green_Stock_Analysis_with_Matplotlib/blob/0f56ed7087b80cf68a06abc3c4d760ce1f0fa3f9/images/movingav_hvplot.jpg" />

### Although more interactive than the previous graph, the hvplot fails to produce an aesthetically-pleasing and easily customizable design that the previous graph produces.

# Daily Percentage Change

### Daily percentage change is a technical analysis tool used to measure volatility (distribution). DPC is the percentage change in a value of a stock over a single trading day. The larger the value (positive or negative), the more volatile the stock is. Pandas' shift function is used to calculate this.

### 2-3% (or 0.02 / 0.03 is considered high volatility, a.k.a more risk)

### Formula for calculating DPC which will be used in code (excluding dividends):  rt = Pt/Pt-1 -1

## Daily Percentage Change - AMRC
<img src="https://github.com/katmarcin/Green_Stock_Analysis_with_Matplotlib/blob/0f56ed7087b80cf68a06abc3c4d760ce1f0fa3f9/images/amrc_dpc.jpg" />

## Daily Percentage Change - Combined Dataframe
<img src="https://github.com/katmarcin/Green_Stock_Analysis_with_Matplotlib/blob/0f56ed7087b80cf68a06abc3c4d760ce1f0fa3f9/images/dcp.jpg" />

## Method 2: Daily Percentage Change using pct_change() formula

### Rather than introducing the DPC formula into the code, an alternative calculation would be to use the pandas' pct_change function. This function is used to get the percentage change between the current and prior element. In Method 2, I created new dataframes from the 'Close' column of each stock so I can apply this function. Once concatenated and renamed, the table produces a neat representation of each stock's daily return.

<img src="https://github.com/katmarcin/Green_Stock_Analysis_with_Matplotlib/blob/0f56ed7087b80cf68a06abc3c4d760ce1f0fa3f9/images/dcp_2.jpg" />

## KDE Plot 

### Kernel density estimate is a normalized method for visualizing the distribution of observations in a dataset. The KDE is calculated by weighing the distances of all the data points seen for each point on the line graph. 

<img src="https://github.com/katmarcin/Green_Stock_Analysis_with_Matplotlib/blob/0f56ed7087b80cf68a06abc3c4d760ce1f0fa3f9/images/dcp_kdeplot.jpg" />

## Histogram

### A bin size of 50 is established for this histogram, which highlights major distribution features.

<img src="https://github.com/katmarcin/Green_Stock_Analysis_with_Matplotlib/blob/0f56ed7087b80cf68a06abc3c4d760ce1f0fa3f9/images/dcp_hist.jpg" />

### STEM generally has a larger distribution in its daily percentage change in comparison to AMRC and ON. Tight distributions indicate low volatility and wider distributions indicate higher volatility. In this scenario, STEM is riskier than both AMRC and ON which have relatively tight distributions.

## Boxplot

### Introduced a boxplot to examine any skewness and outliers the stock data may present.

<img src="https://github.com/katmarcin/Green_Stock_Analysis_with_Matplotlib/blob/0f56ed7087b80cf68a06abc3c4d760ce1f0fa3f9/images/dcp_box.jpg" />

### STEM has a greater range and abundance of outliers.


## Present: For-loop and pct_change (Formula for obtaining returns from present date to that of previous year)

### This entire analysis focuses on retroactive data for prediction purposes. It analyzes data from 09/15/2022 to the year prior. However, if we wanted to calculate daily percentage change for the present date down to the year prior, we could apply a for-loop and the pct_change function. This method closely resembles the previous example. By creating a list which is itemized by each stock, we can loop through each closing price with pct_change() applied to it. In doing so, we can append each DPC onto our list from the current date and all the way back to that date of the previous year. 

### Combine close and percent change in formula for daily return 
<img src="https://github.com/katmarcin/Green_Stock_Analysis_with_Matplotlib/blob/0f56ed7087b80cf68a06abc3c4d760ce1f0fa3f9/images/present.jpg" />


# Cumulative Return

### Cumulative return is the total change in the investment price over a set time.

### Formula: it = (1+rt)it-1. The cumprod function can be applied onto a dataframe to return the cumulative product. These cumulative return graphs were modified in code with the subplots functions to create a readable and comparable display.

<img src="https://github.com/katmarcin/Green_Stock_Analysis_with_Matplotlib/blob/0f56ed7087b80cf68a06abc3c4d760ce1f0fa3f9/images/creturn_df.jpg" />

### The subplots functions can be used to compare graphs beside each other
<img src="https://github.com/katmarcin/Green_Stock_Analysis_with_Matplotlib/blob/0f56ed7087b80cf68a06abc3c4d760ce1f0fa3f9/images/subplots.jpg" />

## Portfolio example: AMRC

### Initial capital of 100,000 with a share size of 500. THe cumsum function is used to calculated cumulative return on the ARMC stock.

<img src="https://github.com/katmarcin/Green_Stock_Analysis_with_Matplotlib/blob/0f56ed7087b80cf68a06abc3c4d760ce1f0fa3f9/images/portfolio.jpg" />

### Cumulative Return Portfolio Plot

<img src="https://github.com/katmarcin/Green_Stock_Analysis_with_Matplotlib/blob/0f56ed7087b80cf68a06abc3c4d760ce1f0fa3f9/images/cumulative_portf.jpg" />

## Correlation and scatter matrix on 'Open' data

<img src="https://github.com/katmarcin/Green_Stock_Analysis_with_Matplotlib/blob/0f56ed7087b80cf68a06abc3c4d760ce1f0fa3f9/images/correlation.jpg" />

## Scatter plot

<img src="https://github.com/katmarcin/Green_Stock_Analysis_with_Matplotlib/blob/0f56ed7087b80cf68a06abc3c4d760ce1f0fa3f9/images/scatter_plot.jpg" />

## Correlation table and exponentially weighted average plot

The EMA is a moving average that places a greater weight and significance on the most recent data points. This technical indicator is used to produce buy and sell signals based on crossovers and divergences from the historical average. A halflife, of number of observations, used in this graph is 21 days. A 21-day SMA is the sum of the closing prices for the past 21 trading days, divided by 21.
* The highest EMA is demonstrated by STEM, followed by AMRC, then ON. 

<img src="https://github.com/katmarcin/Green_Stock_Analysis_with_Matplotlib/blob/0f56ed7087b80cf68a06abc3c4d760ce1f0fa3f9/images/exp_weight_avg.jpg" />

## Exit position

<img src="https://github.com/katmarcin/Green_Stock_Analysis_with_Matplotlib/blob/0f56ed7087b80cf68a06abc3c4d760ce1f0fa3f9/images/exit_position.jpg" />


## Sharpe Ratios

Sharpe ratios are calcualted to compare how well an equity investment performs compared to the rate of return on a risk-free investment such a US treasury bonds. It evaluates the overall performance of a portolio or this scenario, a stock. SR is calculated by multiplying expected value by the difference between risk free return and asset return, then dividing it by the standard deviation of the asset excess return. An SR greater than 1 but less than 2 indicates good investment performance. A ratio < 1 is considered less than good.
* The highest sharpe ratio is observed in ON, followed by AMRC, then STEM.
* This formula has its limitations and can lead to unreliable results given that the standard deviation is held in the denominator. Because of this, the SR suggests equality volatility across the asset.

<img src="https://github.com/katmarcin/Green_Stock_Analysis_with_Matplotlib/blob/0f56ed7087b80cf68a06abc3c4d760ce1f0fa3f9/images/sharpe.jpg" />

## Backtest Formula

<img src="https://github.com/katmarcin/Green_Stock_Analysis_with_Matplotlib/blob/0f56ed7087b80cf68a06abc3c4d760ce1f0fa3f9/images/backtest_formula.jpg" />

## Backtest Table


## Final analysis



# Conclusion

In conclusion, I analyzed three stocks to understand performance by executing different technical indicators in code such as moving averages, cumulative return, daily percentage return, and sharpe ratios. The final backtest table puts all the pieces of the stock analysis together, allowing us to formulate concrete predictions on the best stock of the three to invest in. STEM presents investment risk; this is confirmed by the kernel desnity estimate plot, histogram, and boxplot produced for for the daily percentage change analyses. These are excellent visual representations of risk due to the fact that volatility is a measure of dispersion around the mean return. Wider distributions and outliers confirm greater risk. Both ON and STEM achieved their greatest cumulative return in the past two months, whereas ARMC's cumulative return is steadily decreasing. We can conclude from the exponentially moving average that there is strength is STEM's stock, however, all three stocks show a falling EMA. The final backtest table summarizes all the key technical indicators that play the largest roles in determing stocks performance: annual return, annual volatility, and sharpe ratio. For a safe long-term  investment, ON with it's high annual return, high sharpe ratio, and low volatility proves to be the best choice of the three stocks. Backtest table aside, STEM's stock is performing well with record highs, however this may not be a good time to buy in, per its cumulative return and expoentionally moving average (EMA). AMRC, on the other hand, would be an ideal stock to hold onto given its slightly high volatility, low annual return, and low sharpe ratio.
