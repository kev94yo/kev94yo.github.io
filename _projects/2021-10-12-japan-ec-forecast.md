---
layout: project
title: Japan Electricity Consumption Forecasting
caption: Forecasting electricity consumption of Tokyo based on time series data and features.
description: >
  Extensive exploratory data analysis was done to filter out relevant features.
date: '2021-10-12'
image: 
  path: /assets/img/projects/japan-ec-forecast-xgboost.jpg
  # srcset: 
  #   1920w: /assets/img/projects/qwtel.jpg
  #   960w:  /assets/img/projects/qwtel@0,5x.jpg
  #   480w:  /assets/img/projects/qwtel@0,25x.jpg
links:
  - title: Link
    url: https://github.com/kev94yo/japan-electricity-forecasting
# accent_color: '#4fb1ba'
# accent_image:
#   background: '#193747'
# theme_color: '#193747'
sitemap: true
---

This personal project was for my thesis qualification exam, to prove my skills as a data scientist.
It is on forecasting electricity consumption based on time series data and features.

## Motivation
1. Produce more accurate electricity consumption forecasts
2. Successful predictions can lead to less energy waste
  - Better plans for generating energy supply
  - Meeting customers' energy demand

<p align="center">
  <img src="../../assets/img/projects/japan-ec-forecast-data.jpg" alt="data" width="500">
</p>
Final data after preprocessing.
{:.figure}

## Project Outline
- **Data Preprocessing**
  - Added features using datetime and holiday information
  - Concatenated weather data by left joining on the electricity consumption dataset
- **Exploratory Data Analysis (EDA)**
  - Visualized consumption by hour, day, month and year to seek insights on potential patterns
  - Produced heatmap and boxplot to search correlations between holiday and consumption
- **Model Training, Evaluation**
  1. Ridge Regression: Used to model linear relationships between multiple features and one response
  2. SARIMAX: Used for comparison between traditional time series model and machine learning model
  3. XGBoost: Extreme gradient boosting, a form of boosting ensemble method
- **Prediction**
  - Visualized consumption predictions at an hourly level for the next year
- **Presentation**: Held a talk session about the project using powerpoint slides

<p align="center">
  <img src="../../assets/img/projects/japan-ec-boxplot.jpg" alt="boxplot" width="600">
</p>
Boxplot of average consumption when weekday is working or non-working. Used for EDA.
{:.figure}

## Result
- Produced successful predictions with XGBoost, with an R-squared value over 0.9
  - Successful feature selection based on EDA
- Offered insightful comparisons between two machine learning models and one time series model
- Selected as *Best Project Showcase* by the all the professors of GSDS

## Obstacles
Here are a few important obstacles I faced during this project.
- **Feature Selection**
  - I had to select only relevant features to use for the model in order to not hinder performance
  - **Solution**: Performed extensive EDA to analyze correlations between various features and electricity consumption.
- **Multiple Seasonalities**
  - SARIMAX not great at handling multiple seasonalities
  - **Solution**: Used fourier transformation (representing a periodic function as sum of sine and cosine functions) to capture multiple seasonalities
  of year, week and day.

## Languages & Tools
Here are the languages and tools used for this project.
- Python, Matplotlib, Seaborn, SKLearn
- Jupyter Notebook
- Microsoft Powerpoint
- Git

## Links
*  **Github**: <a href="https://github.com/kev94yo/japan-electricity-forecasting" target="_blank">https://github.com/kev94yo/japan-electricity-forecasting</a>
*  **Slides**: <a href="https://docs.google.com/presentation/d/1fCRtAoJKXoLXrs9vK84Dp94kusPvB40U/edit?usp=sharing&ouid=100543530057756188294&rtpof=true&sd=true" target="_blank">https://docs.google.com/presentation/d/1fCRtAoJKXoLXrs9vK84Dp94kusPvB40U/edit?usp=sharing&ouid=100543530057756188294&rtpof=true&sd=true</a>