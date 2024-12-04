# Predicting-DoorDash-ETA-A-Machine-Learning-Approach

## Overview

This project aims to predict DoorDash delivery times using machine learning. It explores various models, including Linear Regression, Random Forest, XGBoost, and a Neural Network, to achieve accurate predictions. The project follows a comprehensive data science workflow, encompassing data preprocessing, feature engineering, model training, evaluation, and deployment.

## Dataset

The project utilizes a DoorDash dataset containing historical order information, including order creation time, actual delivery time, store details, order specifics, and delivery driver availability. The dataset is preprocessed to handle missing values, engineer new features, and transform data for optimal model performance.

## Methodology

1. **Data Preprocessing:** 
   - Missing values and duplicates are removed.
   - New features like 'delivery_duration_sec' and 'free_dashers' are created.
   - Date columns are converted to datetime objects.
   - Unnecessary columns are dropped, and outliers in the target variable are removed.

2. **Exploratory Data Analysis (EDA):**
   - Visualizations are employed to explore data distributions, relationships between variables, and correlations.

3. **Model Building and Evaluation:**
   - The dataset is split into training and testing sets.
   - Features are scaled using MinMaxScaler.
   - Four models are trained: Linear Regression, Random Forest, XGBoost, and a Neural Network.
   - Models are evaluated using metrics like R-squared, MAE, MSE, and RMSE.

4. **Model Selection and Deployment:**
   - The Neural Network model is selected as the best-performing model.
   - The model is saved for future use.
   - A function is created to load the saved model and make predictions on new data.

## Results

The Neural Network model achieved the highest accuracy in predicting DoorDash delivery times. The project demonstrates the effectiveness of machine learning in optimizing delivery operations and enhancing customer experience.

## Usage

To use the trained model for prediction:

1. Load the saved model using `tf.keras.models.load_model('model.keras')`.
2. Provide input data for the features used in the model.
3. Use the `prediction()` function to obtain the predicted delivery duration in seconds.

## Future Work

- Explore more advanced deep learning architectures for further performance improvement.
- Incorporate real-time data feeds for dynamic predictions.
- Develop a user interface for easy access to the prediction model.


## Conclusion

This project successfully demonstrates the potential of machine learning in predicting DoorDash delivery times. The insights gained can be valuable for optimizing delivery operations and improving customer satisfaction.
