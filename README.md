# Box-Jenkins Method on the S&P 500

Stuart Truax, 2022-06

This notebook demonstrates the use of the Box-Jenkins method for time series model identification and parameter estimation. The time series is the inflation-adjusted monthly S&P 500 index for the years 1900 to 2017.

This application of the Box-Jenkins method suggests that the times series is best modeled by an ARIMA(2,1,0) process. The process is nonstationary, with a autorgressive order of 2 in the differenced series most strongly indicated by the data, suggesting that monthly index level changes in the S&P 500 are most strongly dependent on the previous two months of index level changes (i.e. a quarter in the past).


The __Box-Jenkins method__ is composed of two primary tasks:

1. __Model identification__ and determination of the degree of __stationarity__ of the time series.
2. __Parameter estimation__ for the identified model.

$\mathbf{x}$


## Visualizations from the Analyses

### Index Series Data at Different Levels of Differencing and Corresponding Autocorrelation Functions
<img src="output_14_0.png" width="300">

### Autocorrelation Function of the Differenced Series
<img src="output_41_0.png" width="300">

### Partial Autocorrelation Function of the Differenced Series
<img src="output_44_0.png" width="300">
