# Car Price Prediction with Machine Learning

## Overview

This project develops a machine learning regression system to predict the selling price of used cars. The analysis explores how factors such as car age, present price, mileage, fuel type, transmission, seller type, and brand relate to the final selling price.

## Objective

To build and evaluate regression models capable of predicting used-car selling prices using relevant vehicle features.

## Dataset

The dataset contains used-car information including:

- Car Name
- Manufacturing Year
- Selling Price
- Present Price
- Kilometers Driven
- Fuel Type
- Seller Type
- Transmission
- Owner

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Methodology

### 1. Data Cleaning
- Checked for missing values.
- Identified and removed duplicate records.
- Checked categorical variables for inconsistent values.

### 2. Feature Engineering
- Created `Car_Age` from the manufacturing year.
- Extracted `Brand` from the car name.

### 3. Exploratory Data Analysis
- Analyzed the distribution of selling prices.
- Compared selling prices across fuel types.
- Examined the relationship between car age and selling price.
- Analyzed feature correlations using a heatmap.

### 4. Data Preparation
- Applied One-Hot Encoding to categorical variables.
- Divided the data into training and testing sets using an 80:20 split.

### 5. Machine Learning
Two regression models were developed:

- Linear Regression
- Random Forest Regressor

### 6. Model Evaluation

The models were evaluated using:

- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R² Score

## Model Results

| Model | MAE | RMSE | R² Score |
|---|---:|---:|---:|
| Linear Regression | 1.809 | 3.399 | 0.552 |
| Random Forest Regressor | 1.409 | 3.429 | 0.544 |

Random Forest achieved a lower MAE, while Linear Regression achieved slightly lower RMSE and a higher R² score on the test set.

## Feature Importance

Feature importance from the Random Forest model was analyzed to identify the variables contributing most to the prediction. `Present_Price` was the most influential feature, followed by `Year` and `Car_Age`.

## Project Structure

```text
Task_3_Car_Price_Prediction/
│
├── Car_Price_Prediction.ipynb
├── car data.csv
└── README.md
