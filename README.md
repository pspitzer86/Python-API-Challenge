# Python-API-Challenge

Using a pre-made section of code and the CitiPy module, approx 550-700 cities throughout the world were randomly pulled and put into a list.  An API Key was created through the OpenWeather API website which provided the current days weather data for most cities across the world.  Using the base url for this weather API, a json was created from the weather data and each of the names of the random cities pulled from CitiPy was looped through the json.  If a city was not found in the API, it was printed in the log that it was not found.  If a city was found in the json, their city id and name were printed in the log as found, then the city name was sent to a new list and various weather data was pulled from the json and put into empty lists for each of the cities found.  These usually left us with a little over 500 cities.  The data pulled included Max Temperature, Cloudiness, Humidity, Wind Speed, and Latitude and Longitude coordinates.  The data was then organized into a dataframe.  The data pulled was then plotted into several scatter plots as follows:

Latitude vs. Max Temperature
Latitude vs. Humidity
Latitude vs. Cloudiness
Latitude vs. Wind Speed

Analysis was done on the resulting graphs to see if any patterns or trends could be seen.  The dataframe was then separated into two separate dataframes based on latitude, one for cities found in the Northern Hemisphere and the other for cities found in the Southern Hemisphere.  A function was created that would create a scatter plot as well as calculate the linear regression for the data, plot the line in the scatter plot and annotate it.  Eight scatter plots with their linear regression were created with similar comparisons to earlier, just separated by hemisphere.  The graphs are as follows:

Latitude vs. Max Temperature - Northern Hemisphere
Latitude vs. Max Temperature - Southern Hemisphere
Latitude vs. Humidity - Northern Hemisphere
Latitude vs. Humidity - Southern Hemisphere
Latitude vs. Cloudiness - Northern Hemisphere
Latitude vs. Cloudiness - Southern Hemisphere
Latitude vs. Wind Speed - Northern Hemisphere
Latitude vs. Wind Speed - Southern Hemisphere

A csv of the cities and their weather data was created in this first section to be used in the second section of this assignment.  A google maps API key was created in order to create a google map based on the data.  A heatmap layer was created based on the humidity for each city and was plotted onto the google map base map.  Using parameters for max temperature, wind speed, humidity, and cloudiness, ideal weather conditions for potential vacation spots were set and shortened the dataframe to less than 10 cities.  The google api was then used to find hotels within 5000 meters of each of these cities now designated as vacation spots.  A marker layer was created with these coordinates that included the country, city name, and the name of the hotel found if there was one.  The marker layer was added to the map and culd be clicked on to show the data for the area.
