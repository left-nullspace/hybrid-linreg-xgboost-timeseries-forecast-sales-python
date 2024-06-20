# README

This project focuses on forecasting store sales using a hybrid model inspired and adapted from Kaggle's Time Series Course. The hybrid model combines Linear Regression and XGBoost to capture both linear trends and non-linear patterns in the sales data. This involves data preprocessing, feature engineering, model training, prediction, and evaluation.

## Project Structure

1. **Data Preparation**:
   - Sales data is loaded, filtered, and preprocessed to include relevant features such as promotions and seasonal information.

2. **Feature Engineering**:
   - Features for Linear Regression are created to capture trends using a deterministic process.
   - Additional features for XGBoost include encoding categorical variables and calculating rolling statistics.

3. **Model Definition**:
   - A custom `BoostedHybrid` class is defined to combine two models. 
   - The `fit` method trains the first model and computes residuals for the second model.
   - The `predict` method combines predictions from both models.

4. **Model Training and Evaluation**:
   - The hybrid model is trained on the prepared features.
   - Model performance is evaluated using Root Mean Squared Error (RMSE) on both training and validation sets.
   - Different combinations of models are experimented with to explore and compare their effectiveness.

5. **Visualization**:
   - Predictions are visualized alongside actual sales data to assess the model's performance.

## Extra

- Inspired by Kaggle's Time Series Course.
- Combines Linear Regression and XGBoost for enhanced prediction accuracy.
- Experimentation with various model combinations to find the best-performing setup.
- Evaluation using RMSE to ensure model reliability.
