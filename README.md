# World_Weather_Analysis


##Description


Provide real-time suggestions for client's ideal hotels. The "ideal" hotels are within a given range of latitude and longitude and provide the right kind of weather for the client.

1: Retrieve Weather Data
2: Create a Customer Travel Destinations Map
3: Create a Travel Itinerary Map

This repository includes:

The Weather_Database folder with the following:
- Weather_Database.ipynb file
- WeatherPy_Database.csv file

The Vacation_Search folder with the following:
- Vacation_Search.ipynb file
- WeatherPy_vacation.csv file
- WeatherPy_vacation_map.png image

The Vacation_Itinerary folder with the following:
- Vacation_Itinerary.ipynb file
- WeatherPy_travel_map.png image


Project Plan:
	
1. Collect the Data
	* Use the NumPy module to generate more than 1,500 random latitudes and longitudes.
	* Use the citipy module to list the nearest city to the latitudes and longitudes.
	* Use the OpenWeatherMap API to request the current weather data from each unique city in your list.
	* Parse the JSON data from the API request.
	* Collect the following data from the JSON file and add it to a DataFrame:
		▪ City, country, and date
		▪ Latitude and longitude
		▪ Maximum temperature
		▪ Humidity
		▪ Cloudiness
		▪ Wind speed
2. Exploratory Analysis with Visualization
	◦	Create scatter plots of the weather data for the following comparisons:
	▪	Latitude versus temperature
	▪	Latitude versus humidity
	▪	Latitude versus cloudiness
	▪	Latitude versus wind speed
	◦	Determine the correlations for the following weather data:
	▪	Latitude and temperature
	▪	Latitude and humidity
	▪	Latitude and cloudiness
	▪	Latitude and wind speed
	◦	Create a series of heatmaps using the Google Maps and Places API that showcases the following:
	▪	Latitude and temperature
	▪	Latitude and humidity
	▪	Latitude and cloudiness
	▪	Latitude and wind speed
	3	Visualize Travel Data Create a heatmap with pop-up markers that can display information on specific cities based on a customer's travel preferences. Complete these steps:
	1	Filter the Pandas DataFrame based on user inputs for a minimum and maximum temperature.
	2	Create a heatmap for the new DataFrame.
	3	Find a hotel from the cities' coordinates using Google's Maps and Places API, and Search Nearby feature.
	4	Store the name of the first hotel in the DataFrame.
	5	Add pop-up markers to the heatmap that display information about the city, current maximum temperature, and a hotel in the city.
