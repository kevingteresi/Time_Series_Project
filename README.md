# Time_Series_Project
R Project to Demonstrate Time Series Forecasting on Tesla Stock Data


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Launch](#launch)
* [Screenshots](#screenshots)




## General Information
- This project was my final project for my Stats 474: Time Series class at Cal State East Bay.  Professor Eric Suess was my professor for this class, and he has given me permission to use this project as a demonstration of Time Series Forecasting.

Format of the Project:

"Find a monthly (or weekly) time series data set of interest to you that contains at least two time series to work with to make forecasts for the next 12 months.

Build the following models for at least two time series and use them to forecast the next 12 months.

1. Build a linear regression model using TSLM().
2. Build an appropriate exponential smoothing model.
3. Build an SARIMA model.
4. Build a neural network.

In your R Notebook show the the fitted values on a time plot and show your forecasts with errors."

- The description of the project is very loose and minimal.  The point of the project was to take the code and principals learned from class (and learned from the book "Forecasting: Principles and Practice") and apply them to stock data of my choosing.  I chose Tesla because I was fascinated with the current boom of stock once Tesla went public.  Elon Musk is a very fascinating man to me.


## Technologies Used

- R (4.0.3)
  - Tidyverse
  - fpp3: Data for "Forecasting: Principles and Practices" book.  Packages to run Time Series functions also included.
  - quantmod: "Quantitative Financial Modelling and Trading Framework for R"
  - Tidyquant:  Used to import stock data from the web into R Studio
  - imputeTS: Used to impute missing values in Time Series.  This makes sense for stock data, as there are days in which the stock market is closed (weekends, holidays)

 
## Launch

- Download .Rmd and import into R.  Make sure to download the packages listed in "Technologies Used"


## Screenshots

![Exponential Smoothing](./exponentialsmoothing.png)
Comparison of 3 types of exponential smoothing forecasts.  Clearly, the Holt forecast makes the most sense of these options, as it is following the trend of the data.

![Single Difference Log](./singledifferencelog.png)
Time Series, ACF, and PACF of single-differenced logged Closing stock data.  Data appears to be stationary based on this visual.

![SARIMA Forecast](./sarimaforecast.png)
Once the best SARIMA formula is chosen, a forecast of 12 months is shown in this visual.

![Neural Network Forecast](./neuralnetworkforecast.png)
Using a Neural Network, we can forecast the data up to a certain point.  I cannot seem to figure out how to extend this forecast beyond this point (and I would love if someone could assist me with this.)


## Acknowledgements

Thank you Professor Eric Suess for teaching this, and so many other, Statistics classes at Cal State East Bay.  Thank you again for allowing students to use projects to demonstrate what we have learned, and to put into our github's for the recruiters' viewing.  Shout out to Rob J Hyndman and George Athanasopoulos for writing an amazing book, "Forecasting: Principles and Practice."




