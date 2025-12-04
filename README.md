<div align="center">

# 🌿 Air Quality Pulse
### End-to-End Environmental Data Analysis & Prediction Pipeline

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?style=for-the-badge&logo=python&logoColor=ffdd54)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black)

<br />

**[ Explore the Notebook ](air_quality.ipynb) • [ View the Data ](AirQualityData.csv) • [ Report Bug ](issues)**

</div>

---

## Project Overview
**Air Quality Pulse** is a Data Science project designed to analyze environmental sensor data and predict the **Air Quality Index (AQI)**.

Pollution is an invisible threat. This project moves beyond simple data reading to translate raw sensor inputs into actionable insights. By investigating how pollutants (like CO, NOx, PM2.5) interact with weather conditions, we aim to build a robust Machine Learning model to forecast air quality levels.

## Repository Contents
* **`air_quality.ipynb`**: The core Jupyter Notebook containing the full analysis pipeline: data loading, cleaning, visualization, and modeling.
* **`AirQualityData.csv`**: The dataset containing historical air quality measurements and engineered features.
* **`README.md`**: Project documentation.

## The Data "Story"
The dataset captures the complex relationship between chemical pollutants and atmospheric conditions. Key features include:

* **Pollutants:** Carbon Monoxide (`CO`), Nitrogen Oxides (`NOx`, `NO2`), Ozone (`O3`), and Particulates (`PM2.5`, `PM10`).
* **Weather:** Temperature, Humidity, Pressure, Wind Speed & Direction.
* **Engineered Features:** Moving averages (e.g., `CO_MA3`) to capture trends, and pollutant ratios.
* **Target:** `AirQualityIndex` (AQI).

## Visual Insights
*A picture is worth a thousand rows of data.* We emphasize data understanding through visualization. For example, we use **Green Boxplots** to inspect the spread of pollutants. This specific visualization helps in quickly identifying extreme outliers (black diamonds) against the median distribution, which is crucial for data cleaning.

>
> *Figure 1: Distribution of key pollutants showing outliers and spread.*

## ⚙️ Tech Stack & Methods

| Component | Technology | Description |
| :--- | :--- | :--- |
| **Data Processing** | Pandas, NumPy | Cleaning, Lag Features, Rolling Averages |
| **Visualization** | Seaborn, Matplotlib | Custom Boxplots, Heatmaps, Time-Series Analysis |
| **Preprocessing** | Scikit-Learn | `StandardScaler` (Mean=0, Std=1), `train_test_split` |
| **Modeling** | *In Progress* | Regression Analysis (Linear, Random Forest) |

##  How to Run
To replicate this analysis on your local machine:

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/marta23-10/air-quality-pulse.git](https://github.com/marta23-10/air-quality-pulse.git)
    cd air-quality-pulse
    ```
2.  **Install required libraries:**
    ```bash
    pip install pandas numpy matplotlib seaborn scikit-learn
    ```
3.  **Launch Jupyter Notebook:**
    ```bash
    jupyter notebook air_quality.ipynb
    ```

##  Project Roadmap
This project follows a structured data science lifecycle:

- [x] **Phase 1: Data Ingestion & Cleaning**
    - Handling missing values and formatting timestamps.
- [x] **Phase 2: Exploratory Data Analysis (EDA)**
    - Distribution analysis using Boxplots plots.
    - Correlation analysis.
- [x] **Phase 3: Preprocessing**
    - Feature standardization using `StandardScaler`.
    - Splitting data into Training and Testing sets.
- [ ] **Phase 4: Predictive Modeling**
    - Training Regression models (Random Forest, XGBoost).
    - Evaluating performance (RMSE, R²).

##  Contributing
Contributions are welcome! If you have ideas for better feature engineering or new models:
1.  Fork the repo.
2.  Create your feature branch.
3.  Submit a Pull Request.

---
<div align="center">
    <p><i>Created by Marta Golka</i></p>
</div>
