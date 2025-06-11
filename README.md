# 🚗 Used Car Price Prediction

A machine learning project to predict the **price of used cars** based on various features like mileage, brand, engine specs, transmission, and accident history.

---

## 📌 Overview

This project involves:
- Cleaning and preprocessing a real-world used cars dataset
- Exploratory Data Analysis (EDA) with visualizations
- Training regression models to predict car prices
- Evaluating models using multiple metrics

---

## 📂 Dataset

The dataset includes both **categorical** and **numerical** features:

- **Categorical:** `brand`, `fuel_type`, `has_accident`
- **Numerical:** `milage`, `model_year`, `gear`, `hp`, `litre`, `cylinder`, `price`
- **Mixed:** `engine` (parsed into `hp`, `litre`, `cylinder`)

---

## ⚙️ ML Pipeline

### 🔧 Preprocessing
- Cleaned `milage`, `price`, and parsed `engine` specs
- Handled missing values:
  - **Numerical**: filled with mean
  - **Categorical**: filled using mode or random choices
- Encoded variables using:
  - Label Encoding (`brand`)
  - One-Hot Encoding (`fuel_type`)

### 🤖 Model Training
- Implemented **Linear Regression** and **Random Forest Regressor**
- Applied **log transformation** on price to reduce skewness

---

## 📊 Model Evaluation (Best: Random Forest)

| Metric   | Value (Absolute) | Value (Relative to Mean Price) |
|----------|------------------|--------------------------------|
| MAE      | 17,670.15        | ~35.16%                        |
| RMSE     | 135,287.21       | ~269.17%                       |
| R² Score | 0.1045           |                                |
| MAPE     | 23.67%           |                                |
| MPE      | -4.42%           |                                |

---

## 🔍 Key Learnings

- Extracting features from messy text (like engine details)
- Handling missing values with appropriate strategies
- Encoding techniques for categorical data
- Model evaluation using **MAE, RMSE, MAPE, R²**
- Benefits of **log transformation** in regression

---

## 🧠 Technologies Used

- **Python**, **Jupyter Notebook**
- **Pandas**, **NumPy**, **Matplotlib**, **Seaborn**
- **Scikit-learn**

---

## 📁 Project Files

| File Name       | Description                                      |
|------------------|--------------------------------------------------|
| `Model.ipynb`    | Full pipeline: EDA, preprocessing, modeling      |
| `used_cars.csv`  | Cleaned dataset used in the notebook             |
| `model.pkl` (opt)| Trained Random Forest model (optional for reuse) |

---

## 📎 How to Run

1. Clone the repo  
2. Open `Model.ipynb` in Jupyter or VS Code  
3. Run the notebook to see the full pipeline in action

---

### 📌 Note

This is an academic/personal learning project and not meant for production deployment without further tuning and validation.

---
