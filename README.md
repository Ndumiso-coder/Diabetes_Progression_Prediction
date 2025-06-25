# Diabetes Progression Prediction using Supervised Learning : Multiple Linear Regression

This repository contains a Jupyter Notebook that performs multiple linear regression on a dataset
(`diabetes_dirty.csv`), csv dataset has been attached, to predict the progression of diabetes in patients
based on various medical attributes.

## Project Description

The objective of this project is to build and evaluate a linear regression model that predicts a patient's 
diabetes progression using available features in the dataset. The project includes data handling (checking
missing entries), Data visualization, feature scaling, model training, and performance evaluation and
conclusion. 

## Steps Followed

The notebook `diabetes_regression_2.ipynb` follows these key steps:

1. **Importing relevent libraries**
 
3. **Read And Preview the Dataset**
   - Load `diabetes_dirty.csv` into a pandas DataFrame.
   - Preview a few rows to make sense of the data.
  
4. **Check the shape of the data and missing entries** 
  - No missing values were identified, otherwise data cleaning and preprocessing would have been performed.

5. **Visualise and Prepare Data** 
   - Identify independent variables (`X`) and the dependent variable (`Y`) for regression.
   - Create a simple linear regression model for each independent variable vs the dependent and plot the best-fit line.
   - Also analyse their correlations using a heatmap.
   - Feature matrix construction (combine all independent variables (x) into a single variable (X)
   - Create a PROGRESSION model and get the intercept and coefficients. 
   - Split the dataset into training and test sets using an 80/20 split.

7. **Data Scaling**
   - Analyze the need for feature scaling.
   - Apply `MinMaxScaler` and/or `StandardScaler` from `sklearn.preprocessing` as required.
   - Fit the scaler on the training set and transform both training and test data.

8. **Model Training**
   - Create and train a multiple linear regression model using `LinearRegression` from `sklearn.linear_model`.
   - Use all independent variables.

9. **Model Evaluation**
   - Print the model's intercept and coefficients.
   - Make predictions on the test set.
   - Evaluate the model using the r2_score and RMSE from `sklearn.metrics`.

8. **Documentation**
   - The notebook includes detailed comments explaining each step.
   - Outputs like the R-squared value are interpreted and discussed.

## Requirements

To run this project, make sure the following programming language & packages are installed:

- Python 3.x          - programming language
- pandas              - for data handling
- numpy               - for numerical computation
- scikit-learn        - for building models
- Matplotlib          - for basic plotting
- Seaborn             - for statistical visualisation
- Jupyter Notebook    - interactive coding environment

You can install the dependencies using pip:
pip install pandas numpy scikit-learn matplotlib seaborn notebook
