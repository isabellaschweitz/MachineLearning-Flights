# Southwest Airlines Arrival Delay Prediction

## Project Overview

This project investigates the predictability of arrival delays for Southwest Airlines' commercial flight operations in the United States. Using a historical flight dataset, we developed and compared machine learning models (Linear Regression, Random Forest, and XGBoost) to forecast arrival delays in minutes.

The primary research questions addressed are:
1. How accurately do pre-flight features (e.g., schedule, route) forecast Southwest Airlines’ arrival delay?
2. How accurately does combining pre-flight and in-flight data (e.g., departure delay, taxi-out time) forecast Southwest Airlines’ arrival delays?

The analysis demonstrates that while pre-flight data alone offers limited predictive power (R² ≈ 0.07), accuracy significantly improves when in-flight operational data is included (R² ≈ 0.93). This highlights the critical importance of real-time operational data for effective delay prediction.

## Course Information

This project was submitted as part of the final requirements for the **KAN-CDSCO2004U  Machine Learning and Deep Learning** course at Copenhagen Business School (CBS) during the Spring 2025 semester.

## Dataset

The data used for this project originates from the U.S. Department of Transportation, covering domestic airline operations. A combined dataset from Kaggle, bundling flight data from January 2019 to August 2023, was utilized. For this analysis, the data was filtered to include only Southwest Airlines.

**Link to Kaggle Dataset:** [Flight Delay and Cancellation Dataset (2019-2023)](https://www.kaggle.com/datasets/patrickzel/flight-delay-and-cancellation-dataset-2019-2023/versions/6)


## Methodology Highlights

- **Data Source:** U.S. Department of Transportation (via Kaggle)
- **Airline Focus:** Southwest Airlines
- **Time Period:** January 2019 - August 2023
- **Target Variable:** Arrival Delay (in minutes)
- **Key Feature Sets Compared:**
    - Pre-flight features (available before departure)
    - Combined pre-flight and in-flight features (including data available after departure)
- **Models Used:** Dummy Regressor (baseline), Linear Regression, Random Forest, XGBoost
- **Techniques:** Exploratory Data Analysis (EDA), Feature Engineering (cyclic encoding, mean target encoding, `is_covid` flag), Data Preprocessing (scaling, pipelines), Hyperparameter Tuning (RandomizedSearchCV with TimeSeriesSplit for XGBoost), Model Evaluation (RMSE, MAE, R²).
- **Software:** Python (Pandas, NumPy, Scikit-learn, XGBoost, Matplotlib, Seaborn, Statsmodels) implemented in a Jupyter Notebook.

## Repository Structure

- 'ML-FinalExam-Master.ipynb': Jupyter Notebook containing all data preprocessing, EDA, model training, and evaluation code.
- 'README.md': This file.

---

Disclaimer: This ReadMe file is not part of the exam submission. 
