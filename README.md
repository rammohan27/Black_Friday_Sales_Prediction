# Black Friday Sales Prediction

## Overview

The *Black Friday Sales Prediction* project aims to predict customer purchases during the Black Friday sales event using customer demographics and product-related features. By applying machine learning algorithms, this project forecasts purchase behaviors for various product categories. The model helps businesses and retailers optimize their marketing and sales strategies based on predicted customer purchase patterns.

## Table of Contents

- [Project Description](#project-description)
- [Dataset](#dataset)
- [Features](#features)
- [Data Preprocessing](#data-preprocessing)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Modeling](#modeling)
- [Evaluation](#evaluation)
- [Prerequisites](#Prerequisites)
## Project Description

The *Black Friday Sales Prediction* project is designed to predict the "Purchase" behavior of customers based on various factors such as demographic details, product categories, and user engagement. Machine learning algorithms, including Random Forest Regressor and Linear Regression, are used to build models that can accurately predict purchases across multiple product categories. The goal is to offer actionable insights for retailers to maximize Black Friday sales.


## Dataset

The dataset used in this project contains detailed customer and sales data for Black Friday. The features include customer demographics (e.g., age, gender, marital status, occupation), product categories, and their corresponding purchases.

- *Age*: Age group of the customer.
- *Gender*: Gender of the customer.
- *City_Category*: The category of the city where the customer resides.
- *Occupation*: Occupation of the customer.
- *Marital_Status*: Marital status of the customer.
- *Product_Category_1, Product_Category_2, Product_Category_3*: Product categories.
- *Purchase*: The target variable that represents the purchase amount made by the customer.

## Features

The key features of the model include:

- *Customer Demographics*: Age, Gender, City_Category, Occupation, and Marital_Status.
- *Product Categories*: Product_Category_1, Product_Category_2, Product_Category_3.
- *Target Variable*: Purchase.

## Data Preprocessing

Key preprocessing steps were performed to prepare the data for machine learning:

- *Handling Missing Values*: Imputation of missing values for Product_Category_2 and Product_Category_3.
- *Feature Encoding*: Categorical variables such as Gender, City_Category, and Age were encoded using techniques like LabelEncoder and OneHotEncoder.
- *Feature Engineering*: Binned customer ages and created new features like Age Group.
- *Normalization*: Data was standardized for the model.

## Exploratory Data Analysis (EDA)

EDA was conducted to analyze the relationships within the dataset. Key steps included:

- Visualizing the distribution of Product_Category_1, Product_Category_2, and Product_Category_3.
- Identifying outliers in the product categories.
- Exploring correlations between demographic features and purchase behavior.
- Generating a heatmap for feature correlations to identify strong relationships.

## Modeling

Various machine learning models were applied to predict customer purchases:

- *Random Forest Regressor*: An ensemble learning method that improves prediction accuracy.
- *Linear Regression*: Used for establishing a baseline model and performance comparison.
- *Random Forest Hyperparameter Tuning*: Optimizing the number of trees and model depth for better performance.

## Evaluation

The models were evaluated using the following metrics:

- *Root Mean Squared Error (RMSE)*: Measures the average magnitude of the errors in predictions.
- *R² Score*: Indicates how well the model fits the data, with a value closer to 1 indicating better performance.
- *Mean Absolute Error (MAE)*: Evaluates the average absolute error between predicted and actual values.


## Prerequisites

Before running the project, ensure that you have the following Python libraries installed:

- *pandas*: For data manipulation and analysis.
- *numpy*: For numerical operations and handling arrays.
- *scikit-learn*: For machine learning algorithms, model evaluation, and data splitting.
  - train_test_split: To split the dataset into training and testing sets.
  - RandomForestRegressor: For building the Random Forest regression model.
  - mean_squared_error: To calculate model performance (Mean Squared Error).
- *seaborn*: For statistical data visualization and creating informative plots.
- *matplotlib*: For creating various plots and visualizations.

You can install the required libraries using pip:

```bash
pip install  numpy
pip install scikit-learn
pip install seaborn
pip install  matplotlib