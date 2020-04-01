# Predicting Airfare Prices 
###### by Ibrahim Patel

![Alt Text](https://media.giphy.com/media/Btn42lfKKrOzS/giphy.gif)
## Executive Summary
I love to travel, and I have been on many planes in my life. I thought it would be fun to make a machine learning algorithm that could predict the price of an airplane ticket. I wanted to use data with features that were easy for the customer to "manipulate". There are features such as cabin class, date difference, departure part of day, and day of week etc. I liked using features like these because these are features the customers can "manipulate".
## Contents
1. [Introduction](#introduction)
    - [Problem Statement](#problem_statement)
    - [Dataset](#dataset)
2. [Analysis](#analysis)
    - [Data Cleaning](#data_cleaning)
    - [Exploratory Analysis](#exploratory_analysis)
    - [Modeling](#modeling)

## Introduction <a name="introduction"></a>
I first attempted to gather my data from a couple different sources such as the Kayak, Travelocity, and Flight Data Api. However, due to the time constraint, and difficulty scraping flight data, I ended up using a pretty good dataset for this project from Kaggle.com. With this data I began to answer the many questions I had about flight prices, and how certain features effect the price. The crux of this project comes from the machine learning algorithms I used to get my results.


### Problem Statement <a name="problem_statement"></a>
Since flying by air has become a very common means of transportation, the day old question arises "Can we predict the cost of an airplane ticket? ". I decided to do try my best and see if there is any way I can predict the price of an airplane ticket. With a dataset of 600 thousand observations and SK learn's machine learning algorithms this should be a piece of cake. 
### Dataset <a name="dataset"></a>
https://www.kaggle.com/lpisallerl/air-tickets-between-shanghai-and-beijing

## Analysis <a name="analysis"></a>

### Data Cleaning <a name="data_cleaning"></a>

I merged 2 different dataframes, dropped null values, and I dropped any outliers in the dataset. 

### Exploratory Analysis <a name="exploratory_analysis"></a>

I found that cabin class, airlines,day of the week, and part of day all have an effect on plane ticket prices. I also found out that the prices flucate a lot at different parts of the day. Noon has the highest average cost per ticket while night has the lowest. The biggest contributing factor to price is cabin class. This makes sense because the price distribution spread for an economy class ticket is significantly smaller than a business or first class ticket.

### Modeling <a name="modeling"></a>
I used these Machine Learning Algorithms for modeling my data.
- Linear Regression
- AdaBoost
- Gradient Boosting
- XG Boost
- Random Forest


