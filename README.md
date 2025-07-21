# Exploratory Analysis of Tesla Stock Data (2010-2025)
Dataset source: https://www.kaggle.com/datasets/adilshamim8/tesla-stock-price-history

Code: [Tesla Stock Exploratory Analysis](https://github.com/ijuzu/Tesla-Stock-Exploratory-Analysis/blob/main/Tesla_stock_data.csv)

# Introduction 
This dataset was downloaded from Kaggle and originally sourced from Yahoo Finance. It provides a history of Tesla stock prices starting from 2010, with information on daily opening and closing prices, highest and lowest prices, and total trading volume.  

I used this dataset to perform some exploratory data analysis and visualize trends on Tableau. This project is still in progress.

# Data Exploration
I first verified that the data was clean (the Kaggle description noted that it had already been cleaned, but I double checked for null values and duplicates) and that there were no discrepancies in the ways the data was formatted.
I then explored general trends in the data, noting where there was a large volume traded or where the price drastically changed during the day or between days. 

For example, I looked into the volume of Tesla stock traded by month along with the average daily percent change (percent change between market open and close). I was interested in seeing if there would be any correlation in average daily percent change and the volume traded.
## [Monthly Volume of Tesla Stock Traded and Average Percent Daily Change](https://public.tableau.com/views/MonthlyVolumeofTeslaStockTradedwithAverageDailyChange2010-2025/MontlyVolume?:language=en-US&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)
![Monthly Volume of Tesla Stock Traded With Average Percent Change](https://github.com/ijuzu/Tesla-Stock-Exploratory-Analysis/blob/main/Montly%20Volume%20With%20Average%20Percent%20Daily%20Change.png) 

I calculated monthly return (by using the closing values for the beginning and end of the month) and visualized this along with the volume traded:
## [Tesla Monthly Return and Volume Traded](https://public.tableau.com/views/TeslaMontlyReturnandVolumeTraded2010-2025/MonthlyReturnPercentage?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)
![Tesla Monthly Return and Volume Traded](https://github.com/ijuzu/Tesla-Stock-Exploratory-Analysis/blob/main/Tesla%20Monthly%20Return%20Percentage%20and%20Volume%20Traded.png)
The peak in May 2013 is particularly intriguing, where the monthly return percentage was 83.5 - the highest during this 15 year history. 

To investigate further, I identified "spike days" to create monthly, quarterly, and yearly summary tables. "Spike days" refer to trading days in which Tesla's stock price moved more than ±5% between the market open and close. 
## Yearly Summary Table
![Tesla Stock Price - Yearly Summary](https://github.com/ijuzu/Tesla-Stock-Exploratory-Analysis/blob/main/Yearly%20Summary%20Table.PNG)


I was interested in then taking a closer look into which months/quarters had higher numbers of spike days and visualized the number of "Spike days" per quarter.
## [Visualization of Spike Days Per Quarter](https://public.tableau.com/views/TeslaSpikeDaysByQuarter2010-2025/QuarterlySummary?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)
![Visualization of "Spike Days" Per Quarter](https://github.com/ijuzu/Tesla-Stock-Exploratory-Analysis/blob/main/Visualization%20of%20Quarterly%20Spikes.png)

I noticed that 2020 and 2022 had much higher numbers of spikes compared to any of the other years. Therefore, I took a closer look into both years. I first visualized the daily percent change along with the volume traded to see if there might be any interesting patterns, especially in Q1 and Q3 (2020) and Q1, Q2, and Q4 (2022) where there were the highest number of spike days. I chose to visualize these along with 2017, which was the year of fewest spike days (only 3 in total):

## [Tesla Stock: Volume Traded and Daily Percent Change in 2017](https://public.tableau.com/views/TeslaStockVolumeTradedandDailyPercentChangein2017/Sheet12?:language=en-US&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)
![Volume Traded and Daily Percent Change in 2017](https://github.com/ijuzu/Tesla-Stock-Exploratory-Analysis/blob/main/Tesla%20Stock%20-%20Volume%20Traded%20and%20Daily%20Percent%20Change%20in%202017.png)

## [Tesla Stock: Volume Traded and Daily Percent Change in 2020](https://public.tableau.com/views/TeslaStockVolumeTradedandDailyPercentChangein2020/Sheet9?:language=en-US&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)
![Volume Traded and Daily Percent Change in 2020](https://github.com/ijuzu/Tesla-Stock-Exploratory-Analysis/blob/main/Tesla%20Stock%20-%20Volume%20Traded%20and%20Daily%20Percent%20Change%20in%202020.png)

## [Tesla Stock: Volume Traded and Daily Percent Change in 2022](https://public.tableau.com/views/TeslaStockVolumeTradedandDailyPercentChangein2022/Sheet11?:language=en-US&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)
![Volume Traded and Daily Percent Change in 2022](https://github.com/ijuzu/Tesla-Stock-Exploratory-Analysis/blob/main/Tesla%20Stock%20Volume%20Traded%20and%20Daily%20Percent%20Change%20in%202022.png)

A few patterns stood out from these visualizations: 
* **Volatility was significantly higher in 2020 and 2022 compared to 2017.**
The daily percent change ranged from -5.79% to +5.70% in 2017, while in 2020 it ranged from -10.76% to +15.78%, and in 2022 from -11.96% to +14.33%.
* **Spikes in trading volume generally aligned with sharp price movements.**
 Local highs and lows in daily percent change aligned with peaks in volume traded, showing increased investor activity during these periods.
* **The quarters in 2020 and 2022 which saw the greatest "spike days" (±5% daily change) showed both increased volatility and trading activity.** For example, in Q1 2020, two major swings occurred:
  - February 3, 2020: Tesla stock rose by +15.78%
  - February 5, 2020: Tesla stock dropped by -10.76%
  
These changes correlated with the highest volume traded at 914 million shares on February 4th. I hypothesize that these specific changes were related to the uncertainty in the early days of the COVID-19 pandemic.



 




