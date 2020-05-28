# GoldPriceForecast
A python based gold forecast tool

# Project Overview

Project Domain: The project is in the finance and investment domain and attempts to use machine learning models to predict gold prices. 

Project Origin: Following the catastrophic impact of COVID pandemic on the global economy, central banks are pushing the limits of the monetary system for reviving the economy. U.S Fed alone attempts to pump in nearly $2 trillion dollar into the economic system so as to restore investor confidence and bring back animal appetite in the economy. Though such booster shoots are immensely needed in the short run, it might prep up long run inflation as more money chases a lesser number of goods. As per historical records, higher inflation translates to higher gold prices as investors scramble for assets that act as stores of value and safe haven. Origin of the project is to forecast gold return using key economic indicators.

Related Dataset: Project’s scope will involve historical gold prices, general economic indicators such as S&P 500, Nasdaq, Dollar index, volatility index, Crude Oil and most importantly real interest rate ie. US primary Interest rate Aka (Fed rate - inflation). The required data will be obtained from yahoo finance and Fred using API calls.  

Data range: Jan 2010 till May 2020

# Problem Statement
1. Identify trends in gold price movement compared to other economic indicators, especially, interest rate and inflation (Interest rates are taken as a proxy for central banks monetary action)
 
2. Forecast return on gold (22 days ahead using key technical and economic indicators

Discussion of expected solution: Create a model that trains using historical data of gold prices and other indicators and predict future price of gold and seek any investment opportunities. We will be using the latest PyCaret library that automatically splits the data into train and test and evaluates the model for its performance. The best model is taken for further forecasting.

# Metrics
Since it is a forecasting of returns and we are using pycaret library automatically splits the data into train and test and test and evaluates the effectiveness of the model. In this case, we are primarily concerned with the plot of residuals, MAE, Mean squared errors, RMSE and RSquare of the models. The model which give the best values in these metrics is taken for analysis and forecasting. 

# Files as part of git
The data is extracted from Yahoo financial and Fred API. 

For API: A valid API key is required for accessing FRED API. In the project we had the API key by using the free sign up link: http://research.stlouisfed.org/fred2/

Ticker List.xlsx: It contains the list of ticker symbols we are interested in for extracting data out of yahoo financials. The excel sheet is provided in the git repository.

GoldPriceProjection (Jupyter Notebook): The Jupyter notebook contains the python codes for execution along with markdown that explain each areas of the code in technical detail

Add a markdownversion of the notebook as well along with imagesas a part of visualization

# Library list
For data manipulation: numpy, pandas and datettime. 
For visualization: plotly and matplotlib are used. 
For api calls: yahoofinancial and fredapi
For Modelling: Pycaret - It is a open source machine learning library that makes modelling process efficient. The inovative library directly approches the problems involving modeling and commands highly on ease of use and speed of processing.  

# Link to the Blog post
https://medium.com/@ramnathkumar8/will-gold-still-glitter-using-python-based-machine-learning-to-forecast-gold-returns-b4197fdab7e9
