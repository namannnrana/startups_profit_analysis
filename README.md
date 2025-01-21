# Startup Analysis

This project implements **Multiple Linear Regression** to predict the profit made by a startup based on expenses incurred and the state where they operate.

## 📌 Objective
The goal of this project is to build a predictive model that estimates startup profits based on various input factors using **Multiple Linear Regression**.

## 🛠️ Technologies Used
- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib

## 📂 Dataset
The dataset used in this project is **50_Startups.csv**, which contains the following columns:
- **R&D Spend** - Investment in Research & Development
- **Administration** - Administrative costs
- **Marketing Spend** - Investment in marketing
- **State** - Location of the startup (New York, California, Florida)
- **Profit** - Net profit earned by the startup

## 🔄 Data Preprocessing
1. **Exploratory Data Analysis (EDA)**
   - Scatter plots of Profit vs. different features
   - Bar chart for average profit across states

2. **Feature Engineering**
   - One-hot encoding for the categorical variable **State**
   - Dropping the original **State** column

3. **Splitting the Dataset**
   - Dividing data into **training (80%)** and **testing (20%)** sets

4. **Feature Scaling**
   - Using **MinMaxScaler** to normalize input features

## 📊 Model Training
- Implemented **Multiple Linear Regression** using `sklearn.linear_model.LinearRegression`.
- Computed **coefficients** and **intercept** of the regression model.

## 🎯 Model Evaluation
- **Mean Squared Error (MSE)** on the test set: `83502864.03`
- **Root Mean Squared Error (RMSE)**
  - Train RMSE: `9031.67`
  - Test RMSE: `9137.99`
- **R² Score on Training Data**: `0.9502` (indicating a strong model performance)

## 📈 Predictions
The model predicts startup profits based on the given input features. Below are some predictions on the test set:

| Actual Profit | Predicted Profit |
|--------------|----------------|
| 103282.38   | 103015.20      |
| 144259.40   | 132582.28      |
| 146121.95   | 132447.74      |
| 77798.83    | 71976.10       |
| 191050.39   | 178537.48      |
