# Exploratory Analysis of Tesla Stock Data
Dataset source: https://www.kaggle.com/datasets/adilshamim8/tesla-stock-price-history

# Introduction 
This dataset, originally sourced from Yahoo Finance, provides a history of Tesla stock prices from 2010 to 2025, with information on daily opening and closing prices, highest and lowest prices, and total trading volume.  

I used the dataset to perform some exploratory data analysis and visualize trends on Tableau. The links to each Tableau graph are inlcluded for easier visualization and interaction. 

# Data Exploration
I first verified that the data was clean (the Kaggle description noted that it had already been cleaned) and that there were no discepancies in the ways the data was formatted. 
I then expolored general trends in the data, noting where there was a large volume traded or where the price drastically changed during the day or between days. 

To investigate these patterns further, I calculated the daily average price change (between market open and close) and identified "spike days" to create monthly, quarterly, and yearly summary tables. "Spike days" refer to trading days in which Tesla's stock price moved more than ±5% between the market open and close. 

# Yearly Summary Table
![Tesla Stock Price - Yearly Summary](https://github.com/ijuzu/Tesla-Stock-Exploratory-Analysis/blob/main/Yearly%20Summary%20Table.PNG)

I also looked at the volume of Tesla stock traded by month: 
# ![Monthly Volume of Tesla Stock Traded]([https://public.tableau.com/app/profile/ijuzu/viz/MonthlyVolumeofTeslaStockTraded2010-2025/MontlyVolume](https://public.tableau.com/views/MonthlyVolumeofTeslaStockTraded2010-2025/MontlyVolume?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link))
![Monthly Volume of Tesla Stock Traded](https://github.com/ijuzu/Tesla-Stock-Exploratory-Analysis/blob/main/Montly%20Trading%20Volume.png)

Based on this, I was interested in taking a closer look into which months/quarters had higher numbers of spike days. I used Tableau to visualize the number of "Spike days" per quarter: 

# ![Visualization of Spike Days Per Quarter](https://public.tableau.com/views/TeslaSpikeDaysByQuarter2010-2025/QuarterlySummary?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)
![Visualization of "Spike Days" Per Quarter](https://github.com/ijuzu/Tesla-Stock-Exploratory-Analysis/blob/main/Visualization%20of%20Quarterly%20Spikes.png)



