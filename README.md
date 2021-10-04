# A Yen for the Future

![Yen Photo](Images/unit-10-readme-photo.png)

## Background

The financial departments of large companies often deal with foreign currency transactions while doing international business. As a result, they are always looking for anything that can help them better understand the future direction and risk of various currencies. Hedge funds, too, are keenly interested in anything that will give them a consistent edge in predicting currency movements.

In this assignment, I tested some time-series tools in order to predict future movements in the value of the Japanese yen versus the U.S. dollar.

- - -

### Time-Series Forecasting

Loaded historical Dollar-Yen exchange rate futures data and applied time series analysis and modeling to determine whether there is any predictable behavior.

**Analysis:**

1. Decomposed the Settle price into trend and noise using a Hodrick-Prescott Filter. 
2. Forecasted Returns using an ARMA Model.
3. Forecasted the Settle Price using an ARIMA Model.
4. Forecasted Volatility with GARCH.

**Based on the results of the time series analysis and modeling:**

Based on my analysis I would not buy Yen now. The ARMA and ARIMA models are not good fits because the p values are all significantly higher than .05. Based on the GARCh model the risk of yen is going to increase. I do not feel confident is using these models for trading at the moment. I would like to analyze how they performed in five days versus the actual data. Then I would repeat the process and tweak the models accordingly. 


### Linear Regression Forecasting

Built a Scikit-Learn linear regression model to predict Yen futures ("settle") returns with *lagged* Yen futures returns and categorical calendar seasonal effects (e.g., day-of-week or week-of-year seasonal effects).

**Analysis:**

1. Data Preparation - prepared the data, created returns and lagged returns, then split the data into training and testing sets.
2. Fit a Linear Regression Model to the data.
3. Made predictions using the testing data.
4. Evaluated out-of-sample performance - data the model has not seen before aka Testing Data.
5. Evaluated in-sample performance - data the model was trained on aka Training Data.

**Based on the results of the linear regression analysis and modeling:**

After analyzing the data, the out-of-sample data performed better than the in-sample data. For the out-of-sample data both the mean squared error and the root mean squared error were less than than the in-sample data.

