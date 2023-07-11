__Faulty Air Quality Sensor Challenge__

This repository contains code for the Faulty Air Quality Sensor Challenge in UmojaHack Africa 2022. The challenge involves predicting faulty air quality sensors based on various sensor readings.

__Dataset__

The dataset consists of a train.csv file containing the training data and a test.csv file containing the test data. The data includes sensor readings, temperature, relative humidity, and offset fault information.

__Data Exploration__

The code performs data exploration to gain insights into the dataset. It includes steps such as loading the data, checking for missing values, visualizing data distributions, and examining correlations between features.

__Data Cleaning__

Data cleaning steps are implemented to handle missing values and outliers in the dataset. Missing numeric values are filled with the median, and outliers in certain features are replaced with appropriate threshold values.

__Feature Engineering__

Date and time features are extracted from the datetime column to enrich the dataset. These features include year, month, day, and hour. The datetime column is then dropped from the dataset.

__Modelling__

The XGBoost classifier is used to train the model. The code splits the dataset into training and testing sets, fits the model on the training data, and evaluates the model's performance on the training set using mean absolute error.

__Hyperparameter Tuning__

RandomizedSearchCV is used to find the best set of hyperparameters for the XGBoost classifier. The code defines a parameter grid with different values for learning rate, max depth, min child weight, n iter, gamma, and colsample bytree. The best parameters are printed, and the model is trained with these parameters.

__Prediction and Submission__

The trained model is used to make predictions on the test data. The predicted offset fault values are saved in a submission file, which is then uploaded to Google Drive.

__Repository Keywords and Hashtags__

Keywords: Faulty Air Quality Sensor, UmojaHack Africa, Data Exploration, Data Cleaning, Feature Engineering, Modelling, Hyperparameter Tuning, XGBoost Classifier, Prediction, Submission.

#FaultyAirQualitySensorChallenge #UmojaHackAfrica #DataExploration #DataCleaning #FeatureEngineering #Modelling #HyperparameterTuning #XGBoostClassifier #Prediction #Submission
