<img src="Pics/Header.png" width="682" height="296">

# python-api-challenge

# WeatherPY Analysis
The task of this project was to pull random cities throughout the world and see if there are any statistical correlations between the city’s global latitude and conditions.  The variables examined in this analysis include:
* City Name
* City Latitude
* City Longitude
* Max Temp (in Celsius) 
* Humidity
* Cloudiness
* Windspeed
* Country
* Date
<br>
547 randomly selected cities and their corresponding variable attributes were pulled from an API through OpenWeatherMap.org and put into a DataFrame for analysis.  A series of Scatter Plots were created to begin the statistical analysis.  The variables examined include:
<br>
<br>

* City Latitude vs Temperature
* City Latitude vs Humidity
* City Latitude vs Cloudiness
* City Latitude vs Wind Speed

### City Latitude vs Temperature
When examining City Max Latitude vs. Temperature (2022-10-18) most of the cities in the study seem to be located between a latitude of -40* to 40*, representing 2760 miles above and below the earth’s equator.  The majority of the cities in the chart reside in a Temperature (C) range of 0 to 35 degrees Celsius (32-95 degrees Fahrenheit).  This result is not surprising as 32-95 degrees Fahrenheit is typically a comfortable temperature range for human beings.       
<img src="Pics/CITY LATITUDE VS TEMPERATURE.png" width="640" height="480">

### City Latitude vs Humidity
While looking at City Latitude vs. Humidity (2022-10-18) the cities seem to be diversified across latitudinal coordinates, but a majority appear to reside in the 60-100% humidity range.  This graph shows a human tendency to gravitate to warmer climates with higher levels of humidity, but also outlines humans’ ability to adapt to a wide variety of latitudes and environmental environments.  This graph could also outline the need to expand latitude living locations as global populations continue to increase.

<img src="Pics/CITY LATITUDE VS HUMIDITY.png" width="640" height="480">

### City Latitude vs Cloudiness
When examining City Latitude vs. Cloudiness (2022-10-18) there appears to be wide variability in the data encompassing the entire range of latitudes shown in the graph.  There does seem to be tendency toward the statistical extremes when looking at Cloudiness %, with a majority of the cities residing at the extremes of 0% and 100%.  When looking at the entirety of this graph it shows us that most cities reside in areas with very low or very high cloud cover and span a wide variety of latitudes.
<img src="Pics/CITY LATITUDE VS CLOUDINESS.png" width="640" height="480">

### City Latitude vs Wind Speed
While looking at City Latitude vs. Wind Speed (2022-10-18) there appears to be wide variability in the higher city latitudes, but a tighter band of cities residing in the range below 6.5 wind speed(m/s). This result may not be all that surprising as a lower wind level would be more conducive to a wider range of outdoor human activities and be a positive addition to an overall living environment.      
<img src="Pics/CITY LATITUDE VS WIND SPEED.png" width="640" height="480">

### Temperature vs Latitude Linear Regression Plot
When examining the linear regression plot of Temperature vs Latitude for the Northern Hemisphere you immediately can see a strong negative correlation showing higher city temperatures as the latitude nears the equator and lower city temperatures as the latitude moves away from the equator.  This linear regression appears to show a strong correlation with a definitive negative slope and an r-value of -0.70.  This correlation also makes intuitive sense as temperatures generally tend to rise as locations get closer to the equator and drop as locations mover further away.             
When examining the Linear Regression Plot of Temperature vs Latitude for the Southern Hemisphere we see a weaker positive correlation between higher city temperatures as the latitude.  This linear regression displays a more gradual positive slope and a weaker r-value of 0.82.  A potential explanation of the weaker linear regression seen in the southern hemisphere could potentially be due to a significantly smaller human population in the southern hemisphere vs the norther hemisphere, allowing southern hemisphere cities to be more spread out geographically. 

<br>
<img src="Pics/TEMPERATURE VS LATITUDE LINEAR REGRESSION PLOT NORTH.png" width="573" height="376">
<img src="Pics/TEMPERATURE VS LATITUDE LINEAR REGRESSION PLOT SOUTH.png" width="576" height="373">


### Humidity vs Latitude Linear Regression Plot
The Humidity vs Latitude Linear Regression Plot for the Northern and Southern Hemispheres, both provided a low correlation in the results.  Both lineal regression plots show relatively loose positive correlations between city latitude and humidity, with a r-value in the north at 0.01 and a r-value in the south at 0.01.  Neither of these polts show strong considerations for city location in relation to humidity, and it can be assumed that other environmental factors play a much stronger role in determining where a city is to be located.   
<br>
<img src="Pics/HUMIDITY VS LATITUDE LINEAR REGRESSION PLOT NORTH.png" width="551" height="377">
<img src="Pics/HUMIDITY VS LATITUDE LINEAR REGRESSION PLOT SOUTH.png" width="552" height="378">

### Cloudiness vs Latitude Linear Regression Plot
Upon examining Cloudiness vs Latitude Linear Regression Plots for the Northern and Southern Hemispheres both plots show very weak correlations between Cloudiness and City Latitude.  The linear regression plot for both the northern and southern hemispheres shows a gradual positive slope and a r-value of 0.0128 for the northern hemisphere and a r-value of -0.1309. for the southern hemisphere.  The graphs for both hemispheres point to a weak correlation between city latitude and cloudiness.      
<br>
<img src="Pics/CLOUDINESS VS LATITUDE LINEAR REGRESSION PLOT NORTH.png" width="564" height="377">
<img src="Pics/CLOUDINESS VS LATITUDE LINEAR REGRESSION PLOT SOUTH.png" width="566" height="375">

### Wind Speed vs Latitude Linear Regression Plot
When looking that the Latitude Linear Regression Plots for Wind Speed vs City Latitude, both plots (northern and southern) show a very low correlation between the variables.  The plot for the northern hemisphere shows an almost horizonal slope with a r-value of -0.029 while the southern hemisphere plot shows a slightly negative slope with an r-value of -0.079.  Both plots display a very low correlation between city latitude and wind speed.

<br>
<img src="Pics/WIND SPEED VS LATITUDE LINEAR REGRESSION PLOT NORTH.png" width="570" height="377">
<img src="Pics/WIND SPEED VS LATITUDE LINEAR REGRESSION PLOT SOUTH.png" width="571" height="373">


# VacationPY Analysis
In this deliverable, weather data skills were used to plan future vacations. This was accomplished using Jupyter notebooks, the geoViews Python library, and the Geoapify API.

### Create a map that displays a point for every city in the city DataFrame.  The size of the point should be the humidity in each city.

<img src="Pics/Initial Map.png" width="957" height="459">


### Narrow down the DataFrame to find your ideal weather conditions:
* A max temperature lower than 27 degrees but higher than 21
* Wind speed less than 4.5 m/s
* Zero cloudiness

<img src="Pics/Ideal Weather.png" width="879" height="725">
  
### For each city, use the Geoapify API to find the first hotel located within 10,000 meters of your coordinates.  

<img src="Pics/Associated Hotels.png" width="689" height="726">



### Add the hotel name and the country as additional information in the hover message for each city on the map.

<img src="Pics/Hotel Map.png" width="923" height="457">

