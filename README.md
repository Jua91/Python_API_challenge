# Python API Homework - What's the Weather Like?

The purpose of this project was to analyze how weather changes at different levels of latitude. I pulled data from OpenWeatherMap API to assemble a datset on over 500 cities.

## Part I - WeatherPy

The following scatter plots are showcased:

* Temperature (F) vs. Latitude
![Temperature vs Latitude](output_data/lat_vs_temp.png)
* Humidity (%) vs. Latitude
![Humidity vs Latitude](output_data/lat_vs_humidity.png)
* Cloudiness (%) vs. Latitude
![Cloudines vs Latitude](output_data/lat_vs_cloudiness.png)
* Wind Speed (mph) vs. Latitude
![Wind Speed vs Latitude](output_data/lat_vs_windspeed.png)

* Northern Hemisphere - Temperature (F) vs. Latitude
![NH_temperature_vs_lat](output_data/NH_regression_temp_vs_lat.png)
* Southern Hemisphere - Temperature (F) vs. Latitude
![SH_temperature_vs_lat](output_data/SH_regression_temp_vs_lat.png)
* Northern Hemisphere - Humidity (%) vs. Latitude
![NH_humidity_vs_lat](output_data/NH_regression_humidity_vs_lat.png)
* Southern Hemisphere - Humidity (%) vs. Latitude
![SH_humidity_vs_lat](output_data/SH_regression_humidity_vs_lat.png)
* Northern Hemisphere - Cloudiness (%) vs. Latitude
![NH_cloudiness_vs_lat](output_data/NH_regression_cloudiness_vs_lat.png)
* Southern Hemisphere - Cloudiness (%) vs. Latitude
![SH_cloudiness_vs_lat](output_data/SH_regression_cloudiness_vs_lat.png)
* Northern Hemisphere - Wind Speed (mph) vs. Latitude
![NH_windspeed_vs_lat](output_data/NH_regression_windspeed_vs_lat.png)
* Southern Hemisphere - Wind Speed (mph) vs. Latitude
![SH_windspeed_vs_lat](output_data/SH_regression_windspeed_vs_lat.png)


### Observations:
* Temperatures get higher as the city gets nearer to the equator (where latitude is 0).

* In the northern hemisphere, the latitude and temperature have negative correlation while in the southern hemisphere, the latitude and temperature have positive correlation.

* The cloudiness has a little correlation with the latitude. It seems that as the city gets further from the equator, the city gets more cloudy.

* Windspeed and latitude has no correlation, since the slope is nearly zero. Windspeed is not affected by the latitude.




## Part II - VacationPy

Jupyter-gmaps and the Google Places API were used to create a heat map for this part of the assignment.

* Create a heat map that displays the humidity for every city from the part I of the homework.

* Narrow down the DataFrame to find your ideal weather condition. For example:

  * A max temperature lower than 80 degrees but higher than 70.
  * Wind speed less than 10 mph.
  * Zero cloudiness.
  * Drop any rows that don't contain all three conditions. You want to be sure the weather is ideal.

* Using Google Places API to find the first hotel for each city located within 5000 meters of your coordinates.

* Plot the hotels on top of the humidity heatmap with each pin containing the **Hotel Name**, **City**, and **Country**.

![heatmap](output_data/map.png)
