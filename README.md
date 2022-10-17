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
provides clean energy solutions with "clean energy intelligence. Stem's AI-driven enterprise software platform, Athena, enables organizations to deploy and monoteizse utility scale systems. The majority of Stem's clients are mid-sized commercial and industrial businesses, including Fortune 500 companies, and utilies and independent power producers that are seeking ways to save on energy to meet their ESG goals and make a positive impact on the environment. Stem focuses on maximizing ROI by demonstrating the value of renewable assets with energy storage. 
* Stem stood out to me as a company I'd want to invest in because of its long-term software contracts and because it targets a market growing 25x to $1.2 trillion by 2050. 



### Tools:

Jupyter Notebook

### Language:

Python

Libraries:

matplotlib.pyplot as plt, pandas, hvplot.pandas, pandas_datareader, numpy, datetime, yfinance as yf, scattermatrix, warnings, mplcyberpunk

Database: N/A

Dataset:

All financial data is extracted in code from Yahoo Finance via yfinance library (Python). 


# Data Extracting with Python

## Extracting data via web.DataReader

<img src="https://github.com/katmarcin/Green_Stock_Analysis_with_Matplotlib/blob/0f56ed7087b80cf68a06abc3c4d760ce1f0fa3f9/images/extract.jpg" />

## Method 2: Extracting data via yf.Ticker module and history method

<img src="https://github.com/katmarcin/Green_Stock_Analysis_with_Matplotlib/blob/0f56ed7087b80cf68a06abc3c4d760ce1f0fa3f9/images/extract_2.jpg" />


# Data Mining and Visual Representation of Data via Python

## Stock Open Prices
<img src="https://github.com/katmarcin/Green_Stock_Analysis_with_Matplotlib/blob/0f56ed7087b80cf68a06abc3c4d760ce1f0fa3f9/images/stock_open.jpg" />

## Stock Close Prices
<img src="https://github.com/katmarcin/Green_Stock_Analysis_with_Matplotlib/blob/0f56ed7087b80cf68a06abc3c4d760ce1f0fa3f9/images/stock_close.jpg" />

## Stock Volume
<img src="https://github.com/katmarcin/Green_Stock_Analysis_with_Matplotlib/blob/0f56ed7087b80cf68a06abc3c4d760ce1f0fa3f9/images/volume.jpg" />

## Total Stock Traded 
<img src="https://github.com/katmarcin/Green_Stock_Analysis_with_Matplotlib/blob/0f56ed7087b80cf68a06abc3c4d760ce1f0fa3f9/images/tt.jpg" />

## Argmax
<img src="https://github.com/katmarcin/Green_Stock_Analysis_with_Matplotlib/blob/0f56ed7087b80cf68a06abc3c4d760ce1f0fa3f9/images/argmax.jpg" />


## Moving Averages

<img src="https://github.com/katmarcin/Green_Stock_Analysis_with_Matplotlib/blob/0f56ed7087b80cf68a06abc3c4d760ce1f0fa3f9/images/movingav.jpg" />

## Moving Averages - AMRC Plot
<img src="https://github.com/katmarcin/Green_Stock_Analysis_with_Matplotlib/blob/0f56ed7087b80cf68a06abc3c4d760ce1f0fa3f9/images/movingav_plot.jpg" />

## Moving Averages - ON Plot
<img src="https://github.com/katmarcin/Green_Stock_Analysis_with_Matplotlib/blob/0f56ed7087b80cf68a06abc3c4d760ce1f0fa3f9/images/on_movingav.jpg" />

## Moving Averages - STEM Plot
<img src="https://github.com/katmarcin/Green_Stock_Analysis_with_Matplotlib/blob/0f56ed7087b80cf68a06abc3c4d760ce1f0fa3f9/images/stem_movingav.jpg" />

## Moving Average Visualization with HVPlot package
<img src="https://github.com/katmarcin/Green_Stock_Analysis_with_Matplotlib/blob/0f56ed7087b80cf68a06abc3c4d760ce1f0fa3f9/images/movingav_hvplot.jpg" />


# Daily Percentage Change

## Daily Percentage Change - AMRC
<img src="https://github.com/katmarcin/Green_Stock_Analysis_with_Matplotlib/blob/0f56ed7087b80cf68a06abc3c4d760ce1f0fa3f9/images/amrc_dpc.jpg" />

## Daily Percentage Change - Combined Dataframe
<img src="https://github.com/katmarcin/Green_Stock_Analysis_with_Matplotlib/blob/0f56ed7087b80cf68a06abc3c4d760ce1f0fa3f9/images/dcp.jpg" />

## Method 2: Daily Percentage Change using pct_change() formula
<img src="https://github.com/katmarcin/Green_Stock_Analysis_with_Matplotlib/blob/0f56ed7087b80cf68a06abc3c4d760ce1f0fa3f9/images/dcp_2.jpg" />

## KDE Plot 
<img src="https://github.com/katmarcin/Green_Stock_Analysis_with_Matplotlib/blob/0f56ed7087b80cf68a06abc3c4d760ce1f0fa3f9/images/dcp_kdeplot.jpg" />

## Historgram
<img src="https://github.com/katmarcin/Green_Stock_Analysis_with_Matplotlib/blob/0f56ed7087b80cf68a06abc3c4d760ce1f0fa3f9/images/dcp_hist.jpg" />

## Boxplot
<img src="https://github.com/katmarcin/Green_Stock_Analysis_with_Matplotlib/blob/0f56ed7087b80cf68a06abc3c4d760ce1f0fa3f9/images/dcp_box.jpg" />


## Present: For-loop and pct_change (Formula for obtaining returns from present date to that of previous year)
### Combine close and percent change in formula for daily return 
<img src="https://github.com/katmarcin/Green_Stock_Analysis_with_Matplotlib/blob/0f56ed7087b80cf68a06abc3c4d760ce1f0fa3f9/images/present.jpg" />


# Cumulative Return
<img src="https://github.com/katmarcin/Green_Stock_Analysis_with_Matplotlib/blob/0f56ed7087b80cf68a06abc3c4d760ce1f0fa3f9/images/creturn_df.jpg" />


<img src="https://github.com/katmarcin/Green_Stock_Analysis_with_Matplotlib/blob/0f56ed7087b80cf68a06abc3c4d760ce1f0fa3f9/images/subplots.jpg" />
<img src="https://github.com/katmarcin/Green_Stock_Analysis_with_Matplotlib/blob/0f56ed7087b80cf68a06abc3c4d760ce1f0fa3f9/images/portfolio.jpg" />
<img src="https://github.com/katmarcin/Green_Stock_Analysis_with_Matplotlib/blob/0f56ed7087b80cf68a06abc3c4d760ce1f0fa3f9/images/cumulative_portf.jpg" />
<img src="https://github.com/katmarcin/Green_Stock_Analysis_with_Matplotlib/blob/0f56ed7087b80cf68a06abc3c4d760ce1f0fa3f9/images/correlation.jpg" />
<img src="https://github.com/katmarcin/Green_Stock_Analysis_with_Matplotlib/blob/0f56ed7087b80cf68a06abc3c4d760ce1f0fa3f9/images/scatter_plot.jpg" />
<img src="https://github.com/katmarcin/Green_Stock_Analysis_with_Matplotlib/blob/0f56ed7087b80cf68a06abc3c4d760ce1f0fa3f9/images/exp_weight_avg.jpg" />


<img src="https://github.com/katmarcin/Green_Stock_Analysis_with_Matplotlib/blob/0f56ed7087b80cf68a06abc3c4d760ce1f0fa3f9/images/exit_position.jpg" />


<img src="https://github.com/katmarcin/Green_Stock_Analysis_with_Matplotlib/blob/0f56ed7087b80cf68a06abc3c4d760ce1f0fa3f9/images/sharpe.jpg" />

<img src="https://github.com/katmarcin/Green_Stock_Analysis_with_Matplotlib/blob/0f56ed7087b80cf68a06abc3c4d760ce1f0fa3f9/images/backtest_formula.jpg" />
<img src="https://github.com/katmarcin/Green_Stock_Analysis_with_Matplotlib/blob/0f56ed7087b80cf68a06abc3c4d760ce1f0fa3f9/images/bacltest_table.jpg" />
<img src="https://github.com/katmarcin/Green_Stock_Analysis_with_Matplotlib/blob/0f56ed7087b80cf68a06abc3c4d760ce1f0fa3f9/images/backtest_final.jpg" />



# Explanation of Visualization Techniques

# Conclusion






