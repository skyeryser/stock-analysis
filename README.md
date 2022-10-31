# Stock Analysis
## Overview of Project
This project aims to collect the total daily volume and return for a list of twelve different stocks in the years 2017 and 2018. The analysis was based on a nested for loop that ran through each of the stock tickers three times, first to get the stock's return, while the following two iterations gathered the start and end price in the given year. While this method ultimately got the job done, it took a while to complete all the loops needed to pull all the necessary information. 
To make the analysis run faster for the client, the code needed to be refactored. This goal was accomplished by changing the existing for loop to run only once per stock ticker - pulling all three data points in one iteration instead of three iterations. This change successfully decreased the run time.
## Results
## The Initial Investigation
The stock analysis for 2017 shows that eleven of the twelve selected stocks had net positive returns between the start of 2017 and the end of the year. In addition, many stocks outperformed the average 8% annual return of the S&P 500 by well over 100%. The only security that underperformed in 2017 was 'TERP' with a -7.2% return. 

![stock_overview_2017.png](https://github.com/skyeryser/stock-analysis/blob/main/Resources/stock_overview_2017.png)

The original code for the 2017 analysis took 55623.93 seconds to run.

![VBA_Challenge_2017](https://github.com/skyeryser/stock-analysis/blob/main/Resources/VBA_Challeng_2017.png)

In 2018, the market climate shifted for the worse. Most of the listed stocks ended the year at a lower price than they started. Even though the average trading volume for the stocks increased from 263,886,592 trades in 2017 to 275,503,183 trades in 2018, it looks like the majority of investors were not holding their stocks for the entire year.

![stock_overview_2018.png](https://github.com/skyeryser/stock-analysis/blob/main/Resources/stock_overview_2018.png)

## The Refactored Analysis
The original code for the 2018 analysis took 41025.55 seconds to run.

![VBA_Challenge_2018.png](https://github.com/skyeryser/stock-analysis/blob/main/Resources/VBA_Challenge_2018.png)

When refactored, the resulting analysis for 2017 and 2018 was identical to the original investigation; however, the run time for the analysis decreased. For the year 2017, the code took .0703125 seconds to run.

![Refactored_VBA_Challenge_2017](https://github.com/skyeryser/stock-analysis/blob/main/Resources/Refactored_VBA_Challenge_2017.png)

The refactored code took .0703125 seconds to run for the year 2018.

![Refactored_VBA_2018.png](https://github.com/skyeryser/stock-analysis/blob/main/Resources/Refactored_VBA_Challenge_2018.png)

Ultimately, the exercise of refactoring the code resulted in the same conclusion as the original analysis, only now the client can see the result much faster than in the original analysis. 

## Summary
1. The first advantage of refactoring code is that reviewing your work lets you understand what you've written and why it works. This deep dive gives you a chance to identify where the essential arguments are versus lines of code that might not be necessary for the algorithm to function. Once the code has been refactored and no longer has unnecessary information, it will likely run faster than it did in the original solution. After the revision step, the second key advantage of refactoring code comes into play; it allows the code to be applied to expanded datasets or potentially to different datasets. The only real disadvantage of refactoring code is the additional time spent optimizing and reworking it.
2. For example, the stock data used in this project only included twelve stocks. Once refactored, the client could easily add a thirteenth stock to analyze by updating the ticker array and the number of iterations for the loop. Since the code is refactored to run faster than the original, the client wouldn't risk overdoing the run time for the stock analysis by adding another stock. The most significant disadvantage of refactoring the stock analysis code was the time and effort it takes for the developer to rewrite the code. For the client, refactoring the code is almost always more efficient and useful.
