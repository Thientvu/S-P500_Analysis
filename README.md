# S&P 500 Index Analysis and Forecasting

This repository contains a detailed analysis of the historical performance of the S&P 500 index and predictions of future trends using machine learning techniques. The goal of this study is to help investors make informed decisions and manage their portfolios effectively.

## Table of Contents

1. [Introduction](#introduction)
2. [Data Description](#data-description)
3. [Data Preprocessing](#data-preprocessing)
4. [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
5. [Methodology](#methodology)
6. [Model Training](#model-training)
7. [Results](#results)
8. [Limitations & Future Work](#limitations--future-work)
9. [Conclusion](#conclusion)

## Introduction

**Problem Statement:**  
The goal of this study is to analyze the historical performance of the S&P 500 index and predict future trends using machine learning techniques.

**Objective:**

- Analyze the historical price and volume data of the S&P 500.
- Calculate moving averages and other technical indicators.
- Forecast future prices using the Prophet model.

**Importance:**  
Understanding the trends and making accurate predictions can help investors make informed decisions and manage their portfolios effectively.

## Data Description

**Data Source:**  
The dataset is sourced from [Kaggle](https://www.kaggle.com/datasets/eli2022/yahoo-finance-apple-inc-gspc) and contains historical stock market data for the S&P 500 index.

**Data Overview:**  
The data spans from January 11, 2017, to May 29, 2024, including columns such as date, high, low, open, close, volume, adjusted close, RSI, daily return, volume change, lag values, and trend.

## Data Preprocessing

**Data Cleaning:**

- No missing values were found in the dataset.
- No duplicate records were present.

**Data Transformation:**

- Selected relevant columns: date, high, low, open, close, and volume.
- Converted the formatted date column to datetime format.

**Feature Engineering:**

- Created columns for 14-day, 50-day, and 200-day moving averages.

## Exploratory Data Analysis (EDA)

**Initial Analysis:**

|  | open | low | high | low | volume |
| --- | --- | --- | --- | --- | --- |
| count | 1857.000000 | 1857.000000 | 1857.000000 | 1857.000000 | 1.857000e+03 |
| mean | 3519.564660 | 3498.878890 | 3538.908257 | 3498.878890 | 4.079932e+09 |
| min | 2267.780029 | 2191.860107 | 2271.780029 | 2191.860107 | 1.296530e+09 |
| 25% | 2779.820068 | 2761.729980 | 2789.800049 | 2761.729980 | 3.461920e+09 |
| 50% | 3384.560059 | 3366.840088 | 3399.959961 | 3366.840088 | 3.873100e+09 |
| 75% | 4229.339844 | 4201.640137 | 4257.160156 | 4201.640137 | 4.445260e+09 |
| max | 5340.259766 | 5302.399902 | 5341.879883 | 5302.399902 | 9.976520e+09 |
| std | 822.991396 | 818.767849 | 827.437443 | 818.767849 | 1.002106e+09 |

**Historical Data Analysis:**

- Plotted historical price and trading volume for each year from 2017 to 2024.
        
- Calculated average daily trading volume for each year.
    
    | Year | Average Daily Trading Volume |
    | --- | --- |
    | 2017 | 3,416,059,061 |
    | 2018 | 3,634,742,988 |
    | 2019 | 3,558,549,643 |
    | 2020 | 4,922,448,419 |
    | 2021 | 4,417,139,921 |
    | 2022 | 4,617,723,068 |
    | 2023 | 4,013,728,760 |
    | 2024 | 3,975,197,087 |

## Methodology

**Model Selection:**  
Prophet is a forecasting tool created by Facebook for predicting time series data. It is designed to handle different patterns in the data, such as daily, weekly, and yearly trends, as well as holidays.

## Model Training

**Training Process:**

- The Prophet model was trained on historical closing prices and used to forecast future prices for one year ahead.

## Results

**Findings:**

- The model predicted a continuous upward trend for the S&P 500 index.
- The forecasted prices for May 2025 ranged between 5372.91 and 6705.43.
        
## Limitations & Future Work

**Limitations:**

- The model does not account for unexpected market shocks or economic events.
- Forecasting accuracy decreases with longer prediction horizons.

**Future Work:**

- Incorporate additional features such as economic indicators and sentiment analysis.
- Explore other forecasting models and compare their performance with Prophet.

## Conclusion

- The study provided a detailed analysis of the S&P 500 historical data and a forecast for future prices using the Prophet model.
- The case study also offers a reliable method for predicting stock prices, beneficial for investors and financial analysts.

## Acknowledgements

- [Kaggle](https://www.kaggle.com/datasets/eli2022/yahoo-finance-apple-inc-gspc) for the dataset.
- Facebook for developing the Prophet model.

