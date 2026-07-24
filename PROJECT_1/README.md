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
- Used Train-Test Split: 70/20 split with random_state=42 for reproducibility.
- Model Fitting: Used statsmodels (for detailed summary tables) and sklearn.linear_model.LinearRegression (for predictions).
- Performance Metrics: Referenced R-squared & Adjusted R-square to enable account for the number of predictors added, Root Mean Squared Error (RMSE): To understand prediction error in actual dollars and Mean Absolute Error (MAE): For a robust, non-penalized error metric.


##  Findings & Interpretation 
 1. Example findings (placeholders for your actual numbers):
 2. The "Smoker Tax": All else being equal, being a smoker increases annual medical costs by $X,XXX (p < 0.001).
 3. The Age Premium: Every additional year of age increases costs by $XXX, holding BMI and exercise constant.


## Recommendations (Derived from the Co-efficients)
- For Underwriting: Flag smokers immediately; the model justifies a specific premium surcharge of $X,XXX.

- For Policy Makers: Since BMI has a low coefficient relative to smoking, prioritize smoking-cessation subsidies over general weight-loss programs for immediate financial ROI.

- For Forecasting: Use the RMSE range to build a "Cost Confidence Interval" for budget planning for the next fiscal year.

## Limitations & Next Steps
Limitations: Linear Regression struggles with complex non-linear interactions (e.g., age might affect smokers differently than non-smokers).

Next Steps: Build a Regularized version (Ridge/Lasso) to reduce overfitting if we have many dummy variables, or try a Polynomial Regression to capture subtle non-linearity while maintaining interpretability.

## Data Source
https://www.kaggle.com/datasets/mirzayasirabdullah07/medical-insurance-cost-dataset
