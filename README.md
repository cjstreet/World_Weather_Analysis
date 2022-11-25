# World_Weather_Analysis


describes the purpose of the repository. Although there is no graded written analysis for this challenge, it is encouraged and good practice to add a brief description of your project.

For this challenge, you will use the weather description data you've already retrieved in this module to enhance the PlanMyTrip app. Then, you'll have the beta testers use input statements to filter the data for their weather preferences, which will be used to identify potential travel destinations and nearby hotels. The beta tester will choose four cities from the list of potential travel destinations to create a travel itinerary. Finally, using the Geoapify Routing API, you will create a travel route between the four cities and a marker layer map.

Deliverable 1: Retrieve Weather Data
Deliverable 2: Create a Customer Travel Destinations Map
Deliverable 3: Create a Travel Itinerary Map
Upload the following to your WeatherPy GitHub repository:

The Weather_Database folder with the following:

The Weather_Database.ipynb file
The WeatherPy_Database.csv file
The Vacation_Search folder with the following:

The Vacation_Search.ipynb file
The WeatherPy_vacation.csv file
The WeatherPy_vacation_map.png image
The Vacation_Itinerary folder with the following:

The Vacation_Itinerary.ipynb file
The WeatherPy_travel_map.png image

How might we provide real-time suggestions for our client's ideal hotels? Your first task was to define what you meant by "ideal." So, over the course of the conversation, you narrowed that to hotels that were (1) within a given range of latitude and longitude and that (2) provided the right kind of weather for the client.

Basic Project Plan
Here's an outline of your project plan:
	•	Task: Collect and analyze weather data across cities worldwide.
	•	Purpose: PlanMyTrip will use the data to recommend ideal hotels based on clients' weather preferences.
	•	Method: Create a Pandas DataFrame with 500 or more of the world's unique cities and their weather data in real time. This process will entail collecting, analyzing, and visualizing the data.


Your analysis of the data will be split into three main parts, or stages.
	1	Collect the Data
	◦	Use the NumPy module to generate more than 1,500 random latitudes and longitudes.
	◦	Use the citipy module to list the nearest city to the latitudes and longitudes.
	◦	Use the OpenWeatherMap API to request the current weather data from each unique city in your list.
	◦	Parse the JSON data from the API request.
	◦	Collect the following data from the JSON file and add it to a DataFrame:
	▪	City, country, and date
	▪	Latitude and longitude
	▪	Maximum temperature
	▪	Humidity
	▪	Cloudiness
	▪	Wind speed
	2	Exploratory Analysis with Visualization
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
