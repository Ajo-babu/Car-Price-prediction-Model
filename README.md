# Car-Price-prediction-Model
This is a Regression machine learning model  to predict price of cars
Project Report: Car Price Prediction Model
Introduction
The objective of this project was to develop a machine learning model to predict car prices accurately. Using the car price dataset, we explored relationships between various car features and their prices to assist manufacturers in understanding pricing dynamics. This involved data cleaning, preprocessing, exploratory data analysis, model building, and evaluation to identify the best regression model.

Dataset and Preprocessing
Dataset Details:

The dataset contained various features like car specifications and pricing information.
Initial data exploration revealed the presence of null values, duplicates, skewed features, and outliers.
Preprocessing Steps:

Handled missing values and duplicates to ensure data integrity.
Fixed skewness in numerical features using logarithmic and square root transformations.
Detected and treated outliers using box plots, the IQR method, and capping techniques.
Feature Engineering:

Encoded categorical variables using One-Hot and Label Encoding techniques.
Selected relevant features using the Variance Threshold method to retain only impactful predictors.

Exploratory Data Analysis (EDA)
Visualizations such as histograms, scatter plots, correlation matrices, and bar charts were used to explore relationships and distributions in the data.
A correlation matrix identified key features highly correlated with the target variable (price).

Model Development
The dataset was split into training and testing sets, and multiple regression models were built to predict car prices. The following models were implemented and evaluated:

Model	             R² Score	MAE	RMSE
Linear Regression	0.8257	0.1616	0.2018
Decision Tree Regressor	0.7450	0.1709	0.2441
Random Forest Regressor	0.8762	0.1366	0.1700
Gradient Boosting Regressor	0.8912	0.1337	0.1594
Support Vector Regressor	0.7909	0.1779	0.2210

Gradient Boosting Regressor emerged as the best model based on its superior R² score and lower error metrics.

Model Evaluation and Hyperparameter Tuning
Model Evaluation:

Actual vs. Predicted prices were visualized using scatter plots with a trend line to assess model performance.
Gradient Boosting Regressor showed the closest alignment between predicted and actual values.
Hyperparameter Tuning:

The Gradient Boosting Regressor was optimized using GridSearchCV, improving its performance further.
Final tuned model test results:
R² Score: 0.9089
MAE: 0.12
RMSE: 0.15

Model Deployment
The final Gradient Boosting Regressor model was saved for future use, enabling its integration into production systems for price prediction tasks.

Conclusion
This project successfully developed a robust regression model for car price prediction. Key highlights include:

Comprehensive preprocessing ensured data quality.
Gradient Boosting Regressor was identified as the best-performing model, achieving high accuracy with an R² score of 0.9089 on the test set.
Hyperparameter tuning further enhanced model performance.
This model can help car manufacturers understand pricing dynamics and make data-driven decisions regarding design and market strategy.
Future work could explore advanced ensemble methods, additional feature engineering, or the inclusion of real-time market data for further improvement.






