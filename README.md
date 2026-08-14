# 🚗 Car Price Prediction with Machine Learning

## 📌 Project Overview

This project focuses on building a Machine Learning regression model to predict the selling price of used cars based on features such as car brand, car age, kilometers driven, fuel type, seller type, transmission, and ownership.

The project was developed using Python in Google Colab and uses Pandas, NumPy, Matplotlib, Seaborn, and Scikit-learn for data preprocessing, exploratory data analysis, visualization, model training, and evaluation.

The CarDekho Used Cars dataset is used for this project. The complete machine learning workflow is implemented, starting from data cleaning and feature engineering to model comparison and feature importance analysis.

## 🎯 Objectives

- Clean and preprocess the used-car dataset.
- Handle missing values and duplicate records.
- Standardize categorical values.
- Calculate car age from the manufacturing year.
- Extract the car brand from the car name.
- Perform Exploratory Data Analysis.
- Analyze factors affecting car selling prices.
- Encode categorical variables using One-Hot Encoding.
- Train multiple regression models.
- Compare model performance using MAE, RMSE, and R².
- Identify the best-performing model.
- Analyze feature importance.

## 🛠️ Tech Stack

- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

## 📂 Dataset

The project uses the CarDekho Used Cars Dataset.

The dataset contains information about used cars, including:

- name
- year
- selling_price
- km_driven
- fuel
- seller_type
- transmission
- owner

## 🧹 Data Cleaning and Preprocessing

The following preprocessing steps were performed:

- Loaded the CSV dataset using Pandas.
- Inspected the dataset shape and structure.
- Checked data types.
- Checked for missing values.
- Identified duplicate records.
- Removed duplicate rows.
- Cleaned categorical values.
- Standardized text values such as fuel type, seller type, transmission, and owner.

## ⚙️ Feature Engineering

### Car Age

Car age was calculated from the manufacturing year:

Car Age = Current Year - Manufacturing Year

### Brand

The brand was extracted from the first word of the car name.

Examples:

Maruti Swift Dzire VDI → Maruti

Hyundai i20 Sportz → Hyundai

Honda City → Honda

## 📊 Exploratory Data Analysis

Several analyses were performed to understand the dataset and identify patterns.

### Selling Price Distribution

A histogram was created to understand the distribution of used-car selling prices.

### Price vs Fuel Type

A box plot was used to compare selling prices across different fuel types.

### Price vs Car Age

A scatter plot was used to investigate the relationship between car age and selling price.

### Price vs Kilometers Driven

A scatter plot was used to analyze the relationship between kilometers driven and selling price.

### Correlation Analysis

A correlation heatmap was created to analyze relationships between numerical variables such as:

- Car Age
- Manufacturing Year
- Kilometers Driven
- Selling Price

## 🔢 Categorical Encoding

Machine learning algorithms require numerical input.

Categorical variables were converted into numerical features using One-Hot Encoding.

The following categorical features were encoded:

- Fuel
- Seller Type
- Transmission
- Owner
- Brand

## 🤖 Machine Learning Models

Two regression models were trained:

### 1. Linear Regression

Linear Regression was used as a baseline model to establish a relationship between the input features and selling price.

### 2. Random Forest Regressor

Random Forest Regressor was used as an ensemble model capable of capturing nonlinear relationships between different car characteristics and selling prices.

## 📏 Model Evaluation

The models were evaluated using three regression metrics:

### Mean Absolute Error (MAE)

Measures the average absolute difference between actual and predicted prices.

Lower MAE indicates better performance.

### Root Mean Squared Error (RMSE)

Measures the square root of the average squared prediction error.

Lower RMSE indicates better performance.

### R² Score

Measures how much variation in the selling price is explained by the model.

Higher R² indicates better performance.

## 📊 Model Comparison

The performance of Linear Regression and Random Forest Regressor is compared using:

- MAE
- RMSE
- R² Score

The notebook automatically identifies the best-performing model based primarily on the highest R² score and lower prediction errors.

## ⭐ Feature Importance

Feature importance analysis was performed using the Random Forest Regressor.

This helps identify which characteristics have the greatest influence on used-car selling prices.

A feature importance chart is generated in the notebook to visualize the most influential features.

## 📈 Actual vs Predicted Prices

An actual-vs-predicted scatter plot was created for the best-performing model.

The closer the predictions are to the reference line, the better the model's predictions.

## 💡 Key Insights

The analysis demonstrates that used-car prices can vary significantly depending on factors such as:

- Car age
- Brand
- Kilometers driven
- Fuel type
- Transmission
- Ownership
- Seller type

Generally, newer cars tend to have higher resale prices, while older cars and vehicles with higher mileage tend to have lower selling prices.

The machine learning models help quantify these relationships and provide predictions for used-car prices.

## 📁 Project Structure

Car-Price-Prediction-Machine-Learning/
│
├── Car Price Prediction.ipynb
├── CAR DETAILS FROM CAR DEKHO.csv
└── README.md

## ▶️ How to Run

This project was developed using Google Colab.

1. Download or clone this repository.
2. Open Car Price Prediction.ipynb in Google Colab.
3. Upload CAR DETAILS FROM CAR DEKHO.csv when prompted.
4. Run the notebook cells sequentially.
5. View the generated analysis, charts, model results, and conclusions.

## 🎓 Learning Outcomes

Through this project, I gained practical experience in:

- Python programming
- Pandas data manipulation
- NumPy
- Data cleaning
- Feature engineering
- Exploratory Data Analysis
- Data visualization
- One-Hot Encoding
- Linear Regression
- Random Forest Regression
- Model evaluation
- MAE, RMSE, and R²
- Feature importance
- Machine learning workflows

## 🏁 Conclusion

This project demonstrates a complete Machine Learning regression workflow for predicting used-car selling prices.

Starting with raw CarDekho data, the project performs data cleaning, feature engineering, exploratory analysis, categorical encoding, model training, and evaluation.

Two regression algorithms, Linear Regression and Random Forest Regressor, are compared using MAE, RMSE, and R² scores. Feature importance analysis is also performed to understand which car characteristics contribute most to price predictions.

Overall, the project demonstrates how machine learning can be applied to real-world automotive data to generate useful price predictions and insights.

## 👨‍💻 Project Details

Task: Task 3 — Car Price Prediction with Machine Learning

Environment: Google Colab

Language: Python

Dataset: CarDekho Used Cars Dataset

Domain: Machine Learning and Data Science

⭐ If you find this project useful, consider giving the repository a star!
