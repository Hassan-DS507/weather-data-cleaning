# Data Cleaning Project

## Overview
This project focuses on cleaning and preprocessing raw data from different sources, including cities, countries, and daily weather datasets. The goal is to ensure the data is well-structured, consistent, and ready for further analysis.

## Dataset Information
- **cities.csv**: Contains data about various cities, including population, geographical information, and more.
- **countries.csv**: Provides details about different countries, such as GDP, population, and economic indicators.
- **daily_weather.parquet**: Stores daily weather records, including temperature, humidity, and other meteorological data.

## Project Workflow
1. **Loading Data**: The datasets are loaded into Pandas DataFrames.
2. **Data Exploration**: Checking the structure, missing values, and basic statistics.
3. **Data Cleaning**:
   - Handling missing values
   - Standardizing formats
   - Removing duplicates
   - Fixing inconsistent entries
4. **Data Export**: Saving cleaned data into new files for future analysis.

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

