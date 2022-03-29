# World_Weather_Analysis
## Overview
PlanMyTrip is a travel technology company that specializes in internet related services in the Hotel and Lodging industry. To improve utilization of the app, the board has recommended adding the weather description to all relevant weather data when traveling. Using input statements to filter the data for their weather preferences, we can identify potential travel destinations and nearby hotels. From the list of potential travel destinations, anyone can choose four cities to create a travel itinerary. Finally, using the Google Maps Directions API, we have created a travel route between the four cities as well as a marker layer map.

## Resources for the Analysis
* **CSV Files:** 
[Weather_Database.csv]( https://github.com/Roark23/World_Weather_Analysis/blob/main/Weather_Database/WeatherPy_Database.csv), 
[WeatherPy_vacation.csv]( https://github.com/Roark23/World_Weather_Analysis/blob/main/Vacation_Search/WeatherPy_vacation.csv)
* **Jupyter Notebook Files:**: 
[Weather_Database.ipynb]( https://github.com/Roark23/World_Weather_Analysis/blob/main/Weather_Database/Weather_database.ipynb), 
[Vacation_Search.ipynb](https://github.com/Roark23/World_Weather_Analysis/blob/main/Vacation_Search/Vacation_Search.ipynb),
[Vacation_Itinerary.ipynb]( https://github.com/Roark23/World_Weather_Analysis/blob/main/Vactaion_Itinerary/Vacation_Itinerary.ipynb)
* **Python**: Python v3.7.6, Dependencies: Pandas, Matplotlib, CitiPy, SciPy, Python Requests, APIs, JSON Traversals

## Deliverable 1
### Retrieving Weather Data
I generated a set of 2,000 random latitudes and longitudes to retrieve the nearest city and perform an API call with the OpenWeatherMap. Using an API call to retrieve the current weather description for each city, we can create a new DataFrame containing the updated weather data.

[Weather_Database.csv]( https://github.com/Roark23/World_Weather_Analysis/blob/main/Weather_Database/WeatherPy_Database.csv)

This is a snapshot of the first random 10 cities generated:

![List of Random Cities and Weather Data](/Weather_Database/List of Random Cities Weather Data.png)

## Deliverable 2
### Creating a Customer Travel Destinations Map
Through using input statements to retrieve customer weather preferences, we can then use those preferences to identify potential travel destinations and nearby hotels. I have identified some potential destinations on a marker layer map with pop-up markers.

#### Potential Travel Destinations
After inputting preferences related to current temperatures of various cities, we have identified some potential travel destinatoins:

![Potential Destinations Based on Weather Preference](/Vacation_Search/WeatherPy_vacation_map.png)

Each marker shows a city and their relevant weather inforamtion along with a hotel for a potential travel destination:

![Potential Hotels for Each Destination](/Vactaion_Itinerary/WeatherPy_travel_map_markers.png)

## Deliverable 3
### Travel Itinerary
I used the Google Directions API to create a travel itinerary that shows the route between four cities chosen from the customer’s possible travel destinations. I also created a marker layer map with a pop-up marker for each city on the itinerary. This could be easily re created for any travel destination based on customer preference.

![Travel Itinerary for Potential Destinations](/Vactaion_Itinerary/WeatherPy_travel_map.png)

Each city also has their relevant weather information listed along with a hotel:

![Potential Hotels for Each Destination](/Vactaion_Itinerary/WeatherPy_travel_map_markers.png)