# Python API Challenge

This analysis involved pulling city information from citipy, pulling weather information from the Open Weather API, and using the Google Places API to search for hotels within distance of a curated vacation spot list.


## Background

The first part of the analysis is saved in the WeatherPy file.  After creating a random list of latitude and longitudes (spanning the globe), these were referencced against a list of cities and coordinates (using citipy).  From there, an Open Weather API pull was performed for each city.  The output included details on current weather conditions.  This information was captured in a dataframe and analyzed.  The resulting output are visualizations representing key weather relationships, demonstrating that the weather generally gets hotter closer to the equator and cooler the closer to the poles.  However, there is a seasonality effect.  Currently, the Northern Hemisphere is in winter and the Southern Hemisphere is in summer.  The results will look somewhat different based on the time of the year. These output charts are saved in the WeatherPy folder.

The second part of the analysis incorporates the weather data by city.  A heatmap was created reflecting all of the locations determined by weather, with heatmap intensity changing based on humidity levels. This list is narrowed down to create a list of ideal vacation spots, based on desired weather conditions:
* Humidity less than or equal to 50%
* Max Temperature between 65F and 75F
* Cloudiness <10%

Using the Google Places API, Hotels (lodging) within 5000 meters were isolated.  The first observations were included and marked on the heatmap, which reflects the humidity levels of all selected (500+) locations.



