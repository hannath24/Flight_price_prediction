# Flight Price Prediction Using Machine Learning

## Project Overview
This project aims to predict airline ticket prices using machine learning techniques. The dataset contains flight details such as airline, source, destination, departure time, arrival time, total stops, journey date, and duration.

The goal is to build a regression model capable of accurately predicting flight prices by performing data preprocessing, feature engineering, model training, evaluation, and interpretation.

---

## Dataset Features

The dataset contains the following important features:

- Airline
- Source
- Destination
- Departure Time
- Arrival Time
- Duration
- Total Stops
- Journey Date
- Additional Information
- Price (Target Variable)

---

## Feature Engineering

Several new features were created to improve model performance:

- **Journey Month**
- **Journey Day**
- **Journey Weekday**
- **Total Duration in Minutes**
- **Departure Total Minutes**
- **Arrival Total Minutes**
- **Departure Time Category (Morning / Afternoon / Evening / Night)**
- **Arrival Time Category**

These transformations helped convert raw time and date features into meaningful numerical and categorical variables.

---

## Data Preprocessing

The following preprocessing steps were applied:

- Handling categorical variables using **One Hot Encoding**
- Feature scaling for numerical features
- ColumnTransformer pipeline for automated preprocessing
- Train-Test Split for model evaluation

---

## Machine Learning Models Used

The following regression models were trained and compared:

- HistGradientBoosting Regressor
- Random Forest Regressor
- XGBoost Regressor
- HistGradientBoosting
- Decision Tree

Hyperparameter tuning was performed to improve model performance.

---

## Model Evaluation

The models were evaluated using:

- R² Score
- RMSE (Root Mean Squared Error)
- MAE (Mean Absolute Error)

The final selected model was **HistGradientBoosting Regressor**, which achieved the best balance between performance and generalization.

---

## Cross Validation

5-Fold Cross Validation was performed to ensure model stability.
Example result:
Mean CV R² Score ≈ **0.939**
Standard Deviation ≈ **0.003**
model performance is consistent across different data splits.

---

## Residual Analysis

Residual analysis was performed to check model assumptions and prediction behavior.

Plots used:

- Residual vs Predicted plot
- Residual distribution plot

These plots helped identify variance patterns and evaluate prediction errors.

---

## Feature Importance

Permutation Feature Importance was used to interpret the model.

Top important features included:

1. Duration (Total Minutes)
2. Airline
3. Journey Month


This analysis helps understand which variables influence ticket prices the most.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn

---


