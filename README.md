# Air Quality Prediction & Analysis

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python&logoColor=white)
![Status](https://img.shields.io/badge/Status-In%20Progress-yellow)

## Project Overview
This project is an end-to-end Data Science pipeline designed to analyze environmental sensor data and predict the **Air Quality Index (AQI)**. 

The goal is to investigate how various pollutants (CO, NOx, Ozone, PM2.5) and weather conditions (Temperature, Humidity, Wind) influence air quality, and subsequently build a Machine Learning model to forecast AQI levels.

## Key Objectives
* **Exploratory Data Analysis (EDA):** Visualizing distributions of pollutants using Boxplots and Violin plots to identify outliers and trends.
* **Data Preprocessing:** Handling missing values, feature scaling (`StandardScaler`), and preparing time-series data.
* **Feature Engineering:** Creating pollutant ratios and moving averages to improve model sensitivity.
* **Machine Learning (In Progress):** Training regression/classification models to predict AQI based on sensor inputs.

## Tech Stack
* **Core:** Python 3.x
* **Data Manipulation:** Pandas, NumPy
* **Visualization:** Matplotlib, Seaborn
* **Machine Learning:** Scikit-Learn (preprocessing, model selection)

## Dataset Structure
The project utilizes the `AirQualityData.csv` dataset, which includes:
* **Pollutants:** Carbon Monoxide (`CO`), Nitrogen Oxides (`NOx`, `NO2`), Ozone (`O3`), Sulfur Dioxide (`SO2`), Particulates (`PM2.5`, `PM10`).
* **Weather:** Temperature, Humidity, Pressure, Wind Speed & Direction.
* **Target:** `AirQualityIndex`.

## Project Workflow
1.  **Data Ingestion:** Loading raw CSV data.
2.  **EDA:** * Statistical summary of features.
    * Visual inspection of pollutant spreads (using green-filled boxplots for clarity).
3.  **Preprocessing:** * Standardizing features (Mean=0, Std=1) for optimal model performance.
    * Splitting data into Training and Testing sets.
4.  **Modeling (Upcoming):** * Implementation of algorithms such as **Linear Regression**, **Random Forest**, or **XGBoost**.
    * Model evaluation using RMSE and R² metrics.

## Repository Contents
* `air_quality.ipynb`: The main Jupyter Notebook containing the analysis, visualization code, and ML pipeline.
* `AirQualityData.csv`: The dataset used for training and testing.
* `README.md`: Project documentation.

## Visualizations
The project places a strong emphasis on data understanding. Below is an example of the distribution analysis logic used in the notebook:

```python

Example of visualization logic used in the notebook
...
```

## Future Work
* Train and tune a Random Forest Regressor.

* Evaluate model performance on the test set.

* Deploy the model as a simple API or Streamlit web app.

## Created by Marta Golka
