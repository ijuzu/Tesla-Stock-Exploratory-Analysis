# Tesla Stock Exploratory Analysis
Dataset source: https://www.kaggle.com/datasets/adilshamim8/tesla-stock-price-history

# Introduction 


This dataset, originally sourced from Yahoo Finance, provides a history of Tesla stock prices from 2010 to 2025, with information on daily opening and closing prices, highest and lowest prices, and total trading volume.  

I used the dataset to perform some exploratory data analysis and visualize trends on ![Tableau](https://public.tableau.com/app/profile/ijuzu/vizzes)

First, I calculated daily average price change (between market open and close) and spike days to create monthly, quarterly, and yearly summary tables. "Spike days" refer to trading days in which Tesla's stock price moved more than ±5% between the market open and close. 

# Yearly Summary Table
![Tesla Stock Price - Yearly Summary](https://github.com/ijuzu/Tesla-Stock-Exploratory-Analysis/blob/main/Yearly%20Summary%20Table.PNG)

Based on this, I was interested in taking a closer look into which months/quarters had higher numbers of spike days. I used Tableau to visualize the number of "Spike days" per quarter: 

# Visualization of Spike Days Per Quarter
![Visualization of "Spike Days" Per Quarter](https://github.com/ijuzu/Tesla-Stock-Exploratory-Analysis/blob/main/Visualization%20of%20Quarterly%20Spikes.png)

It looks like 2020 and 2022 had the highest numbers of spike days, so I investigated a bit further into why: 

