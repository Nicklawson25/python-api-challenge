# WeatherPy and VacationPy Project

## Overview
This project is divided into two main parts: WeatherPy and VacationPy. The goal is to visualize weather data from over 500 cities around the world and then use this data to plan potential vacation destinations based on specific weather criteria.

## Part 1: WeatherPy

### Objective
Create a Python script to visualize the weather of over 500 cities of varying distances from the equator using the citipy Python library, the OpenWeatherMap API, and various Python programming techniques.

### Steps and Requirements

#### Requirement 1: Create Plots to Showcase the Relationship Between Weather Variables and Latitude
1. Use the OpenWeatherMap API to retrieve weather data for the list of cities generated in the starter code.
2. Create scatter plots to showcase the following relationships:
    - Latitude vs. Temperature
    - Latitude vs. Humidity
    - Latitude vs. Cloudiness
    - Latitude vs. Wind Speed

#### Requirement 2: Compute Linear Regression for Each Relationship
1. Compute linear regression for each of the relationships mentioned above.
2. Separate the plots into Northern Hemisphere (latitude >= 0) and Southern Hemisphere (latitude < 0).
3. Create scatter plots including:
    - Linear regression line
    - The model's formula
    - The R-squared values

The plots required are:
- Northern Hemisphere: Temperature vs. Latitude
- Southern Hemisphere: Temperature vs. Latitude
- Northern Hemisphere: Humidity vs. Latitude
- Southern Hemisphere: Humidity vs. Latitude
- Northern Hemisphere: Cloudiness vs. Latitude
- Southern Hemisphere: Cloudiness vs. Latitude
- Northern Hemisphere: Wind Speed vs. Latitude
- Southern Hemisphere: Wind Speed vs. Latitude

After creating each pair of plots, describe the linear regression model, any relationships noticed, and any other findings.

### How to Run WeatherPy
1. Open the `WeatherPy.ipynb` Jupyter notebook provided in the starter code.
2. Follow the guided steps to complete the required functionalities.
3. Use your API key for OpenWeatherMap and ensure all dependencies are installed.
4. Execute the cells in the notebook to generate the required plots and analyses.

## Part 2: VacationPy

### Objective
Use weather data skills to plan future vacations by creating map visualizations using Jupyter notebooks, the geoViews Python library, and the Geoapify API.

### Steps and Requirements

1. **Create a City Map**:
    - Display a point for every city in the `city_data_df` DataFrame. The size of the point should represent the humidity in each city.

2. **Filter for Ideal Weather Conditions**:
    - Narrow down the `city_data_df` DataFrame to find cities that match your ideal weather conditions. For example:
        - Max temperature between 21°C and 27°C
        - Wind speed less than 4.5 m/s
        - Zero cloudiness

3. **Find Hotels**:
    - Create a new DataFrame called `hotel_df` to store the city, country, coordinates, and humidity.
    - Use the Geoapify API to find the first hotel within 10,000 meters of each city's coordinates.
    - Add the hotel name and country as additional information in the hover message for each city on the map.

### How to Run VacationPy
1. Open the `VacationPy.ipynb` Jupyter notebook provided in the starter code.
2. Load the CSV file containing weather and coordinates data generated from Part 1.
3. Follow the guided steps to create the map visualizations.
4. Use your API key for Geoapify and ensure all dependencies are installed.
5. Execute the cells in the notebook to generate the required maps and analyses.

## Hints and Considerations
- Study the OpenWeatherMap and Geoapify APIs thoroughly to understand how to use them effectively.
- Use simple test cases to understand how the citipy library works before integrating it into your main script.
- Ensure that you cover a full range of latitudes and longitudes to avoid a biased dataset.
- Regularly commit your work to your repository and provide clear commit messages.
- Ensure your README file is comprehensive and provides clear instructions on how to run your scripts and interpret the results.

## Conclusion
This project will enhance your understanding of data analytics, API integration, and geographic data visualization. Completing this task will demonstrate your ability to handle complex data analysis and visualization tasks, setting a solid foundation for future data science projects.

Good luck!
