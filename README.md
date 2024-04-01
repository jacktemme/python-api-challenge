Module 6 Challenge

This repository contains two Jupyter Notebook files that access the Open Weather Api and the Geoapify Api. The WeatherPY file randomly selects 614 cities and finds weather data about this city. Then the relationship between different attributes of the weather and the latitude of the cities is anaylzed for linear regression models. The cities sampled and the scatterplots of this data can be found in the output folder. The VactionPy file uses the csv of sampled cities to  filter the cities by desirable weather traits for travel. Then the Geoapify Api is used to find the closest hotel to the coordinates of the city. These cities are plotted using hvplot and the hotel and weather information can be found by hovering over the city on the plotted map.

Making requests to the Open weather api utilized this website to create a query url with endpoints that would allow weather data on each city to be pulled in json.

https://openweathermap.org/current

This website was referenced to create the query url in order to find hotels near each city by utilizing its latitude and longitude.

https://apidocs.geoapify.com/docs/places/#about

Then chat gpt was used on how to output certain variables from the linear regress function, and then how to call them in another section of code

to output:

   return regress_values, line_fit, rvalue

to call:

  regress_values, line_fit, rvalue = regress(x, y)

And this site was referenced to save a hvplot: 

https://hvplot.holoviz.org/user_guide/Viewing.html

   hvplot.save(plot, 'test.html')
