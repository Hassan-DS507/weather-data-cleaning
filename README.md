# Data Cleaning Project

## Overview
This project focuses on cleaning and preprocessing raw data from different sources, including cities, countries, and daily weather datasets. The goal is to ensure the data is well-structured, consistent, and ready for further analysis.

## Dataset Information
This project utilizes the **Weather Dataset**, which provides comprehensive weather data for over 1200 cities worldwide. The dataset is updated weekly using data from the **Meteostat API**, ensuring fresh and accurate weather insights. The dataset includes historical weather data dating back to **January 2, 1833**, making it valuable for long-term climate analysis.

### **Cities DataFrame (`cities.csv`)**
This dataframe contains metadata about individual cities and weather stations.

**Columns:**
- `station_id`: Unique ID for the weather station.
- `city_name`: Name of the city.
- `country`: The country where the city is located.
- `state`: The state or province within the country.
- `iso2`: The two-letter country code.
- `iso3`: The three-letter country code.
- `latitude`: Latitude coordinate of the city.
- `longitude`: Longitude coordinate of the city.

### **Countries DataFrame (`countries.csv`)**
Provides geographic and demographic details about different countries.

**Columns:**
- `iso3`: The three-letter code representing the country.
- `country`: The English name of the country.
- `native_name`: The native name of the country.
- `iso2`: The two-letter code representing the country.
- `population`: The population of the country.
- `area`: The total land area of the country in square kilometers.
- `capital`: The name of the capital city.
- `capital_lat`: The latitude coordinate of the capital city.
- `capital_lng`: The longitude coordinate of the capital city.
- `region`: The specific region within the continent where the country is located.
- `continent`: The continent to which the country belongs.
- `hemisphere`: The hemisphere in which the country is located (e.g., Northern, Southern).

### **Daily Weather DataFrame (`daily_weather.parquet`)**
Stores daily weather records from weather stations worldwide.

**Columns:**
- `station_id`: Unique ID for the weather station.
- `city_name`: Name of the city where the station is located.
- `date`: Date of the weather record.
- `season`: Season corresponding to the date (e.g., summer, winter).
- `avg_temp_c`: Average temperature in Celsius.
- `min_temp_c`: Minimum temperature in Celsius.
- `max_temp_c`: Maximum temperature in Celsius.
- `precipitation_mm`: Precipitation in millimeters.
- `snow_depth_mm`: Snow depth in millimeters.
- `avg_wind_dir_deg`: Average wind direction in degrees.
- `avg_wind_speed_kmh`: Average wind speed in kilometers per hour.
- `peak_wind_gust_kmh`: Peak wind gust in kilometers per hour.
- `avg_sea_level_pres_hpa`: Average sea-level pressure in hectopascals.
- `sunshine_total_min`: Total sunshine duration in minutes.

## Project Workflow
1. **Loading Data**: The datasets are loaded into Pandas DataFrames.
2. **Data Exploration**: Checking the structure, missing values, and basic statistics.
3. **Data Cleaning**:
   - Handling missing values
   - Standardizing formats
   - Removing duplicates
   - Fixing inconsistent entries
4. **Data Export**: Saving cleaned data into new files for future analysis.

## Benefits of This Project
- **Data Accuracy**: Ensures the dataset is free from missing values and inconsistencies.
- **Enhanced Usability**: Cleaned data can be used for machine learning, visualization, and forecasting.
- **Historical Insights**: Useful for climate trend analysis and long-term weather predictions.
- **Scalability**: Ready to integrate with databases for larger-scale applications.

## Requirements
To run this project, install the following dependencies:
```sh
pip install -r requirements.txt
```

## Running the Project
Execute the Jupyter Notebook `data_cleaning.ipynb` step by step to perform the data cleaning process.

## Folder Structure
```
📂 Data_Cleaning_Project
├── data_cleaning.ipynb  # Main Jupyter Notebook
├── cities.csv           # Raw cities dataset
├── countries.csv        # Raw countries dataset
├── daily_weather.parquet # Raw weather dataset
├── requirements.txt     # Required Python libraries
├── .gitignore           # Files to ignore in Git
└── README.md            # Project Documentation
```

## Future Improvements
- Automate the cleaning process with scripts.
- Add visualization for better insights.
- Integrate with a database for scalable data storage.

## Author
Hassan Abdelrazek

