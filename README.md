# Python API : What's the Weather Like?

## Part I - WeatherPy
In this example, you'll be creating a Python script to visualize the weather of 500+ cities across the world of varying distance from the equator. To accomplish this, you'll be utilizing a simple Python library, the OpenWeatherMap API, and a little common sense to create a representative model of weather across world cities.
1. Your first requirement is to create a series of scatter plots to showcase the following relationships:
- Temperature (F) vs. Latitude

![image](https://user-images.githubusercontent.com/69765842/103466242-34c46100-4d11-11eb-8587-d5fc96b7350e.png)

- Humidity (%) vs. Latitude

![image](https://user-images.githubusercontent.com/69765842/103466248-40b02300-4d11-11eb-9d36-d9f580aea6e6.png)

- Cloudiness (%) vs. Latitude

![image](https://user-images.githubusercontent.com/69765842/103466253-486fc780-4d11-11eb-8ea9-5b14b7c46dad.png)

- Wind Speed (mph) vs. Latitude

![image](https://user-images.githubusercontent.com/69765842/103466257-5291c600-4d11-11eb-8194-c2e7a6d293f4.png)

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

## Part II - VacationPy
Using jupyter-gmaps and the Google Places API for this part of the assignment,:
- Create a heat map that displays the humidity for every city from the part I of the homework.

![image](https://user-images.githubusercontent.com/69765842/103466232-18282900-4d11-11eb-8735-3bbf6cab1ccb.png)

- Narrow down the DataFrame to find your ideal weather condition. For example:
  - A max temperature lower than 80 degrees but higher than 70.
  - Wind speed less than 10 mph.
  - Zero cloudiness
  - Drop any rows that don't contain all three conditions. You want to be sure the weather is ideal.
  
 
  
- Using Google Places API to find the first hotel for each city located within 5000 meters of your coordinates.
- Plot the hotels on top of the humidity heatmap with each pin containing the Hotel Name, City, and Country.

![image](https://user-images.githubusercontent.com/69765842/103466237-2b3af900-4d11-11eb-8fb2-85f40a6f9362.png)

## Observation of the data:
1. When pulling random cities from the OpenWeatherMap API and looking at its data, you can see that the weather conditions in the North appear more harsh in comparison to the South. The max temperature is highest at 0 latitude and begins to drop as the Latitude decreases.

2. You can also see that there appears to be more humidity in some areas of the world, particularly above 40 degrees Latitude.

3. When looking at the relationship between City Latitude and Wind Speed, it appears to show that there isn't really high wind speeds all across the globe. Many of the wind speeds are less than 15 mph. For the parts of the world that are between 0-80 degrees Latitude, most of their wind speeds are under 10 mph.
