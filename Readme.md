# Weather Prediction using Multiple Machine Learning Algorithms: A Comparison

This project is part of the IBM AI Engineer Professional Certificate on Coursera. It serves as the final project for the "Machine Learning with Python" course. The goal is to build and compare various classification models to predict the weather condition for the next day, specifically focusing on whether it will rain tomorrow (`RainTomorrow`).

## Project Objective

The main objective of this project is to create classification models using different machine learning algorithms to predict the weather condition for the next day. The target variable is `RainTomorrow`, which indicates whether it will rain the next day.

## Algorithms Used

The following machine learning algorithms were used for building classification models:

1. Linear Regression (adapted for classification)
2. K-Nearest Neighbors (KNN)
3. Decision Trees
4. Logistic Regression
5. Support Vector Machine (SVM)

## Evaluation Metrics

To evaluate the performance of the models, the following metrics were used:

1. **Accuracy Score**: The proportion of correctly predicted observations.
2. **Jaccard Index**: A measure of similarity between the predicted and actual labels.
3. **F1-Score**: The harmonic mean of precision and recall, useful for imbalanced datasets.
4. **Log Loss**: A performance metric that considers the uncertainty of the prediction.
5. **Mean Absolute Error (MAE)**: The average of absolute errors between the predicted and actual values.
6. **Mean Squared Error (MSE)**: The average of squared errors between the predicted and actual values.
7. **R2 Score**: Indicates the proportion of variance in the dependent variable predictable from the independent variable(s).

## Dataset Description

The dataset used in this project comes from the Australian Government's Bureau of Meteorology, with data spanning from 2008 to 2017. It includes daily weather observations with features such as temperature, rainfall, wind speed, humidity, and more. 

- **Source of the data**: Australian Government's Bureau of Meteorology (latest data can be found [here](http://www.bom.gov.au/climate/dwo/))
- **Additional Data**: The dataset also includes columns like `RainToday` and `RainTomorrow` and was gathered from Rattle, which can be accessed [here](https://bitbucket.org/kayontoga/rattle/src/master/data/weatherAUS.RData).

### Fields in the Dataset

| Field         | Description                                           | Unit            | Type   |
| ------------- | ----------------------------------------------------- | --------------- | ------ |
| Date          | Date of the observation in YYYY-MM-DD format          | Date            | object |
| Location      | Location of the observation                           | Location        | object |
| MinTemp       | Minimum temperature                                   | Celsius         | float  |
| MaxTemp       | Maximum temperature                                   | Celsius         | float  |
| Rainfall      | Amount of rainfall                                    | Millimeters     | float  |
| Evaporation   | Amount of evaporation                                 | Millimeters     | float  |
| Sunshine      | Amount of bright sunshine                             | hours           | float  |
| WindGustDir   | Direction of the strongest gust                       | Compass Points  | object |
| WindGustSpeed | Speed of the strongest gust                           | Kilometers/Hour | float  |
| WindDir9am    | Wind direction averaged over 10 minutes before 9 am   | Compass Points  | object |
| WindDir3pm    | Wind direction averaged over 10 minutes before 3 pm   | Compass Points  | object |
| WindSpeed9am  | Wind speed averaged over 10 minutes before 9 am       | Kilometers/Hour | float  |
| WindSpeed3pm  | Wind speed averaged over 10 minutes before 3 pm       | Kilometers/Hour | float  |
| Humidity9am   | Humidity at 9 am                                      | Percent         | float  |
| Humidity3pm   | Humidity at 3 pm                                      | Percent         | float  |
| Pressure9am   | Atmospheric pressure reduced to mean sea level at 9 am | Hectopascal     | float  |
| Pressure3pm   | Atmospheric pressure reduced to mean sea level at 3 pm | Hectopascal     | float  |
| Cloud9am      | Fraction of sky obscured by cloud at 9 am             | Eights          | float  |
| Cloud3pm      | Fraction of sky obscured by cloud at 3 pm             | Eights          | float  |
| Temp9am       | Temperature at 9 am                                   | Celsius         | float  |
| Temp3pm       | Temperature at 3 pm                                   | Celsius         | float  |
| RainToday     | Indicator if it rained today                          | Yes/No          | object |
| RainTomorrow  | Indicator if it will rain tomorrow                    | Yes/No          | object |

Column definitions were gathered from the Bureau of Meteorology's climate data page [here](http://www.bom.gov.au/climate/dwo/IDCJDW0000.shtml).


