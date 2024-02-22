
![App Screenshot](https://www.dataiku.com/wp-content/uploads/2020/04/OpenWeather.png)

# Open Weather Map - Explorative Data Analysis

This project utilizes the OpenWeatherMap API to collect weather forecast data for various cities, performs exploratory data analysis (EDA) on the collected data, and visualizes insights using Python libraries such as Pandas, Matplotlib, Seaborn, and Plotly.


## Project Overview

The project involves the following key steps:

1. Importing necessary libraries for data manipulation, visualization, and API requests.
2. Fetching weather data for multiple cities using the OpenWeatherMap API.
3. Extracting relevant information from the API response and structuring it into a DataFrame.
4. Conducting exploratory data analysis to derive insights and patterns from the weather data.
5. Visualizing the findings through various plots and charts.
6. Saving the cleaned data to a CSV file for further analysis or visualization in tools like Tableau.
## File Structure

* cities.csv: Contains a list of city names for which weather data is to be fetched.
* OpenWeatherMap_cleanedData.csv: Cleaned data saved after the EDA process.
* OpenWeatherMap_EDA.ipynb: Jupyter Notebook containing the Python code for data fetching, analysis, and visualization.
* ReadMe.md: Markdown file providing an overview of the project.

## Libraries Used

- requests: For making HTTP requests to the OpenWeatherMap API.
- datetime: For handling date and time operations.
- pandas: For data manipulation and analysis.
- matplotlib and seaborn: For data visualization.
- plotly: For interactive visualization.
- json_normalize: For flattening JSON objects into a DataFrame.

## How to Run

1. Ensure you have the necessary Python libraries installed (you can install them via pip).
2. Obtain an API key from OpenWeatherMap and replace "YOUR_API_KEY" with your actual API key in the code.
3. Run the Jupyter Notebook OpenWeatherMap_EDA.ipynb to execute the code and perform EDA on weather data.
4. Explore the generated visualizations and insights within the notebook.
5. Optionally, you can save the cleaned data to OpenWeatherMap_cleanedData.csv for further analysis or visualization in external tools.
## API Reference

#### API for retrieving information City wise

```http
  f"http://api.openweathermap.org/data/2.5/weather?q={city}&appid={API_KEY}&units=metric"
```
#### API for retrieving information by Latitute and Longitude

```http
  f"http://api.openweathermap.org/data/2.5/forecast?lat={city['lat']}&lon={city['lon']}&appid={API_KEY}&units=metric"
```

This project is implemented by using these two free API by OpenWeatherMap. 

You can explore more API's at https://openweathermap.org/api 

This is the URL where the used API's and API_KEY generated https://openweathermap.org/price#weather with detailed step by step process.

## Visualizations

The project generates various visualizations, including histograms, scatter plots, line plots, and geospatial plots, to explore relationships and patterns within the weather data.


