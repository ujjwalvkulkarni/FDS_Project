# FORECASTING NEW YORK CITY CRIME DATA
Our goal is to build a forecasting model that can accurately predict Criminal Data in NYC. Our method will be to use an ARIMA Model to predict the criminal data and to use the clustering techniques of KNN to cluster the types of crimes in each borough given those predictions. We want to use these forecast to help prepare law enforcement and citizens.

The data that we are using for this project comes from NYC Open data website. The dataset we are working with has 7.38M instances with 35 features. The data dates back to 2006
https://data.cityofnewyork.us/Public-Safety/NYPD-Complaint-Data-Historic/qgea-i56i

Due to the size of the data set, we went through each feature to help us reduce dimensionality
There were features removed that were duplicates (Ex: removing the latitude and longitude when we were presented with a Geospatial location point)
Removed suspect data since we are not trying to target groups of people that have committed crimes but instead populations as a whole
Went through and removed incomplete or not relevant instances from the data set (crimes that happened before 2006 but were reported in 2006 onwards)
Our final data set contains 6.82 million instances with 16 features each

The Splitter.py file splits the entire dataset into 5 boroughs.

The NYC_cleaned.py is the main program which visualises the data and forecasts the data using ARIMA.
