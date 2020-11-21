# Time_Series_and_Linear_Regression_Forecasting_Simulation

## Time Series Analysis

In the time series analysis notebook, we look at historical yen to US dollar data. We use different models to forecast returns, settle price, and voltility. The Questions we are attempting to answer with these models are: Do wee see any patterns of the settle price, long-term and/or short? Based on the p-value, is our ARMA model a good fit? What does our ARIMA model forecast will happen to the Japanese Yen in the near term? Based on our time series analysis, would we buy the yen now? Is the risk of the yen expected to increase or decrease? Based on the model evaluation, would we feel confident in using these models for trading?

Do wee see any patterns of the settle price, long-term and/or short? 

Based on the plot in our notebook file, we can see a long-term strengthening of the Japanese Yen against the Dollar. There do seem to be some more medium, 1-3 year consistent trends, but on a daily basis, there are a lot of short-term ups and downs.

Based on the p-value, is our ARMA model a good fit? 

Based on the ARMA model summary table, none of the p-values are below 0.05, which suggests that additional input variables may need to be added or the lag order needs to be adjusted. Assuming we are confident with this model's ability to predict, however, our model-based forecast for the next 5 days is of positive returns for the Yen.

What does our ARIMA model forecast will happen to the Japanese Yen in the near term? 

Based on the graph in our notebook file, it looks like the price of the Yen is going to rise over the next five days, which is consistent with the findings of the ARMA model.

Based on our time series analysis, would we buy the yen now? Is the risk of the yen expected to increase or decrease? Based on the model evaluation, would we feel confident in using these models for trading?

Based on our time series analysis, it would make sense to buy the yen now, with anticipation that it will rise further over the next five days. However, the risk is also forecast to rise. This means there might be some days in the interim where we see larger than usual swings in the price. 

Overall, our model for forecasting volatility looks reasonably solid. However, our models for predicting future yen returns, ARMA, and for yen prices, ARIMA, seem like they could use some improvement before we start using them to make financial bets. This is because none of the features included in the model were significant, as all had p-values above 0.05.


## Linear Regression

In the regression analysis notebook we build a linear regression model to see how performs on out-of-sample data versus in-sample data. Based on our model, we have a root mean squarred error of about 0.415 for the out-of-sample data and 0.596 for the in-sample data. This means that our linear regression model performs slightly better on data that it hasn't seen before.

Even though our linear regression has performed better on the out-of-sample data, we should expect a higher rate for this type of data since the model is trained to predict the in-sample data as best as it can. It is possible that if additional data continued to be added over time then the out-of-sample performance may not continue to be as good, meaning the out-of-sample root mean squared error may rise.

