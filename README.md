# Flight Fare Prediction App

## Introduction
The **Flight Fare Prediction App** is designed to address the challenge of fluctuating flight fares, which makes it difficult for travelers to predict the best time to purchase tickets. By leveraging machine learning, this app aims to provide users with accurate fare predictions, helping them plan cost-effective trips.

## Problem Statement
Flight ticket prices vary significantly based on factors like:
- Demand
- Seasonality
- Airlines

These fluctuations make it difficult for travelers to determine the ideal time to book a flight, often leading to overpaying or missing out on lower prices.

## Solution Overview
This project uses machine learning to predict flight fares by:
- Building a predictive model using historical flight fare data.
- Developing a user-friendly web application that allows users to access flight fare predictions.

## Data Collection
The data used for this project was collected from provided datasets, which include:
- **Training set**: Used to train the machine learning model.
- **Test set**: Used to evaluate the model's performance.

The data contains features such as:
- **Date and time of the journey**: Information regarding when the flight takes place.
- **Airline, source, and destination**: The airline offering the flight and the airports involved.
- **Number of stops and duration**: Details about how many stops the flight has and how long the journey will take.

## Data Preprocessing
The preprocessing steps for the collected data include:
- **Handling missing values**: Removing or filling in missing data.
- **Converting categorical data**: Transforming non-numerical (categorical) values into numerical data for the machine learning model.
- **Timestamp extraction**: Breaking down date-time features into day, month, hour, and minute components.

## Exploratory Data Analysis (EDA)
To better understand the data, visualizations were created, including:
- **Histograms** and **box plots** to visualize data distributions.
- **Correlation analysis** to determine the relationships between various features and flight fares.

## Feature Selection
To improve model performance, less significant features were removed, and only the most impactful features were kept for training. This process included:
- Identifying and removing features that had little to no correlation with the target variable (flight fare).
- Focusing on features with a strong impact on the prediction results.

## Model Building
The predictive model was built using the **Random Forest Regressor** algorithm. Key steps include:
- **Splitting the data** into training and testing sets.
- **Training the model** using the training data.

## Model Evaluation
The model was evaluated using several performance metrics, including:
- **Mean Absolute Error (MAE)**
- **Mean Squared Error (MSE)**
- **Root Mean Squared Error (RMSE)**
- **R² Score**

Additionally, feature importance was analyzed to understand the impact of each feature on the model's predictions.

## Web Application Overview
The trained machine learning model was integrated into a web application that allows users to access fare predictions. The application consists of:
- **Django Backend**: The model is served through an API that processes prediction requests.
- **React Frontend**: A user-friendly interface where users can input their travel details and receive fare predictions.

## Conclusion
The Flight Fare Prediction App successfully predicts flight fares based on historical data. It offers travelers an easy-to-use tool to make informed decisions about when to book flights. 

### Potential Future Improvements
- Enhance the prediction accuracy by incorporating additional features.
- Add more data sources to increase the scope of predictions.
