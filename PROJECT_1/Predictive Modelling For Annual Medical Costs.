## Project Title: Predictive Modelling for Annual Medical Costs.
- Under this project, I built a Linear Regression Model to enable predict a patient's annual medical cost based on demographic, lifestyle, clinical, and financial features.

## Statemet of the Problem
Problem: Healthcare costs are complex, but actuaries need transparent, auditable models to set premiums and allocate budgets

## Objective: 
- To develop a Regression model with complete accuracy  adhering to Linear Regression assumptions, ensuring that every feature's coefficient is statistically significant and logically sound (e.g., older age must correlate with higher costs).

## PROJECT Outline
Data Preprocessing & Feature Engineering (Crucial for Linear Reg)
Handling Categoricals: Converting smoker, gender, region, insurance_plan, and occupation into numerical dummy variables (One-Hot Encoding) while avoiding the Dummy Variable Trap.

Scaling Decision: Discussing why scaling (StandardScaler/MinMax) is not strictly necessary for interpreting coefficients in Linear Regression, but might be applied to improve gradient descent convergence if using SGDRegressor.

Log-Transformation: Assessing if annual_medical_cost_usd is right-skewed. If so, applying a log-transformation to the target variable to satisfy the normality of residuals assumption (and later exponentiating coefficients for interpretation).

Exploratory Data Analysis (The "Pre-Model" Check)
Linearity Check: Scatter plots with lowess smoothing to visually confirm that continuous features (age, bmi, income) have a roughly linear relationship with the log of cost.

Correlation & Multicollinearity: Heatmap analysis to spot highly correlated predictors (e.g., age and doctor_visits). High multicollinearity inflates coefficient variance, so we calculate Variance Inflation Factor (VIF) early to drop redundant features.

## Building on the Model
- Used Train-Test Split: 80/20 split with random_state=42 for reproducibility.
- Model Fitting: Used statsmodels (for detailed summary tables) and sklearn.linear_model.LinearRegression (for predictions).
- Performance Metrics: Referenced R-squared & Adjusted R-square to enable account for the number of predictors added, Root Mean Squared Error (RMSE): To understand prediction error in actual dollars and Mean Absolute Error (MAE): For a robust, non-penalized error metric.

## Evaluating the  Model Diagnostics 
- The Model was then evaluated based off Linear Regresssion Assumptions to determine its effectiveness at Predictions.

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
