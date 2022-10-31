# Stock Analysis
## Overview of Project
The purpose of this project is to collect the total daily volume and return for a list of 12 different stocks in the years 2017 and 2018. The analysis was originally based on a nested for loop that ran through each of the stock tickers 3 times; first to get the stock's return, and the next two iterations to gather the start and end price in the given year. While this method ultimately got the job done, it took a while to complete all the loops needed to pull all the necessary information. 
In order to make the analysis more flexible for the client, it needed to be refactored to run in less time. This goal was accomplished by changing the existing for loop to run only one time per stock ticker - pulling all three data points in one iteration instead of 3 iterations. This change succesfully decreased the run time.
## Results
The stock analysis for 2017 shows that 11 out of the 12 selected stocks had net positive returns between the start of 2017 and the end of the year. Many stocks outperformed the average return of the S&P500 of 8% by a factor of ___. The only stock that underperformed was 'TERP' with a -7.2% return. 

![stock_overview_2017.png](https://github.com/skyeryser/stock-analysis/blob/main/Resources/stock_overview_2017.png)

The original code for the 2017 analysis took ___ to run.

In 2018, it appears that the market climate shifted for the worse. The majority of the listed stocks ended the year at a lower price than they started the year. Even though the average trading volume for the stocks increased from 263,886,592 trades in 2017 to 275,503,183 trades in 2018, it looks like the majority of investors weren't holding their stocks for the entire year.

![stock_overview_2018.png](https://github.com/skyeryser/stock-analysis/blob/main/Resources/stock_overview_2018.png)

The original code for the 2018 analysis took ___ to run.


When refactored, the resulting analysis for 2017 and 2018 were identical to the original analysis, however; the run time for the analysis decreased. For the year 2017, the code took ___ seconds to run.

The refactored code took __ seconds to run for the year 2018.


## Summary
1. The first advantage of refactoring code is that the process of reviewing your work gives you the opportunity to understand what you've written and why it works. This gives you the chance to identify where the essential arguments are, versus lines of code that might not be needed for the algorithm to function. Once the code has been refactored and no longer has unnecessary information, it will likely run faster than it did in the original solution. This is where the second key advantage of refactoring code comes into play; it allows the code to be used on bigger sets of data, or potentially for different datasets. For example, the stocks data used in this project only included 12 stocks. Once refactored, the client could easily add a 13th stock to analyze, just by updating the ticker array and the number of iterations for the loop. The only real disadvantage of refactoring code is the additional time that is spent optimizing and reworking it.
2. 
