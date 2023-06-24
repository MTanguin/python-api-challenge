#### "Analyzing Weather Patterns and Latitude Relationships"

Application Programming Interface (API)| JavaScript Object Notation (JSON) | Using API key | Try & Except | Linear Regression | For loop  | Statistics

# Background

Weather is a fascinating and dynamic aspect of our environment, and its relationship with latitude can offer valuable insights. In this project, we aim to explore the connection between weather variables and the proximity to the equator. By analyzing weather data from over 500 cities across different latitudes, we can gain a better understanding of how temperature, humidity, cloudiness, and wind speed vary as we approach or move away from the equator.

To accomplish this, we utilize the citipy Python library to obtain the nearest city based on randomly generated geographic coordinates. We then leverage the OpenWeatherMap API to retrieve real-time weather data for these cities. Through data visualization and statistical analysis, we can visualize and quantify the relationships between latitude and various weather variables.

In addition to exploring these relationships, we employ linear regression analysis to provide further insights. By separating the cities into the northern and southern hemispheres, we can observe how the relationships between latitude and weather variables differ between these regions.

# Methods

### Part 1: WeatherPy

In WeatherPy, we generate scatter plots to showcase the relationships between latitude and weather variables. We obtain weather data from the OpenWeatherMap API for the cities in our dataset and create the following scatter plots:

- Latitude vs. Temperature
- Latitude vs. Humidity
- Latitude vs. Cloudiness
- Latitude vs. Wind Speed

To further analyze these relationships, we compute linear regression for each plot. By dividing the dataset into the northern and southern hemispheres, we generate additional scatter plots with linear regression lines. The linear regression analysis helps us understand the correlation between latitude and weather variables in each hemisphere.

### Part 2: VacationPy

In VacationPy, we shift our focus to using the obtained weather data to plan future vacations. Using the Geoapify API and the geoViews Python library, we create map visualizations to aid in decision-making. The key steps involved are:

1. Creating a map displaying a point for every city in the dataset, with the size of each point representing the humidity level.
2. Narrowing down the cities based on desired weather conditions, such as maximum temperature, wind speed, and cloudiness.
3. Utilizing the Geoapify API to find hotels near the chosen coordinates for each city.
4. Constructing a new DataFrame, hotel_df, to store relevant information about the hotels.
5. Adding the hotel name and country as additional details in the hover message for each city on the map.

By combining weather data, geographical information, and hotel details, VacationPy facilitates the selection of ideal vacation destinations based on desired weather conditions and available accommodations.

Please refer to the respective Jupyter notebooks, WeatherPy.ipynb and VacationPy.ipynb, for the step-by-step implementation of these methods.

# Deliverables

- WeatherPy.ipynb: Jupyter notebook containing the code for data retrieval, visualization, and analysis of weather data.
- VacationPy.ipynb: Jupyter notebook demonstrating the usage of geoViews and Geoapify API to plan vacations based on desired weather conditions and hotel availability.

# Results

### WeatherPy

![City Latitude vs Max Temperature](https://github.com/MTanguin/python-api-challenge/assets/114210481/26b51109-0199-47a8-a834-85850df85538)

![City Latitude vs Humidity](https://github.com/MTanguin/python-api-challenge/assets/114210481/fc07b38f-a11b-4c64-9a49-65093598fd02)

![City Latitude vs Cloudiness](https://github.com/MTanguin/python-api-challenge/assets/114210481/8b0f8d04-7b24-4733-b122-c983f63eed2d)

![City Latitude vs Wind Speed (mph)](https://github.com/MTanguin/python-api-challenge/assets/114210481/64ca448f-ea9e-4075-b417-fa68d457358e)

![Northern Hemisphere - Max Temp vs Latitude Linear Regression](https://github.com/MTanguin/python-api-challenge/assets/114210481/f10f8c7b-2d8e-46df-81ad-d9ba7568c670)

![Southern Hemisphere - Max Temp vs Latitude Linear Regression](https://github.com/MTanguin/python-api-challenge/assets/114210481/a69c14e4-7e83-40bb-b98d-e6c9afb23ab0)

![Northern Hemisphere - Humidity (%) vs Latitude Linear Regression](https://github.com/MTanguin/python-api-challenge/assets/114210481/81047655-dc9b-4979-999a-4509ad07fbe9)

![Southern Hemisphere - Humidity (%) vs Latitude Linear Regression](https://github.com/MTanguin/python-api-challenge/assets/114210481/0180310f-ae65-4da7-b1f5-dd510854391b)

![Northern Hemisphere - Cloudiness (%) vs Latitude Linear Regression](https://github.com/MTanguin/python-api-challenge/assets/114210481/c4c203f5-3268-477e-bbb7-88b03bdffa99)

![Southern Hemisphere - Cloudiness (%) vs Latitude Linear Regression](https://github.com/MTanguin/python-api-challenge/assets/114210481/4cd41f26-c50d-436f-8811-7758a8db55fc)

![Northern Hemisphere - Wind Speed vs Latitude Linear Regression](https://github.com/MTanguin/python-api-challenge/assets/114210481/1e380614-1828-4167-9f26-ec785d4bea7a)

![Southern Hemisphere - Wind Speed vs Latitude Linear Regression](https://github.com/MTanguin/python-api-challenge/assets/114210481/bd23f2c6-24d7-49a8-a05e-a136ea00c799)

### VacationPy

![Fig1](https://github.com/MTanguin/python-api-challenge/assets/114210481/2ed48832-4709-4ff5-b4fe-ccc697dcf34d)

![Fig2](https://github.com/MTanguin/python-api-challenge/assets/114210481/fb0f50a8-e61f-483c-9a35-3084f18cd428)

![Fig3](https://github.com/MTanguin/python-api-challenge/assets/114210481/50ac27fa-00c5-4666-b12b-2ec1b9c22176)

![Fig4](https://github.com/MTanguin/python-api-challenge/assets/114210481/1f9b66da-a6da-47c4-9118-69f4b9cbe81e)

# Conclusion

Through this project, we aim to uncover meaningful insights regarding the relationship between weather variables and latitude. By visualizing and analyzing the data, we can observe how temperature, humidity, cloudiness, and wind speed change with proximity to the equator. These findings can contribute to our understanding of weather patterns and support informed decision-making for future travel plans.

Note: The starter code and necessary dependencies are provided in the respective Jupyter notebooks.


Source:
https://courses.bootcampspot.com/courses/2799/assignments/42949?module_item_id=802979
