## Project Title: Predictive Modelling for Annual Medical Costs.
- Under this project, I built a Linear Regression Model to enable predict a patient's annual medical cost based on demographic, lifestyle, clinical, and financial features.

## Statemet of the Problem
Problem: Healthcare costs are complex, but actuaries need transparent, auditable models to set premiums and allocate budgets

## Objective: 
- To develop a Regression model with complete accuracy  adhering to Linear Regression assumptions, ensuring that every feature's coefficient is statistically significant and logically sound (e.g., older age must correlate with higher costs).

## PROJECT OUTLINE
- Data Preprocessing: Importing, reading and storing the dataset.
- Cleaning and proper structuring of the dataset.
- Feature Selection to enable model building.
- Handling Categoricals by transforming categorical variables into numeric variables.
- Converting smoker, gender, region, insurance_plan, and occupation into numerical dummy variables (One-Hot Encoding) while avoiding the Dummy Variable Trap.
- Exploratory Data Analysis (The "Pre-Model" Check): Using Plots to check for relationships between target variables and predictors.
- Correlation: Using  Heatmap plots to spot predictors relationships with the Target variable.


## Building on the Model
- Used Train-Test Split: 70/30 split with random_state=42 for reproducibility.
- Model Fitting: Used statsmodels (for detailed summary tables) and sklearn.linear_model.LinearRegression (for predictions).
- Performance Metrics: Referenced R-squared & Adjusted R-square to enable account for the number of predictors added, Root Mean Squared Error (RMSE): To understand prediction error in actual dollars and Mean Absolute Error (MAE): For a robust, non-penalized error metric.


##  Findings & Interpretation 
 1. Each of the predictor variable: Chronic disease, Doctor visits, Number of hospitalizations, Smoking habits and Insurance plans are significant in Predicting the Annual Medical Cost at Trade Global Health Center. (P-value < 0.05).
 2. With the addition of More feature variables into the model, accuracy of the model improved from 24% to 84% giving confidence that the model is suitable for practical real life use cases at the health facility.


## Data Source
https://www.kaggle.com/datasets/mirzayasirabdullah07/medical-insurance-cost-dataset


## HOW TO RUN THE PROJECT
- First Install dependencies: pip install pandas, numpy,scikit-learn etc.
- The run the Predicting Medical Expenses.ipynb to go through my entire project data.

