# Air-Quality-Prediction-Using-Regression-Analysis
This project aimed to develop predictive models for air quality index (AQI) prediction using regression analysis techniques. By leveraging machine learning algorithms and time series forecasting methods, the project sought to provide insights into air pollution patterns and support informed decision-making for air quality management.

## Project Overview

- **Dataset**: Air quality index (AQI) data collected from a monitoring station in a city in Italy, spanning a 12-month period from March 2004 to February 2005, with 9,358 instances of hourly averaged responses from an array of five metal oxide chemical sensors.
- **Technologies Used**: Python (NumPy, Pandas, Matplotlib, Scikit-learn, Statsmodels), Machine Learning Algorithms (Decision Tree, KNN, Random Forest, SVM), Time Series Forecasting (ARIMA, Exponential Smoothing)
- **Key Objectives**:
  - Preprocess and analyze the AQI dataset, handling missing values and outliers.
  - Develop machine learning models for AQI classification using algorithms like Decision Tree, KNN, Random Forest, and SVM.
  - Perform time series analysis and forecasting using ARIMA and Exponential Smoothing models.
  - Evaluate model performance and provide insights into air quality patterns and future trends.

## Project Implementation

1. **Data Preprocessing**: Handled missing values using KNN imputation and performed outlier detection and removal. Defined the AQI variable based on pollutant concentrations and categorized it into distinct categories (Good, Satisfactory, Fairly Polluted, Poor, Hazardous).

2. **Machine Learning Models for AQI Classification**:
   - Decision Tree Classifier: Achieved an accuracy of 0.7763 with tuned hyperparameters (max_depth=3, min_samples_leaf=0.1).
   - KNN Classifier: Obtained an accuracy of 0.9441 with optimized hyperparameters (k=5, weighting='distance').
   - Random Forest Classifier: Achieved an accuracy of 0.8736 with tuned parameters (max_depth=4, max_features=4, min_samples_leaf=5, n_estimators=200).
   - SVM Classifier: Achieved an accuracy of 0.8978 with optimized hyperparameters ('C': 0.01, 'degree': 4, 'kernel': 'poly').

3. **Time Series Analysis and Forecasting**:
   - ARIMA Model: Conducted seasonal decomposition analysis, identified stationarity using the Augmented Dickey-Fuller (ADF) test, and developed an ARIMA model for forecasting. The model had a mean absolute error of 74.98 and a root mean square error of 84.96.
   - Exponential Smoothing: Implemented the Holt-Winters method with additive trend and additive seasonal components. The model achieved a Mean Absolute Percentage Error (MAPE) of 4.51%, indicating good prediction accuracy.

## Key Findings and Results

- The KNN Classifier achieved the highest accuracy of 0.9441 among the evaluated machine learning models for AQI classification.
- The Exponential Smoothing model outperformed the ARIMA model for time series forecasting, with a MAPE of 4.51%, indicating reliable predictions.
- The analysis revealed occasional spikes in pollution levels, highlighting the need for continued air quality monitoring and mitigation efforts.


## Conclusion

This project successfully developed machine learning models and time series forecasting techniques for air quality prediction and analysis. The findings provide valuable insights into air pollution patterns, enabling informed decision-making and supporting air quality management strategies. The models can be further refined and integrated into air quality monitoring systems to support proactive measures and protect public health.
