# predict_houses_price_using_Machine_Learning
This project implements a complete machine learning workflow to predict house prices. It moves beyond simple linear models by incorporating feature engineering and ensemble strategies to achieve high predictive accuracy.
# Data Loading & EDA
The notebook begins by loading the dataset and performing Exploratory Data Analysis (EDA). Key steps include:

-Identifying correlations between features (e.g., Square Footage vs. Price).

-Handling missing values and outliers.

-Visualizing distributions to check for skewness.
# Feature Engineering & Preprocessing 
-Log Transformation: Applied to the target variable (y) to normalize its distribution and handle heteroscedasticity.

-One-Hot Encoding: Used to convert categorical variables into a format suitable for machine learning.

-Standard Scaling: Ensuring all numerical features are on the same scale for models like SVR and Linear Regression.

-Polynomial Features: Generating interaction terms to capture non-linear relationships between variables.
# Model Implementation
-Linear Regression: The baseline model for performance comparison.

-Support Vector Regression (SVR): A robust regressor that handles high-dimensional data well.

-Random Forest Regressor: An ensemble of decision trees to capture complex patterns.

-Gradient Boosting Regressor: A boosting method that builds trees sequentially to minimize error.
# Advanced Ensemble: Stacking
-The notebook concludes with a Stacking Regressor. This "meta-model" combines the strengths of Random Forest and Gradient Boosting, using a Linear Regression model as the final estimator to produce the ultimate prediction.

# Key Results
-The Stacked Model successfully reduced error compared to individual base models, demonstrating that combining different algorithmic approaches (bagging and boosting) provides a more generalized and accurate prediction for housing prices.
