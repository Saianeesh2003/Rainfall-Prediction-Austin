# Rainfall-Prediction-Austin

This project uses historical weather data from Austin to:

1. **Predict how much it will rain (inches)** – *Regression problem*  
2. **Predict whether it will rain or not** – *Classification problem*

Both tasks are built using **Python** and **scikit-learn**, with a clean preprocessing pipeline and model evaluation.
## 🔍 Dataset

- File: `austin_weather.csv`
- Source: Public Austin weather data (daily level)
- Target column:
  - `PrecipitationSumInches` – total rainfall in inches

### Important preprocessing steps

- Replace `"T"` (trace precipitation) with a small value: `0.005`
- Replace `"-"` with `0.0`
- Convert numeric-like string columns to `float`
- Create a binary rain label:
  - `RainTomorrow = 1` if `PrecipitationSumInches > 0`
  - `RainTomorrow = 0` otherwise


## 🧠 Project Objectives

1. **Regression task**  
   Predict `PrecipitationSumInches` (continuous rainfall amount in inches).

2. **Classification task**  
   Predict `RainTomorrow` (1 = rain, 0 = no rain).

## 🏗️ Tech Stack

- Python 
- pandas  
- numpy  
- scikit-learn  

📊 Model Performance (example run)

Regression – Predicting rainfall (inches)

RMSE: ~0.39 inches

R²: ~0.18

Classification – Predicting rain / no rain

Accuracy: ~0.88

Good precision and recall for both rain and no-rain classes.

💬 Author

Created by Sai Aneesh

Focused on learning and demonstrating:
End-to-end ML workflow
Regression and classification on the same dataset
Clean coding and project structure for data science.
