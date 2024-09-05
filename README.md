# Predicting Car Prices Using Multivariate Linear Regression

This project aims to predict the price of a car based on various features such as the car's make, model, year, engine size, mileage, and more. The model developed in this project applies **multivariate linear regression** to perform the predictions.

## Objective

To build a regression model that can predict car prices based on multiple features using **multivariate linear regression**.

## Problem Statement

Given a dataset containing information about different cars, the task is to predict the price of a car using features like make, model, year, mileage, engine size, fuel type, transmission, and horsepower.

## Dataset Features

- **Make**: Brand of the car (e.g., Toyota, Honda, BMW)
- **Model**: Specific model of the car
- **Year**: Year of manufacture
- **Mileage**: Total miles driven by the car
- **Engine Size**: Engine capacity in liters
- **Fuel Type**: Type of fuel (e.g., petrol, diesel, electric)
- **Transmission**: Type of transmission (manual or automatic)
- **Horsepower**: The car's horsepower
- **Number of Doors**: Number of doors in the car
- **Price**: Target variable (price of the car in dollars)

## Steps

### 1. Data Collection and Exploration
- The dataset used is `car_prices_dataset.csv`. 
- Initial exploration of data to understand the relationships between the features and the target variable (price).

### 2. Data Preprocessing
- **Handling Missing Values**: Missing data will be cleaned and filled as appropriate.
- **Categorical Variables**: Conversion of categorical variables like 'make', 'model', and 'fuel type' into numerical values using techniques such as **one-hot encoding**.
- **Feature Scaling**: Standardize features to ensure uniformity across variables, if necessary.

### 3. Feature Selection
- Correlation analysis and other techniques to identify the most impactful features on car price prediction.

### 4. Model Development
- Split the dataset into **training** and **testing** sets.
- Build a **multivariate linear regression model** using the training set.
- Train and evaluate the model using metrics such as **Mean Squared Error (MSE)** and **R²** score.

### 5. Model Evaluation and Interpretation
- Analyze model performance on test data.
- Interpret the regression coefficients to determine the impact of each feature on the predicted car prices.

### 6. Model Improvement
- Experiment with feature engineering or adding **polynomial features** to enhance model accuracy and performance.

### 7. Conclusion and Insights
- Summarize findings and identify which features are the most influential in predicting car prices.
- Provide insights on how to improve car price prediction models in the future.

## Tools and Technologies

- **Python**
- **Pandas**
- **NumPy**
- **Scikit-Learn**
- **Matplotlib** (for visualizations)

## How to Run the Project

1. Clone this repository.
2. Install the necessary libraries:
   ```bash
   pip install pandas numpy scikit-learn matplotlib
   ```
3. Run the script to train and test the model:
   ```bash
   python car_price_prediction.py
   ```
4. The model's performance metrics will be displayed, and predictions can be made by providing input features.

## Results

- The model predicts car prices with a certain level of accuracy as evaluated by MSE and R² metrics.
- Features like **year**, **mileage**, **engine size**, and **make** have the highest impact on the price.
