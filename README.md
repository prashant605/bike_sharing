# Bike Sharing Assignment
> The purpose of this project is to understand the factors affecting the demand for BoomBikes in the American market and build a multiple linear regression model for the prediction of demand for its shared bikes.


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)


## General Information
## Objective
The main objective of this analysis is to:
- Identify the factors affecting the demand for BoomBikes in the American market.
- Understand how exactly the demands vary with different features.
- Build a multiple linear regression model for the prediction of demand for its shared bikes.

## Dataset
The dataset used for this project contains detailed features and bike usage. It includes both categorical and numerical features, such as temp, hum, season, and weathersit.

### Key Features:
- **yr:** year (0: 2018, 1:2019)
- **mnth:** month ( 1 to 12)
- **weekday:** day of the week
- **workingday:** if day is neither weekend nor holiday is 1, otherwise is 0
- **holiday:** whether day is a holiday or not
- **season:** season (1:spring, 2:summer, 3:fall, 4:winter)
- **weathersit:** (1: Clear, Few clouds, Partly cloudy, Partly cloudy; 2: Mist + Cloudy, Mist + Broken clouds, Mist + Few clouds, Mist; Light Snow, Light Rain + Thunderstorm + Scattered clouds, Light Rain + Scattered clouds; 4: Heavy Rain + Ice Pallets + Thunderstorm + Mist, Snow + Fog)
- **temp:** temperature in Celsius
- **atemp:** feeling temperature in Celsius
- **hum:** humidity
- **windspeed:** wind speed

## Approach
### Data Preprocessing:
- **Handling Missing Data:** Rows with significant missing values were either removed or imputed.
- **Derived Metrics:** Created new metrics like issue_month, issue_year from existing data.
- **Categorical Variables:** Proper handling and transformation of categorical variables to be used into model
  
### Exploratory Data Analysis (EDA):
- **Univariate Analysis:** Studied the distribution of key features such as `season`, `temp`, and `weathersit` using histograms and boxplots.
- **Bivariate Analysis:** Analyzed the relationship between `cnt` and other features like `temp`, `yr`, and `season` using bar plots, box plots and correlation heatmaps.
- **Categorical Feature Analysis:** Examined categorical features such as `season` and `weathersit` to understand their influence on demand.

### Business Problem:

The core business problem revolves around making strategies to to prepare BoomBikes to cater to the people's needs once the situation gets better all around and stand out from other service providers and make huge profits.

#### Objective:
The objective of this project is to understand the factors affecting the demand for BoomBikes in the American market and build a multiple linear regression model for the prediction of demand for its shared bikes.

## Conclusions
- ### Conclusion:

A multiple linear regression model has been built to understand the impact of various features on demand for shared bikes. The key features affecting the demand are:

- **temp:** higher temperature reduces the demand
- **weathersit:** light rain and mist tends to reduce demand
- **windspeed:** higher windspeed tends to reduce demand
- **season:** demand is higher in winter and summer
- **yr:** demand is higher in 2019 as compared to 2018

**Adjusted R-squared value of 0.839, F-statistic 178.3, p-values of all variables lower than 0.05 and VIF of all variables much lower than 10** clearly indicaate a good overall fit of model and its stability. All the assumptions of linear model are validated


## Technologies Used

- **Python:** The primary programming language used for data analysis and model development.
- **Pandas (version 1.3.3):** For data manipulation and preparation, including handling missing values, feature engineering, and transforming the dataset.
- **NumPy (version 1.21.2):** For numerical computations, used primarily for array operations and statistical calculations.
- **Matplotlib (version 3.4.3):** For data visualization, used to create plots such as histograms, boxplots, and bar charts.
- **Seaborn (version 0.11.2):** High-level visualization library based on Matplotlib, used for statistical graphics like heatmaps and count plots.
- **statsmodels (version 0.14.4):** For statistical modeling and hypothesis testing, providing classes and functions for estimating and testing different statistical models.
- **scikit-learn (version 0.24.2):** For machine learning, including tasks such as regression, classification, clustering, and model evaluation, with tools for preprocessing, pipeline creation, and hyperparameter tuning.
- **Jupyter Notebook:** For writing and organizing the code, visualizations, and documentation interactively.

These technologies helped efficiently process, visualize, and analyze the data, providing key insights into loan default patterns.

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements

- Special thanks to the **UpGrad Data Science Program** for providing the framework and guidance for this project.

## Contact
Created by Prashant Saxena [prashantonly2024@gmail.com] - feel free to contact me!

