# 06-Python-API-Challenge

______________________________________________________________________
WeatherPy

Code: WeatherPy/WeatherPy.ipynb
Data source: OpenWeather API
Analysis results buried in the code file.
Python packages: matplotlib.pyplot, pandas, numpy, requests, time, scipy.stats, citipy

Description:

generate random coordinate pairs 
locate the nearest city of the lat-lon pairs
get weather info of the cities and store in dataframe
scatter plot latitude vs Temperature/Humidity/Cloudiness/Wind Speed of the cities


divide cities by lat into 2 sub-groups: north/south hemisphere
scatter plot and run linear regression on 
  latitude vs Temperature/Humidity/Cloudiness/Wind Speed of the cities
   
Conclusion:
1. Temperature and Latitude are strongly correlated, the closer to eqator, the hotter.
2. Correlation between Humidity/Cloudiness and Latitude are positive and weak in both hemispheres.
3. Correlation between Wind Speed and Latitude is a bit complicate:
     in north hemisphere, it is very weak but positive
     in south hemisphere, it is moderate and negative

______________________________________________________________________
