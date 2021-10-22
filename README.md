# Python API  - What's the Weather Like?

![Equator](Images/equatorsign.png)

## Part I - WeatherPy

I created a Python script to visualize the weather of 500+ cities across the world of varying distance from the equator using [simple Python library](https://pypi.python.org/pypi/citipy) and the [OpenWeatherMap API](https://openweathermap.org/api). 

To visually explore the characteristics of global weather, I created a series of scatter plots to showcase the following relationships:

* Temperature (F) vs. Latitude
* Humidity (%) vs. Latitude
* Cloudiness (%) vs. Latitude
* Wind Speed (mph) vs. Latitude

To mathematically explore the data I ran simple linear regressions for the following characteristics, separating the plots into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude):

* Northern Hemisphere - Temperature (F) vs. Latitude
* Southern Hemisphere - Temperature (F) vs. Latitude
* Northern Hemisphere - Humidity (%) vs. Latitude
* Southern Hemisphere - Humidity (%) vs. Latitude
* Northern Hemisphere - Cloudiness (%) vs. Latitude
* Southern Hemisphere - Cloudiness (%) vs. Latitude
* Northern Hemisphere - Wind Speed (mph) vs. Latitude
* Southern Hemisphere - Wind Speed (mph) vs. Latitude

### Part II - VacationPy

Here is a heatmap representing the humidity level of every city within the dataset.

  ![heatmap](Images/heatmap.png)

* I then wanted to narrow down my dataset by choosing conditions that met my ideal weather conditions for a vacations

  * A max temperature lower than 90 degrees but higher than 80.

  * Wind speed less than 15 mph.

  * I dropped any rows that didn't contain all conditions. I wanted to be sure the weather is ideal.

  
* I then used Google Places API to find the first hotel for each city located within 5000 meters of my remaining candidate cities.

* I plotted the hotels on top of the humidity heatmap with each pin containing the **Hotel Name**, **City**, and **Country**.

  ![hotel map](Images/hotel_map.png)



