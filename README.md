# Bike Demand Forecasting

## Overview

This project analyzes bike-sharing demand using weather, calendar, and seasonal variables. The goal is to model hourly bike rental counts and evaluate how well count-based regression methods can forecast demand.

Bike-sharing systems face operational challenges because demand changes by hour, season, weather condition, temperature, humidity, and wind speed. Accurate demand forecasting can help improve bike allocation, staffing, and service availability.

## Dataset

The dataset includes bike rental observations with variables such as:

- Rental count
- Season
- Year, month, hour, weekday, and holiday indicators
- Weather situation
- Temperature and perceived temperature
- Humidity
- Wind speed

## Objectives

- Analyze factors associated with bike rental demand
- Prepare and clean bike-sharing data for modeling
- Build a Poisson Regression model for count-based demand forecasting
- Evaluate model accuracy using train/test splits and repeated sampling
- Diagnose model limitations such as multicollinearity and overdispersion

## Methodology

### Data Preparation

- Removed irrelevant identifier and leakage-related columns
- Converted categorical variables into model-ready predictors
- Split observations into training and testing sets

### Statistical Modeling

- Applied Poisson Regression to model bike rental count data
- Evaluated prediction accuracy using repeated random sampling
- Checked coefficient significance using subsampling
- Assessed multicollinearity using VIF
- Investigated overdispersion using residual diagnostics

### Evaluation Metrics

- Mean Squared Error (MSE)
- Mean Absolute Error (MAE)
- Mean Absolute Percentage Error (MAPE)
- Precision Measure (PM)

## Technologies Used

- Python
- Pandas
- NumPy
- Statsmodels
- Scikit-learn
- Matplotlib
- Seaborn
- Jupyter Notebook

## Skills Demonstrated

- Demand Forecasting
- Count Data Modeling
- Poisson Regression
- Regression Diagnostics
- Train/Test Evaluation
- Repeated Sampling
- Multicollinearity Analysis
- Overdispersion Analysis
- Exploratory Data Analysis

## Repository Files

- `bike_demand_forecasting.ipynb` — Main analysis notebook
- `bikes.csv` — Bike-sharing demand dataset
- `requirements.txt` — Python dependencies
- `README.md` — Project documentation
- `LICENSE` — MIT License

## Future Improvements

- Add Negative Binomial Regression to better handle overdispersion
- Compare Poisson Regression with tree-based machine learning models
- Add visualizations for hourly, seasonal, and weather-based demand patterns
- Organize final model outputs and charts into a report folder
