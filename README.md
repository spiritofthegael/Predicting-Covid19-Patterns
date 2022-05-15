# Predicting-Covid19-Patterns
- uses time series data from https://github.com/owid/covid-19-data/tree/master/public/data/
- data goes from Januaray 27th, 2020 to November 22, 2020 (301 days)
- data before January 27th removed to get rid of noise
- covid19dataset.ipynb uses the Dickey-Fuller test to see if data is stationary
  - utilizes a logarithmic transformation to remove the multiplicative trend from the data
  - removes seasonality
  - .pynb file uses Python3
- uses linear regression to predict case counts and case deaths for the future
- achieved a relative error score of around .03 for both cases and deaths
# Future Directions
- other forms of seasonality and patterns may show up in the data, especially if broken down by country:
  - when lockdowns were started and ended
  - how strict the type of lockdown was
- a more complicated network, such as an LSTM may improve results
