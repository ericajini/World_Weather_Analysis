# World_Weather_Analysis


## Overview 

The purpose of this analysis was to pull 2000 random latitudes and longitude pairs using the Open Weather API, use this data to find favorable weather conditions for vacation and hotels close to these areas, and then use the Google Maps API to create the itinerary for 4 hotels in different cities within a country. 

### Weather DataBase

I started with creating a CSV database that is used throughout the rest of this analysis. This was done using 2000 random longitude and latitude pairs and pulling in the City, Country, Lat, Lng, Max Temp, Humidity, Cloudiness, Wind Speed, and the Current Description. 

![Weather DataBase](https://github.com/ericajini/World_Weather_Analysis/blob/main/weather_database.png)

### Vacation Search

During the Vacation Search part of this analysis, I refined the data I was pulling from the database by filtering out any cities that didn't match the criteria I set for Max Temp (70-80 degrees) and that didn't have a hotel that was found close by. There was also a new data frame created with the "Clean Data" where the null values were dropped and the criteria for max temp was re-applied. 

![Vacation Search](https://github.com/ericajini/World_Weather_Analysis/blob/main/Vacation_Search/WeatherPy_vacation_map.png)

### Vacation Itinerary 

During the Vacation Itinerary part of this analysis, I picked 4 cities close by in the same country that someone may want to go to on vacation. I picked Coahuayana, Lazaro Cardenas, Acapulco, Alpoyeca in MX. Using the Google API I created a travel map for the where there is the starting point, 3 additional stops, and then the ending point being the same place as the starting point. 

![Vacation Itinerary](https://github.com/ericajini/World_Weather_Analysis/blob/main/Vaction_Itinerary/WeatherPy_travel_map_markers.png)