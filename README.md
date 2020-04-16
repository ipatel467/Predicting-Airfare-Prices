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
    - [Results](#results)

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

I found that cabin class, airlines,day of the week, and part of day all have an effect on plane ticket prices. 

I also found out that the prices flucate a lot at different parts of the day. Noon has the highest average cost per ticket while night has the lowest. The biggest contributing factor to price is cabin class. This makes sense because the price distribution spread for an economy class ticket is significantly smaller than a business or first class ticket.

This is the average cost of a ticket by cabin class.
![Screen Shot 2020-04-15 at 6 31 26 PM](https://user-images.githubusercontent.com/52756457/79399221-6198d400-7f48-11ea-9aff-61b147b5c5b7.png)

However, airplane tickets prices are dynamic due to their cost always changing. There is no "One Price Fits All".

Since airplane prices are constantly changing here is a distibution of prices by cabin class.
![Screen Shot 2020-04-15 at 6 31 17 PM](https://user-images.githubusercontent.com/52756457/79399276-8725dd80-7f48-11ea-8dfd-aab17065f8af.png)

We can see that there is a much smaller spread for economy than there is for bussiness and first class.






Here is how the price of a ticket is affected by the day of the week.

![Screen Shot 2020-04-15 at 6 31 43 PM](https://user-images.githubusercontent.com/52756457/79399141-2e564500-7f48-11ea-8be9-9e8b9b5cac7d.png)

We can see that Saturday is the cheapest day to fly for all cabin classes. The most economic approach would be to fly on Saturday because all classes have lower prices.








### Modeling <a name="modeling"></a>
I used these Machine Learning Algorithms for modeling my data.
- Linear Regression
- AdaBoost
- Gradient Boosting
- XG Boost
- Random Forest

![Alt Text](https://media.giphy.com/media/h2e9cR28Wf82Y/giphy.gif)



### Results <a name="results"></a>

After running multiple models through an iterative process the model that gave me the best results was an XG Boost. I got an R^2 of .724 which means my model captures 72% of the data needed to explain the price of an airplane ticket. 

![Screen Shot 2020-04-15 at 6 55 16 PM](https://user-images.githubusercontent.com/52756457/79400056-b2a9c780-7f4a-11ea-8c97-a2f365996959.png)

To make my model better I have to decrease the MSE and RMSE, and increase the R^2.

I will work on this project in the future, and try my best to make my model better by doing more feature engineering.


