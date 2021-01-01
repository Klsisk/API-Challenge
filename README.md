# Python API : What's the Weather Like?

## Part I - WeatherPy
In this example, you'll be creating a Python script to visualize the weather of 500+ cities across the world of varying distance from the equator. To accomplish this, you'll be utilizing a simple Python library, the OpenWeatherMap API, and a little common sense to create a representative model of weather across world cities.
1. Your first requirement is to create a series of scatter plots to showcase the following relationships:
- Temperature (F) vs. Latitude
- Humidity (%) vs. Latitude
- Cloudiness (%) vs. Latitude
- Wind Speed (mph) vs. Latitude

After each plot, add a sentence or too explaining what the code is and analyzing.

2. Your second requirement is to run linear regression on each relationship, only this time separating them into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude):
- Northern Hemisphere - Temperature (F) vs. Latitude
- Southern Hemisphere - Temperature (F) vs. Latitude
- Northern Hemisphere - Humidity (%) vs. Latitude
- Southern Hemisphere - Humidity (%) vs. Latitude
- Northern Hemisphere - Cloudiness (%) vs. Latitude
- Southern Hemisphere - Cloudiness (%) vs. Latitude
- Northern Hemisphere - Wind Speed (mph) vs. Latitude
- Southern Hemisphere - Wind Speed (mph) vs. Latitude

After each pair of plots, explain what the linear regression is modeling such as any relationships you notice and any other analysis you may have.

Your final notebook must:
- Randomly select at least 500 unique (non-repeat) cities based on latitude and longitude.
- Perform a weather check on each of the cities using a series of successive API calls.
- Include a print log of each city as it's being processed with the city number and city name.
- Save a CSV of all retrieved data and a PNG image for each scatter plot.

## Observation of the data:
1. When pulling random cities from the OpenWeatherMap API and looking at its data, you can see that the weather conditions in the North appear more harsh in comparison to the South. The max temperature is highest at 0 latitude and begins to drop as the Latitude decreases.

2. You can also see that there appears to be more humidity in some areas of the world, particularly above 40 degrees Latitude.

3. When looking at the relationship between City Latitude and Wind Speed, it appears to show that there isn't really high wind speeds all across the globe. Many of the wind speeds are less than 15 mph. For the parts of the world that are between 0-80 degrees Latitude, most of their wind speeds are under 10 mph.
