🚗 Used Car Price Prediction – Machine Learning Project

📌 Overview
This project focuses on predicting the price of used cars using machine learning techniques. The dataset contains various features like brand, model year, mileage, engine specs, fuel type, accident history, and more.

The goal was to clean and preprocess the data, explore it through visualizations, and train models to predict the car price effectively.

📂 Dataset
The dataset includes:

Categorical: brand, fuel_type, has_accident

Numerical: milage, model_year, gear, hp, litre, cylinder, price

Mixed: engine (preprocessed to extract hp, litre, cylinder)

⚙️ ML Pipeline
Data Preprocessing

Cleaned milage, price, and engine columns

Handled missing values with mean (numerical) and mode/random choice (categorical)

Encoded categorical variables using Label Encoding and One-Hot Encoding

Model Training

Tried both Linear Regression and Random Forest Regressor

Applied log transformation on the target to reduce skewness

Model Evaluation
📊 Random Forest (best performing model):

MAE: 17,670.15 (~35.16%)

RMSE: 135,287.21 (~269.17%)

R² Score: 0.1045

MAPE: 23.67%

MPE: -4.42%

🔍 Key Learnings
Feature extraction from messy text columns

Handling missing values and encoding techniques

Model evaluation using multiple metrics (MAE, RMSE, MAPE, R²)

Log transformation to handle skewed price distributions

🧠 Technologies Used
Python, Jupyter Notebook

Pandas, NumPy, Matplotlib, Seaborn

Scikit-learn

📁 Files
Model.ipynb – Full notebook with code, EDA, preprocessing, model training, and evaluation

used_cars.csv – Cleaned dataset used in the project
