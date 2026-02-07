# 🏡 Airbnb Price Prediction using Machine Learning

## 📌 Project Overview
- This project focuses on predicting Airbnb listing prices using machine learning models. The dataset includes features such as amenities, room type, number of bedrooms and bathrooms, and distance from the city center. The goal is to build and compare multiple regression models and identify the best-performing one for price prediction.

## 🎯 Objective
- Clean and preprocess Airbnb listing data
- Train and compare multiple machine learning models
- Tune the best model for improved performance
- Interpret feature importance using SHAP analysis

## 📂 Dataset Features
The dataset contains information such as:
- Amenities
- Number of bedrooms
- Number of bathrooms
- Room type
- Distance from city center
Categorical variables were converted into numerical format for model training.
Download Link: 👇
https://www.kaggle.com/datasets/stevezhenghp/airbnb-price-prediction
## ⚙️ Methodology
1. Data Preprocessing
- Loaded and cleaned the dataset
- Handled missing values
- Extracted relevant features
- Encoded categorical variables

2. Model Training
- Four machine learning models were trained:
- Random Forest
- XGBoost
- Gradient Boosting
- Extra Trees

## 📊 Model Evaluation
Models were evaluated using:
- RMSE (Root Mean Squared Error)
- MAE (Mean Absolute Error)
- R² Score
Among all models, Random Forest performed best and was selected for tuning.

## 🔧 Hyperparameter Tuning
Random Forest was tuned using RandomizedSearchCV.
Best parameters included:
- n_estimators = 400
- max_depth = 20
- min_samples_leaf = 1

## 🧠 SHAP Analysis
SHAP (SHapley Additive exPlanations) was used to interpret feature impact:
- Amenities such as AC, heating, kitchen, washer, and dryer increase price
- Shared room listings reduce predicted price
- Higher SHAP values indicate greater influence on predictions

## 🏆 Results & Conclusion
- Random Forest achieved the best performance among all tested models
- Price predictions were very large due to scale/log-transformed price values
- SHAP analysis helped identify important price-driving features
- The trained model can be used for dashboards or further development

## 🛠️ Technologies Used
- Python
- Pandas
- NumPy
- Scikit-learn
- XGBoost
- SHAP
- Matplotlib
- Seaborn
- Jupyter Notebook
