# python-api-challenge

## Part 1- WeatherPy

For this project, the OpenWeatherMap API was used to retrieve weather data for the cities provided. The cities weather data was converted into a DataFrame 'city_data_df' and saved as a csv.  Next, I created a series of scatterplots to display the realationships between Latitude vs. Temperature, latitude vs. Humidity, Latitude vs. Cloudiness, and Latitude vs. Wind Speed.

Then, a series of scatterplots computing the linear regression for each relationship for nothern and southern hemispheres were created. This was done by creating plot variables for northern and southern hemispheres. A function for the linear regression plot was created to make the process less tedious. The scatter plots include the linear regression line, the model's formula, and the r value. 


## Part 2- VacationPy

In this section of the project, the geoViews Python library and the Geoapify API were used. They are both used to create map vizualizations. 

First, a map that displays a point for every city in the city_data_df DataFrame was created by loading the csv file created in part 1. the size of the point corresponds to the humidity in each city. 

Next, a new DataFrame was created for my ideal weather conditions, and that was copied into hotel_df. and another column named 'Hotel Name' was added to the hotel_df DataFrame. 

Then, some parameters were set and the request was made to "https://api.geoapify.com/v2/places" to find the hotels for the specific cities in the DataFrame. 

Lastly, another map was created with the ideal places plotted and the hotel name and country added to the hover message.
