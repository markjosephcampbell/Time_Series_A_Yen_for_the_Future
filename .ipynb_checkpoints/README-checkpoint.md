# A Yen for the Future

![Yen Photo](Images/unit-10-readme-photo.png)

## Background

The financial departments of large companies often deal with foreign currency transactions while doing international business. As a result, they are always looking for anything that can help them better understand the future direction and risk of various currencies. Hedge funds, too, are keenly interested in anything that will give them a consistent edge in predicting currency movements.

In this assignment, I tested the some time-series tools in order to predict future movements in the value of the Japanese yen versus the U.S. dollar.

- - -

### Time-Series Forecasting

Loaded historical Dollar-Yen exchange rate futures data and applied time series analysis and modeling to determine whether there is any predictable behavior.

**Analysis:**

1. Decomposition of the Settle price into trend and noise using a Hodrick-Prescott Filter 
2. Forecasting Returns using an ARMA Model.
3. Forecasting the Settle Price using an ARIMA Model.
4. Forecasting Volatility with GARCH.

Based on the results of the time series analysis and modeling:

1. Based on your time series analysis, would you buy the yen now?
2. Is the risk of the yen expected to increase or decrease?
3. Based on the model evaluation, would you feel confident in using these models for trading?


### Linear Regression Forecasting

Built a Scikit-Learn linear regression model to predict Yen futures ("settle") returns with *lagged* Yen futures returns and categorical calendar seasonal effects (e.g., day-of-week or week-of-year seasonal effects).

**Analysis:**

1. Data Preparation - prepared the data, creates returns and lagged returns, then split the data into training and testing sets.
2. Fit a Linear Regression Model to the data.
3. Made predictions using the testing data.
4. Evaluated out-of-sample performance - data the model has not seen before aka Testing Data.
5. Evaluated in-sample performance - data the model was trained on aka Training Data.

Based on the results of the linear regression analysis and modeling:

* Does this model perform better or worse on out-of-sample data compared to in-sample data?
* Analyze the model performance for out-of-sample and in-sample data and write a conclusion

