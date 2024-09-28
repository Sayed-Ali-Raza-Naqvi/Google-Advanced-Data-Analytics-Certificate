# Taxi Ride Analysis

## Overview
This project analyzes taxi ride data to extract meaningful insights and features. The dataset includes various attributes of taxi rides, including pickup and dropoff times, trip distances, fare amounts, and more. The analysis focuses on identifying patterns in the data, including rush hour trends and trip characteristics.

## Features
- **Data Cleaning and Preprocessing**: The dataset is cleaned by handling missing values, outliers, and erroneous entries.
- **Feature Engineering**: New features are derived from existing data, including:
  - **Duration**: The time taken for each ride.
  - **Mean Distance**: The average distance for each pickup/dropoff combination.
  - **Mean Duration**: The average duration for each pickup/dropoff combination.
  - **Rush Hour**: A binary indicator for whether a ride occurred during rush hours.
  - **Day and Month**: The day of the week and month extracted from pickup datetime.

## Data Analysis
The analysis involves:
- Generating summary statistics to understand the distribution of key features.
- Identifying outliers in features such as trip distance and fare amount.
- Visualizing distributions and relationships among features using box plots and other relevant charts.

## Requirements
- Python 3.x
- pandas
- NumPy
- Matplotlib (for visualization)
- statsmodels (for statistical modeling)
