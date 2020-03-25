## COVID-19 USA Time Series Forecasting 

![](https://cdn-images-1.medium.com/max/800/1*pVvHziu_jDLr_I179JeWlw.png)
 

### Introduction
___

Prophet is a procedure for forecasting time series data based on an additive model where non-linear trends are fit with yearly, weekly, and daily seasonality, plus holiday effects. It works best with time series that have strong seasonal effects and several seasons of historical data. Prophet is robust to missing data and shifts in the trend, and typically handles outliers well.

### Data Source
___

* Data downloaded from [Novel Coronavirus COVID-19 (2019-nCoV) Data Repository by Johns Hopkins CSSE](https://github.com/CSSEGISandData/COVID-19)

* [Time Series Data:Confirmed, Recovered and Deaths](https://github.com/CSSEGISandData/COVID-19/tree/master/csse_covid_19_data/csse_covid_19_time_series)

### Data Format

* Time: MM-DD-YYYY.csv in UTC.
*  Province/State: China - province name; US/Canada/Australia/ - city name, state/province name; Others - name of the event (e.g., "Diamond Princess" cruise ship); other countries - blank.
*  Country/Region: country/region name conforming to WHO (will be updated).
*  Last Update: MM/DD/YYYY HH:mm (24 hour format, in UTC).
*  Confirmed: the number of confirmed cases. For Hubei Province: from Feb 13 (GMT +8), we report both clinically diagnosed and lab-confirmed cases. For lab-confirmed cases only (Before Feb 17), please refer to who_covid_19_situation_reports. For Italy, diagnosis standard might be changed since Feb 27 to "slow the growth of new case numbers." (Source)
*  Deaths: the number of deaths.
*  Recovered: the number of recovered cases.

### Installation in Python
___

Prophet is on PyPI, so you can use pip to install it:

#bash

$ pip install fbprophet

The major dependency that Prophet has is pystan. PyStan has its [own installation instructions](https://pystan.readthedocs.io/en/latest/windows.html). Install pystan with pip before using pip to install fbprophet.
  
### Code Compatibility
___

* Google Colab
* Python 3.0
* Prophet Version 0.6 (2020.03.03)
 

  
