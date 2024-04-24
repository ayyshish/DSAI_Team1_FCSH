# FCSH Team 1 DSAI report

## About

In this report, we explore stocks, a core financial instrument, and analyse them as time-series data. We look into the general, aggregated, trends of stocks across industries and explore their historical performance. We aim to model the movement of this data with traditionally recognised methods, such as AutoRegressive and Linear Regression models. Complete details and source codes are all available under the complete jupyter notebook within this repository.

## Contributors

- @ayyshish - Data Visualisation, Data Processing
- @clairecxy - Data extraction, Data Processing
- @hiimstevenzhu - Feature Engineering, Statistical Models

## Problem definition

- Can we forecast the performance of an aggregated industry?
- Which models, variables, and timeframes are suitable for forecasting?

## Models Used

- Auto Regressive Model
- Linear Regression Model

# Project content, and main takeaways

We look into our data and process them to represent an aggregated movement across a larger time period, such as by weeks, or by years. We implement feature engineering techniques such as finding returns instead of raw prices to understand concepts behind time-series data, such as stationarity. We find links between what we have learnt for stationary data in SC1015, such as normal distributions, standard deviations, and correlations, and apply them to fit the specific context of financial data. The report will consolidate our learnings:

1. Price movement of a stock
2. Returns of a stock
3. Aggregated returns over a time period using resampling
4. Volatility
5. Stationarity (Using an Augmented Dickey-Fuller test)
6. Correlations with past values (Autocorrelation function and Partial Autocorrelation function)
7. Correlations with external time series data (Cross-correlation function)
8. Modelling data using Auto Regressive models
9. Modelling data using Linear Regression and external variables

## Conclusion

1. Using returns instead of prices tends to give better stationarity for linear regression fits - we have a clear distribution with a constant mean and variance
2. Modelling data on aggregated values tend to be more stable and accurate (Lower MSE on yearly returns vs weekly returns)
3. The previous prices/returns of an industry has little correlation with its current value
4. Certain industries tend to be heavily correlated with each other
5. Modelling data using values from other correlated industries on top of its own previous values improve our MSE

## References

https://www.kaggle.com/code/iamleonie/time-series-interpreting-acf-and-pacf
https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LinearRegression.html
https://www.investopedia.com/terms/a/autoregressive.asp
https://www.investopedia.com/terms/c/crosscorrelation.asp
https://otexts.com/fpp2/stationarity.html
https://www.statisticssolutions.com/free-resources/directory-of-statistical-analyses/assumptions-of-linear-regression/
