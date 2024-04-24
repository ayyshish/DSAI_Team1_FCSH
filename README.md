# FCSH Team 1 DSAI report

In this report, we explore stocks, a core financial instrument, and analyse them as time-series data. We look into the general, aggregated, trends of stocks across industries and explore their historical performance. We aim to model the movement of this data with traditionally recognised methods, such as AutoRegressive and Linear Regression models.

In this process, we will look into our data and process them to represent an aggregated movement across a larger time period, such as by weeks, or by years. We implement feature engineering techniques such as finding returns instead of raw prices to understand concepts behind time-series data, such as stationarity. We find links between what we have learnt for stationary data in SC1015, such as normal distributions, standard deviations, and correlations, and apply them to fit the specific context of financial data. The report will look into the following:

1) Price movement of a stock
2) Returns of a stock
3) Aggregated returns over a time period using resampling
4) Volatility
5) Stationarity (Using an Augmented Dickey-Fuller test)
6) Correlations with past values (Autocorrelation function and Partial Autocorrelation function)
7) Correlations with external time series data (Cross-correlation function)
8) Modelling data using Auto Regressive models
9) Modelling data using Linear Regression and external variables

Throughout this process, we find purposeful results such as:

1) Modelling data on aggregated values tend to be more stable and accurate
2) Improving our model by introducing external variables that have a high correlation with our data
