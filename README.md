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
VacationPy

Code: WeatherPy/VacationPy.ipynb
Data source: OpenWeather API, Geoapifi
Analysis results buried in the code file.
Python packages: hvplot.pandas, pandas, requests

Description:

read city data generated in WeatherPy
create a map, display humidity as point size
filter cities to identify good ones:
  max temperature between 20-30 C
  wind speed less then 4.5 m/s
  cloudiness < 10
use Geoapify to query the nearest hotels of the good cities 
  within 10000 m radius
add hotel name to dataframe 
display city and hotel in map as hover messege

result:

some cities do not have Hotel within 10000 m radius, maybe we need to use accommodation.motel in categories.
______________________________________________________________________
