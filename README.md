# World_Weather_Analysis

##I am recommended to add a few changes on the PlanMyTrip app which are followings:

  -adding the weather description to the weather data
  
  -adding user input to filter the data for their weather preferences and identify the travel destinations 
  
  -creating the travel route between the four cities chosen by the beta tester and create the travel itenerary with marker layer map

##Results:

I input min 75F and max 95F in the user input field when filtering the weather data. Majority of cities that stay on dataframe as potential destination are located in Southern hemisphere or close to the equator. This is because the weather data was pulled on mid October and many cities in Nothern hemisphere are filtered out based on the current temperature. Also, we need to be aware that some city temperature swing so much by one day. The user may receive a different result set depending on the timing.  

[Vacation_Search_Map](https://github.com/Yunaka1269/World_Weather_Analysis/blob/main/Vacation_Search/WeatherPy_vacation_map.PNG)

[Vacation_Travel_Map](https://github.com/Yunaka1269/World_Weather_Analysis/blob/main/Vacation_Itinerary/WeatherPy_travel_map.PNG)

[Travel_Map_Marker](https://github.com/Yunaka1269/World_Weather_Analysis/blob/main/Vacation_Itinerary/WeatherPy_travel_map_markers.PNG)

###Resources

- Software: Jupyter Notebook 6.1.4
- Weather Map API:
  - url = "http://api.openweathermap.org/data/2.5/weather?units=Imperial&APPID="
- Google Directions API:
  - base_url = "https://maps.googleapis.com/maps/api/place/nearbysearch/json"

###Module Error

- module was not found by Jupyter Notebook though it is in the folder

	-import import_ipynb
		-this didn't fix issue
		
	-import os
	
	-os.getcwd()
		-to display current path
		
	-import sys
	
	-sys.path.append("folder directory")
		-change the file path


##Summary:

Business recommendation that I could offer to improve the PlanMyTrip app are
- add seasonality and get average weather or temperatuer of week/month of city to prevent unnecessary filtering 
- add more than one recommended hotel and enable the direct link to hotel website
- add trip duration information in Travel Itinerary Map  
