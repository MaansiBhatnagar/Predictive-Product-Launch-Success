# Product Success Predictive Model
This repository contains a predictive model to evaluate whether a product launched in a specific U.S. state will be successful. The project uses real-world data, processes it for analysis, and implements machine learning models to make predictions. The primary focus is on analyzing and normalizing data, detecting and removing outliers, and leveraging Random Forest, Support Vector Machine (SVM), and Neural Network classifiers to achieve predictive insights.
________________________________________
# Table of Contents
1.  Project Overview
2.  Features
3.  Data Preprocessing
4.  Machine Learning Models
5.  Results

________________________________________
# Project Overview
This project aims to:
1.	Analyze the relationship between product categories, sales, and state-specific data.
2.	Detect trends and outliers using statistical methods like Z-scores.
3.	Train and evaluate multiple machine learning models to predict product success.
________________________________________
# Features
1.	Data Analysis: Explore relationships and clean missing data.
2.	Outlier Detection: Use Z-scores to detect and remove outliers.
3.	Data Normalization: Normalize numerical features for better performance.
4.	Machine Learning Models: Compare models including Random Forest, SVM, and Neural Networks.
5.	Feature Importance: Analyze which features contribute the most to predictions.
________________________________________
# Data Preprocessing
1.	Data Cleaning:
o	Columns with missing values: ['State', 'Category', 'Dollars', 'Unit sales', etc.].
o	Missing values were filled using column means where applicable.
2.	Outlier Removal:
o	Applied Z-scores to identify outliers.
o	Removed rows with Z-scores above a threshold (|Z| > 3).
3.	Feature Normalization:
o	Normalized numerical columns using MinMaxScaler.
4.	Aggregation:
o	Grouped data by state and category to compute maximum and minimum sales (Dollars).
o	Derived thresholds to classify launches as successful or not.
________________________________________
# Machine Learning Models
1.	Random Forest:
o	Provides feature importance insights.
o	Model was trained and evaluated on clean data.
2.	Support Vector Machine (SVM):
o	Uses RBF kernel for classification.
o	Standardized features using StandardScaler.
3.	Neural Networks:
o	Multi-layer perceptron (MLP) with hidden layers [8, 4, 1].
o	Optimized using the Adam solver with ReLU activation.
________________________________________
# Results
1.  Random Forest: Achieved baseline performance and identified critical features.
2. 	SVM: Provided high accuracy on both training and testing sets.
3.   Neural Networks:
   
o	Training Accuracy: ~85-90%

o	Testing Accuracy: ~80-85%

o	Detailed classification metrics were generated.

