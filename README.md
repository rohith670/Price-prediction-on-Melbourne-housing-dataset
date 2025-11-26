# 🏡 Melbourne Housing Price Prediction

![Python](https://img.shields.io/badge/Python-3.x-blue?style=for-the-badge&logo=python)
![Scikit-Learn](https://img.shields.io/badge/Scikit_Learn-Pipelines-orange?style=for-the-badge&logo=scikit-learn)
![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)

## 📌 Project Overview
This project is a Machine Learning solution designed to predict the price of properties in the Melbourne housing market. By analyzing features such as location (Suburb, Region), room count, land size, and building area, the model estimates property values with high accuracy.

The core focus of this project was to implement **Production-Grade Code** using **Scikit-Learn Pipelines** to prevent data leakage and ensure clean, reproducible preprocessing.

## 🚀 Key Technical Features
* **Automated Preprocessing Pipeline:** Utilized `sklearn.pipeline.Pipeline` to chain preprocessing steps.
* **Column Transformations:** Implemented `ColumnTransformer` to handle mixed data types:
    * **Numerical:** Imputation (Median) + Scaling (StandardScaler).
    * **Categorical:** Imputation (Most Frequent) + One-Hot Encoding.
* **Model Selection:** Deployed a **Random Forest Regressor** to handle non-linear relationships in real estate data.
* **Robust Evaluation:** Evaluated using R² Score, MAE (Mean Absolute Error), and MSE.

## 📊 Model Performance
The Random Forest model performed effectively on the test dataset:

| Metric | Score | Description |
| :--- | :--- | :--- |
| **R² Score** | **0.80** | The model explains 80% of the variance in housing prices. |
| **MAE** | ~167k | Average difference between predicted and actual price. |

## 🛠️ Tech Stack
* **Language:** Python
* **Libraries:** Scikit-Learn, Pandas, NumPy
* **Tools:** Jupyter Notebook

## 📂 Project Structure
```text
├── data/
│   └── melb_data.csv        # Dataset (Source: Kaggle)
├── notebooks/
│   └── price_prediction.ipynb # Model Training & Analysis
├── README.md                # Project Documentation
└── requirements.txt         # Dependencies

