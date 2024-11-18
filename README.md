# Analysis of Economic Indicators and Monetary Policy on Markets

## Table of Contents

[Overview](#overview)

[Data Analysis](#data-analysis)

[The Team](#the-team)

## Project Overiew

### Overview

This project aims to measure the impact of economic indicators and monetary policy on the market. We examined monthly financial data, focusing primarily on the **S&P 500 index**, **treasury bond rates**, and **gold prices** to understand historical trends and understand how the markets may move in the near future. The project provides insights that could aid in strategic decision-making for financial analysts, investors, and policymakers by employing time series analysis and forecasting models.

### Questions we aim to answer

1. **What were the trends in the S&P 500, treasury bonds, and gold prices from 2007 to the present?**
2. **What is the correlation between FedFund rates and SNP500, 10-year Treasuries, Gold, Unemployment, and inflation?**
3. **Predict future Inflation Rates and Unemployment rates to inform investment decisions.**

### Usage and installation instructions

1. Install Dependencies. Make sure all required libraries are installed.

    pip install pandas prophet matplotlib
    #Import the required libraries and dependencies
    import pandas as pd
    import datetime as dt
    from prophet import Prophet
    import pandas as pd
    import datetime as dt
    from prophet import Prophet
    import yfinance as yf
    import matplotlib.pyplot as plt
    import numpy as np
    from scipy.signal import correlate
    from datetime import date

1. Read in the following CSV files: 
SNP500, FEDFUNDS, bls-monthly-unemployment, 10-Year Treasury, GoldPricesMonthly, inflation_rate_US

1. Run the Notebook.
   Open the notebook in Jupyter Notebook or Jupyter Lab and run each cell sequentially.

1. Data cleaning
Each data set is edited to bring the date in the index column and retain only 1 column showing the data of interest.

1. Concatenate
Concatenate all the data frames into a single data frame that includes all the data from 2007 to 2024 monthly.

1. Run correlations matrix and visualizations to observe the relationships between the data

1. Model Training and Forecasting:
The notebook will train the model using the input data and generate forecasts.
Show forecasting trends for Unemployment and Inflation.

Files:
 monthly_analysis.ipynb: The main notebook for performing monthly time series analysis and forecasting.


## Data Analysis

### Business Understanding

This project examines the movements of the S&P 500, 10-Year Treasury and Gold Prices based on Fed Monetary policy, Inflation and Unemployment data. By understanding these relationships, we hope to inform potential investment decisions in 2025.

### Data Understanding

This project leverages a comprehensive dataset containing several economic and financial indicators that collectively offer a multifaceted view of the U.S. market dynamics from 2007 to 2024. Key datasets include:

#### 1. S&P 500 Index

  This index represents the stock performance of 500 leading companies in the U.S., serving as a barometer for the overall health of the U.S. economy. The S&P 500 is essential for understanding market trends and investor sentiment.

#### 2. Treasury Bond Rates

  Data on ten-year Treasury bond yields provides insights into long-term government debt trends. Treasury yields often reflect investor confidence in the market and influence both short-term and long-term interest rates, making them valuable for evaluating financial conditions and market stability.

#### 3. Gold Prices

  Gold is traditionally seen as a safe haven asset, and its price movements often reflect investor sentiment during economic uncertainty. Analyzing gold prices alongside other assets helps us understand how investors react to inflationary pressures and financial risks.

#### 4. Inflation Indicators (Core US Inflation)

  The Consumer Price Index (CPI) measures inflation by tracking changes in the prices of goods and services, while interest rate data reflects the Federal Reserve's monetary policies. These indicators reveal how inflation and policy decisions affect consumer purchasing power and market conditions.

#### 5. Employment Metrics (Unemployment and Labor Force Participation Rates)

  Employment data includes the unemployment rate and the civilian labor force participation rate, which indicate the health of the labor market and the level of economic engagement. These metrics help gauge productivity, labor market tightness, and economic stability.

Each dataset is resampled to a quarterly basis to smooth monthly volatility and uncover long-term trends. This aggregation supports the project’s goal of identifying patterns, correlations, and predictive trends between the stock market and macroeconomic indicators, making it possible to anticipate the S&P 500's future movements.
By studying the relationships among these datasets, the project aims to reveal how economic indicators and policy shifts influence the market. Insights from this analysis can aid financial analysts, investors, and policymakers in making informed decisions based on historical trends and anticipated changes in economic conditions.

### Data Sources

S&P 500 (s&p index) - [YFinance](https://pypi.org/project/yfinance/)

10 Year US Treasuries - [YFinance](https://pypi.org/project/yfinance/)

Fed Interest Rates -  [Fed Reserve Data Download](https://www.federalreserve.gov/datadownload/)

Inflation (US Core inflation) - [Trading Economics](https://data.tradingeconomics.com)

Unemployment - [BLS Unemployment](https://www.bls.gov/data/#unemployment)

Gold - (Gold Futures) - - [Trading Economics](https://data.tradingeconomics.com)

### Analysis


@TO-DO Add correlation matrix image

@TO-DO S&P + unemployment charts

Looking at the relationship between the SNP and Unemployment, there is some inverse correlation (0.57). It is clear how a drop in unemployment post-financial crisis coincided with a rise in the stock market.

@TO-DO FedRate + unemployment chart

@TO-DO FedRate + unemployment conclusions

@TO-DO TBC charts and conclusions

## The Team

[GIBueno25](https://github.com/GIBueno25)

[rgoldstein24](https://github.com/rgoldstein24)

[tamfree](https://github.com/tamfree)

[ttsai19](https://github.com/ttsai19)

[yiannisp1822](https://github.com/yiannisp1822)
