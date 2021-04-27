### Time Series on Covid Cases Using Fbprophet Version 1
Prophet is a procedure for forecasting time series data based on an additive model where non-linear trends are fit with yearly, weekly, and daily seasonality, plus holiday effects. It works best with time series that have strong seasonal effects and several seasons of historical data. Prophet is robust to missing data and shifts in the trend, and typically handles outliers well.
Eg:
  from fbprophet import Prophet
  m = Prophet()
  m.fit(df)  # df is a pandas.DataFrame with 'y' and 'ds' columns
  future = m.make_future_dataframe(periods=365)
  m.predict(future)

### Why FBProphet?
FBProphet uses time as a regressor and tries to fit several linear and nonlinear function of time as components. By default, FBProphet will fit the data using a linear model but it can be changed to the nonlinear model (logistics growth) from its arguments.

I'll be exploring more of these with respect to ARIMA models vs FBProphet..
Work In Progress.
