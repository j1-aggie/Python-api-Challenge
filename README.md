# WeatherPy / VacationPy (Python API Challenge)

![image](https://user-images.githubusercontent.com/66078772/93265495-4e479a00-f76e-11ea-8e19-137c69cd3d02.png)

Background
Whether financial, political, or social -- data's true power lies in its ability to answer questions definitively. So we took what we have learned about Python requests, APIs, and JSON traversals to answer a fundamental question: "What's the weather like as we approach the equator?"
Now, I know what you may be thinking: "Duh. It gets hotter..."
But, if pressed, how would you prove it?


Before We Begin


Create a new repository for this project called python-api-challenge. Do not add this homework to an existing repository.


Clone the new repository to your computer.


Inside your local git repository, create a directory for both of the  Python Challenges. Use folder names corresponding to the challenges: WeatherPy.


Inside the folder that you just created, add new files called WeatherPy.ipynb and VacationPy.ipynb. These will be the main scripts to run for each analysis.


Push the above changes to GitHub.



Part I - WeatherPy
For part one, I created a Python script to visualize the weather of 500+ cities across the world of varying distance from the equator. To accomplish this, I utilized a simple Python library, the OpenWeatherMap API, and a little common sense to create a representative model of weather across world cities.
My first requirement is to create a series of scatter plots to showcase the following relationships:

* Temperature (F) vs. Latitude
* Humidity (%) vs. Latitude
* Cloudiness (%) vs. Latitude
* Wind Speed (mph) vs. Latitude

![Lat vs Cloudiness](https://user-images.githubusercontent.com/66078772/101796017-24ccaf00-3ace-11eb-9849-7b294f5d5c8f.png)
![Lat vs Humidity](https://user-images.githubusercontent.com/66078772/101796019-24ccaf00-3ace-11eb-8ebc-ae5a8cb9428e.png)
![Lat vs Temp](https://user-images.githubusercontent.com/66078772/101796020-25654580-3ace-11eb-922f-bcec38b7367e.png)
![Lat vs Wind Speed](https://user-images.githubusercontent.com/66078772/101796022-25654580-3ace-11eb-9c4b-644c870cdf2d.png)



After each plot add a sentence or too explaining what the code is and analyzing.
MY second requirement is to run linear regression on each relationship, only this time separating them into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude):

* Northern Hemisphere - Temperature (F) vs. Latitude
* Southern Hemisphere - Temperature (F) vs. Latitude
* Northern Hemisphere - Humidity (%) vs. Latitude
* Southern Hemisphere - Humidity (%) vs. Latitude
* Northern Hemisphere - Cloudiness (%) vs. Latitude
* Southern Hemisphere - Cloudiness (%) vs. Latitude
* Northern Hemisphere - Wind Speed (mph) vs. Latitude
* Southern Hemisphere - Wind Speed (mph) vs. Latitude

![Northern Hemispher Lat vs Humidity](https://user-images.githubusercontent.com/66078772/101796023-25654580-3ace-11eb-845c-3382b2462d2e.png)
![Northern Hemisphere Lat vs Cloudiness](https://user-images.githubusercontent.com/66078772/101796025-25654580-3ace-11eb-8ab5-1791d9e86409.png)
![Northern Hemisphere Lat vs Temp](https://user-images.githubusercontent.com/66078772/101796028-25fddc00-3ace-11eb-8a03-9045c7e4cc6c.png)
![Northern Hemisphere Lat vs Wind Speed](https://user-images.githubusercontent.com/66078772/101796029-25fddc00-3ace-11eb-8bef-cdfeb35d813d.png)
![Southern Hemisphere Lat vs Cloudiness](https://user-images.githubusercontent.com/66078772/101796030-25fddc00-3ace-11eb-9a48-1203676a9f51.png)
![Southern Hemisphere Lat vs Humidity](https://user-images.githubusercontent.com/66078772/101796031-25fddc00-3ace-11eb-8508-87724a47d970.png)
![Southern Hemisphere Lat vs Temp](https://user-images.githubusercontent.com/66078772/101796032-26967280-3ace-11eb-9014-dd47fd11711d.png)
![Southern Hemisphere Lat vs Windspeed](https://user-images.githubusercontent.com/66078772/101796033-26967280-3ace-11eb-97c9-fbec80b5f7ee.png)

After each pair of plots, I explained what the linear regression is modeling such as any relationships I have noticed and any other analysis I have.
MY final notebook will:

Randomly select at least 500 unique (non-repeat) cities based on latitude and longitude.
Perform a weather check on each of the cities using a series of successive API calls.
Include a print log of each city as it's being processed with the city number and city name.
Save a CSV of all retrieved data and a PNG image for each scatter plot.


Part II - VacationPy
For this part, I used my skills in working with weather data to plan future vacations. Use jupyter-gmaps and the Google Places API for this part of the assignment.


Created a heat map that displays the humidity for every city from the part I of the homework.


Narrowed down the DataFrame to find my ideal weather condition. For example:


A max temperature lower than 80 degrees but higher than 70.


Wind speed less than 10 mph.


Zero cloudiness.


Dropped any rows that don't contain all three conditions. Wanted to be sure the weather is ideal.


Used Google Places API to find the first hotel for each city located within 5000 meters of your coordinates.


Plotted the hotels on top of the humidity heatmap with each pin containing the Hotel Name, City, and Country.




Conclusions

After completing the weather py analysis using the citipy module to pull in 500 random cities, the conclusions that can be drawn are that:
  * Temperature seems to have a clear correlation with latitude. 
  * As expected, the weather becomes significantly warmer as you approach the equator. On average the southern hemisphere tends to be warmer than the northern hemisphere.  
  * There is no strong relationship between latitude and humidity. However, there is a slightly larger amount of northern hemisphere cities with higher humidity than cities in the southern hemisphere.

