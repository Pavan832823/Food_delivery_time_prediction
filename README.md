# Food Delivery Time Prediction

This repository contains a Jupyter Notebook for predicting food delivery times based on various factors such as distance, delivery person attributes, and order details.

## Project Overview

The goal of this project is to analyze and predict the time taken for food delivery using a dataset that includes:

- Delivery person attributes (age, ratings)
- Restaurant and delivery location coordinates
- Type of order and vehicle
- Calculated distance between restaurant and delivery location

## Key Features

1. **Data Exploration**: Initial analysis of the dataset structure and contents.
2. **Data Cleaning**: Checking for missing values and inconsistencies.
3. **Feature Engineering**: Calculating delivery distances using the Haversine formula.
4. **Visualization**: Scatter plot showing the relationship between distance and delivery time.
5. **Trend Analysis**: OLS trendline to visualize the correlation between distance and time taken.

## Dataset

The dataset (`deliverytime.txt`) contains 45,593 entries with the following columns:

- `ID`: Unique identifier for each delivery
- `Delivery_person_ID`: Identifier for the delivery person
- `Delivery_person_Age`: Age of the delivery person
- `Delivery_person_Ratings`: Ratings of the delivery person
- `Restaurant_latitude`, `Restaurant_longitude`: Coordinates of the restaurant
- `Delivery_location_latitude`, `Delivery_location_longitude`: Coordinates of the delivery location
- `Type_of_order`: Category of the order (e.g., Snack, Drinks)
- `Type_of_vehicle`: Vehicle used for delivery
- `Time_taken(min)`: Target variable - time taken for delivery in minutes

## Distance Calculation

The notebook includes a function to calculate the distance between restaurant and delivery locations using the Haversine formula, which accounts for the curvature of the Earth.

## Visualization

A scatter plot with an OLS trendline is generated to explore the relationship between distance and delivery time, providing insights into how these variables correlate.

## Usage

1. Clone the repository.
2. Ensure you have the required libraries installed (pandas, numpy, plotly.express).
3. Run the Jupyter Notebook to see the analysis and visualizations.

## Future Work

Potential extensions for this project include:
- Building a predictive model for delivery time
- Incorporating additional features like traffic data or weather conditions
- Analyzing the impact of delivery person ratings and age on delivery time

Feel free to contribute or suggest improvements!
