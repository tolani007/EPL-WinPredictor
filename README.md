Match Data Preprocessing and Predictive Modeling

Overview

This project focuses on preprocessing match data and extracting advanced features for predictive modeling. The workflow includes data cleaning, feature engineering, rolling averages, streak calculations, head-to-head statistics, Elo rating computation, and model training using machine learning classifiers.

Features and Processing Steps

1. Data Preprocessing

Loads match data from a CSV file.

Cleans column names and handles missing values.

Converts date values to ordinal format.

Encodes categorical variables for venues and opponents.

Extracts and transforms match time into cyclical features.

Maps match days into numerical values.

2. Feature Engineering

Creates rolling averages of key match statistics (e.g., goals, shots, expected goals).

Computes win and non-win streaks to capture momentum trends.

Generates interaction features such as xG differential and shot accuracy.

Implements head-to-head statistics based on historical matchups.

Calculates Elo ratings to track team strength dynamically.

3. Machine Learning Model Training

Trains multiple classifiers: XGBoost, Random Forest, and Logistic Regression.

Evaluates model performance using precision, recall, and F1-score.

Analyzes feature importance for interpretability.

Uses SHAP analysis for deeper insights into predictions.

4. Predictions on New Matches

Prepares upcoming match data by aligning features with trained models.

Normalizes and scales feature values.

Predicts match outcomes (Win/Draw/Loss) based on trained models.

Outputs probabilities for each result and saves predictions for analysis.

Installation

Ensure you have the required dependencies installed:

pip install --upgrade scikit-learn xgboost dask[dataframe] python-docx shap

Running the Code

To execute the pipeline:

Upload the matches.csv dataset.

Run the preprocessing and feature engineering scripts.

Train and evaluate the models.

Prepare new match data and generate predictions.

Output

matches_rolling.csv: Processed dataset with advanced features.

Misclassified match reports for each model.

Final predictions with win/draw/loss probabilities.

Future Improvements

Incorporate additional team-specific metrics.

Optimize feature selection using automated tuning.

Implement deep learning models for further accuracy enhancements.

For any queries or suggestions, feel free to contribute to this repository!
