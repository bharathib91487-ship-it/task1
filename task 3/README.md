Housing Price Prediction using Linear Regression
📌 Project Overview

This project demonstrates the use of Linear Regression to predict housing prices based on both numeric and categorical features such as area, bedrooms, bathrooms, parking, and amenities like furnishing status, air conditioning, etc. The goal is to identify key factors that influence house prices and estimate prices for new listings.

🚀 Methodology
1. Data Import & Preprocessing

Loaded the Housing.csv dataset using pandas.

Converted categorical features (e.g., mainroad, guestroom, furnishingstatus) into numeric form using one-hot encoding.

Ensured the final dataset contained only numeric values, ready for model training.

2. Train-Test Split

Defined features (X) and target (y = price).

Split data into training and testing sets using train_test_split():

80% for training

20% for testing

3. Model Training

Initialized a Linear Regression model from sklearn.linear_model.

Trained the model on the training data (X_train, y_train).

4. Model Evaluation

Predicted house prices for the test set.

Measured performance using metrics:

MAE (Mean Absolute Error): Average absolute difference between predicted and actual prices.

MSE (Mean Squared Error): Penalizes larger errors more heavily.

R² Score: Indicates how well the model explains variation in house prices.

5. Visualization & Interpretation

Plotted actual vs predicted prices for insights.

Analyzed model coefficients to understand feature impact:

Intercept (b0): Base price when all features are zero.

Feature coefficients (b1, b2, …): Effect of each feature on price.

Example: If the coefficient for area = 500, each extra sq ft increases price by ₹500 (holding other features constant).

📊 Key Insights

High-impact features:

Numeric: area, bedrooms, bathrooms

Categorical: airconditioning_yes, furnishingstatus_furnished

Model performance:

R² score indicates the proportion of price variation explained by the model.

This analysis helps identify which factors most influence housing prices and provides a framework to predict prices for new properties.
