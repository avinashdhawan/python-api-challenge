# python-api-challenge
# Python API - What's the Weather Like?

## Background

In this analysis I wanted to be able to see if distance from the equator had an effect on metrics including Temperature, Humidity, Cloudiness and Windspeed.  To do this a list of 500 cities was randomly chosen

## Part I - WeatherPy

Initially I created a script to visualize the weather of 500+ cities across the world at different distances from the equator. To accomplish this, I used [CitiPy Python library](https://pypi.python.org/pypi/citipy), the [OpenWeatherMap API](https://openweathermap.org/api) to create a resonable model of cities from the equator.

The following scatter plots were created:

* Temperature (F) vs. Latitude
* Humidity (%) vs. Latitude
* Cloudiness (%) vs. Latitude
* Wind Speed (mph) vs. Latitude

After these plots were generated a linear regression line was used to get the best fit of the data based on ploting the Northern and Southern Hemispheres separately.

* Northern Hemisphere - Temperature (F) vs. Latitude
* Southern Hemisphere - Temperature (F) vs. Latitude
* Northern Hemisphere - Humidity (%) vs. Latitude
* Southern Hemisphere - Humidity (%) vs. Latitude
* Northern Hemisphere - Cloudiness (%) vs. Latitude
* Southern Hemisphere - Cloudiness (%) vs. Latitude
* Northern Hemisphere - Wind Speed (mph) vs. Latitude
* Southern Hemisphere - Wind Speed (mph) vs. Latitude

The notebook presented shows:

* 500 randomly selected cities based on latitude and longitude.
* Performed weather check on these cities using Openweather API calls.
* All retrieved data was saved as a CSV file.

### Part II - VacationPy

Now that I plotted the weather in the cities my goal was to using Google APIs find an ideal resort that the best weather profile.

I used jupyter-gmaps and the Google Places API for this part of the assignment.

* Created a heat map that displays the humidity for every city from the part I of the homework.

* To find the ideal temperature I used the following criteria:

  * A max temperature lower than 80 degrees but higher than 70.

  * Wind speed less than 10 mph.

  * Zero cloudiness.

* Using Google Places API to find the first hotel for each city located within 5000 meters of your coordinates.

* Plot the hotels on top of the humidity heatmap with each pin containing the **Hotel Name**, **City**, and **Country**.


Analysis was done using:

* Jupyter notebook.
* Matplotlib was used.

