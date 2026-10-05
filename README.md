# Agroclimatic Crop Yield and Production Prediction in Bangladesh Using Machine Learning and Explainable AI

## Overview
This repository contains the implementation associated with the research paper **“Agroclimatic Crop Yield and Production Prediction in Bangladesh Using Machine Learning and Explainable AI.”**

The study develops a machine learning framework for simultaneously predicting crop yield and total production in Bangladesh using historical agroclimatic and agricultural data.

## Dataset
The study uses the **Bangladesh Agroclimatic Crop Yield (2000–2024)** dataset covering eight divisions of Bangladesh.

The dataset contains:
- 150 division-year observations
- 12 agroclimatic and agricultural input features
- Crop Yield as a target variable
- Total Production as a target variable

Key features include temperature, precipitation, humidity, wind speed, soil wetness, solar radiation, cultivated area, and related agroclimatic variables.

## Models
The following regression models were implemented and evaluated:

- XGBoost
- Random Forest
- Gradient Boosting
- Linear Regression

Model performance was evaluated using:
- R²
- Mean Absolute Error (MAE)
- Root Mean Square Error (RMSE)

## Methodology
The main workflow includes:

1. Data preprocessing and exploratory analysis
2. Log transformation of the production target
3. Training and comparison of multiple regression models
4. Out-of-Fold (OOF) prediction using 5-fold cross-validation
5. Meta-feature augmentation using XGBoost predictions
6. Retraining models on the augmented feature set
7. Model interpretation using feature importance and SHAP

## Explainable AI
SHAP was used to interpret the final model and identify the agroclimatic and engineered features that had the greatest influence on crop yield and production predictions.

## Results
The final **XGBoost + Meta-Feature** model achieved:

- **Crop Yield R²:** 0.9117
- **Production R²:** 0.9820

The analysis showed that engineered meta-features and temporal information were important for crop-yield prediction, while cultivated area was highly influential for production prediction.

## Tools & Technologies
- Python 3.10
- Google Colab
- Scikit-learn
- XGBoost
- SHAP
- Pandas
- NumPy
- Matplotlib

## Publication
**Agroclimatic Crop Yield and Production Prediction in Bangladesh Using Machine Learning and Explainable AI**

2026 IEEE 5th International Conference on Robotics, Automation, Artificial-Intelligence and Internet-of-Things (RAAICON)

## Authors
- Jannatul Maoa Binta Rahim
- Susmita Sejuti Saha
- Rashik Reza Fahim
- Aishwarja Paul Sourav
- Dola Das
