<img src="Pics/Header.png" width="682" height="296">

# python-api-challenge
##### Link to WeatherPY code - https://github.com/MichaelELeonard/python-api-challenge/blob/main/WeatherPyWorking.ipynb


## WeatherPY Analysis
The task of this project was to pull random cities throughout the world and see if there are any statistical correlations between the city’s global latitude and its weather conditions.  The variables examined in this analysis include:
* City Name
* City Latitude
* City Longitude
* Max Temp (in Celsius) 
* Humidity
* Cloudiness
* Windspeed
* Country
* Date
  

560 randomly selected cities and their corresponding variable attributes were pulled from an API through OpenWeatherMap.org and put into a DataFrame for analysis.  A series of Scatter Plots were created to begin the statistical analysis.  The variables examined include:
* City Latitude vs Temperature
* City Latitude vs Humidity
* City Latitude vs Cloudiness
* City Latitude vs Wind Speed



## City Latitude vs Temperature
When examining City Max Latitude vs. Temperature most of the cities in the study seem to be located between a latitude of -40* to 60*, representing 3450 miles above and below the earth’s equator.  Most of the cities in the chart reside in a Temperature (C) range of 0 to 35 degrees Celsius (32-95 degrees Fahrenheit).  This result is not surprising as 32-95 degrees Fahrenheit is typically a comfortable temperature range for human beings.       

<img src="Pics/CITY LATITUDE VS TEMPERATURE.png" width="468" height="377">

## City Latitude vs Humidity
While looking at City Latitude vs. Humidity the cities seem to be diversified across latitudinal coordinates, but a majority appear to reside in the 60-100% humidity range.  This graph highlights a human tendency to gravitate to warmer climates with higher levels of humidity, but also outlines humans’ ability to adapt to a wide variety of latitudes and environmental environments.  


<img src="Pics/CITY LATITUDE VS HUMIDITY.png" width="475" height="376">

## City Latitude vs Cloudiness
When examining City Latitude vs. Cloudiness there appears to be wide variability in the data encompassing the entire range of latitudes shown in the graph.  There does seem to be tendency toward the statistical extremes when looking at Cloudiness %, with most of the cities residing at the extremes of 0% and 100% cloud cover.  

<img src="Pics/CITY LATITUDE VS CLOUDINESS.png" width="474" height="375">

## City Latitude vs Wind Speed
While looking at City Latitude vs. Wind Speed there appears to be wide variability in the higher city latitudes, but a tighter band of cities residing in the range below 6.5 wind speed(m/s). This result may not be all that surprising as a lower wind level would be more conducive to a wider range of outdoor human activities and be a positive addition to an overall living environment.      
<img src="Pics/CITY LATITUDE VS WIND SPEED.png" width="468" height="376">

## Temperature vs Latitude Linear Regression Plot
When examining the Linear Regression Plot of Temperature vs Latitude for the Northern Hemisphere you see a negative correlation showing higher city temperatures as the latitude nears the equator and lower city temperatures as the latitude moves away from the equator.  This linear regression shows a negative slope and an r-value of -0.69.  This correlation also makes intuitive sense as temperatures generally tend to rise as locations get closer to the equator and drop as locations move further away.      
       
<img src="Pics/TEMPERATURE VS LATITUDE LINEAR REGRESSION PLOT NORTH.png" width="491" height="376">

When examining the Linear Regression Plot of Temperature vs Latitude for the Southern Hemisphere we see a positive correlation between higher city temperatures as the latitude.  This linear regression displays a positive slope and a r-value of 0.78.  A potential explanation of this linear regression in the southern hemisphere could potentially be due to a significantly smaller human population in the southern hemisphere vs the norther hemisphere, allowing southern hemisphere cities to be more spread out geographically. 

<img src="Pics/TEMPERATURE VS LATITUDE LINEAR REGRESSION PLOT SOUTH.png" width="495" height="374">


## Humidity vs Latitude Linear Regression Plot
The Humidity vs Latitude Linear Regression Plot for the Northern and Southern Hemispheres provided similar results.  Both Lineal Regression plots show relatively loose correlations between city latitude and humidity, with a r-value in the north at 0.03 and a r-value in the south at -0.09.  Neither of these plots show strong considerations for city location in relation to humidity, and it can be assumed that other environmental factors play a much stronger role in determining where a city is to be located.   
<br>
<img src="Pics/HUMIDITY VS LATITUDE LINEAR REGRESSION PLOT NORTH.png" width="488" height="375">

<img src="Pics/HUMIDITY VS LATITUDE LINEAR REGRESSION PLOT SOUTH.png" width="488" height="375">

## Cloudiness vs Latitude Linear Regression Plot
Upon examining Cloudiness vs Latitude Linear Regression Plots for the Northern and Southern Hemispheres both plots show very weak correlations between Cloudiness and City Latitude.  The linear regression plot for both the northern and southern hemispheres shows a gradual slopes and a r-value of -0.01 for the northern hemisphere and a r-value of 0.1. for the southern hemisphere.  The graphs for both hemispheres point to a weak correlation between city latitude and cloudiness.      
<br>
<img src="Pics/CLOUDINESS VS LATITUDE LINEAR REGRESSION PLOT NORTH.png" width="493" height="376">

<img src="Pics/CLOUDINESS VS LATITUDE LINEAR REGRESSION PLOT SOUTH.png" width="494" height="375">

## Wind Speed vs Latitude Linear Regression Plot
When looking that the Latitude Linear Regression Plots for Wind Speed vs City Latitude, both plots (northern and southern) show a very low correlation between the variables.  The plot for the northern hemisphere shows an almost horizonal slope with a r-value of 0.02 while the southern hemisphere plot shows a slightly negative slope with an r-value of -0.09.  Both plots display a very low correlation between city latitude and wind speed.

<br>
<img src="Pics/WIND SPEED VS LATITUDE LINEAR REGRESSION PLOT NORTH.png" width="490" height="376">
<img src="Pics/WIND SPEED VS LATITUDE LINEAR REGRESSION PLOT SOUTH.png" width="490" height="376">


## VacationPY Analysis

##### Link to VacationPY code - https://github.com/MichaelELeonard/python-api-challenge/blob/main/VacationPyWorking.ipynb

In this deliverable, weather data skills were used to plan future vacations. This was accomplished using Jupyter notebooks, the geoViews Python library, and the Geoapify API.


## The map displays a point for every city in the city DataFrame.  The size of the point correlates to the humidity in each city.

<img src="Pics/Initial Map.png" width="957" height="459">


## The DataFrame was filtered to find your ideal weather conditions:
* A max temperature lower than 27 degrees but higher than 21
* Wind speed less than 4.5 m/s
* Zero cloudiness

<img src="Pics/Ideal Weather.png" width="879" height="725">


## For each city, Geoapify API was used to find the first hotel located within 10,000 meters of the coordinates.  

<br>

<img src="Pics/Associated Hotels.png" width="689" height="726">


## The hotel name and country of origin was added to the map with additional information included as a hover message for each location.

<br>

<img src="Pics/Hotel Map.png" width="923" height="457">

