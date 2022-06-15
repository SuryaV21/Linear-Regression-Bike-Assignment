# Linear Regression Project 

## Table of Contents
* [Problem Statement](#problem-statement)
* [Technologies Used](#technologies-used)
* [Data Cleaning](#data-cleaning)
* [Analysis Flow](#analysis-flow)
* [Model Creation and Analysis](#Model_Creation_and_Analysis)
* [Conclusions](#conclusions)

<!-- You can include any other section that is pertinent to your problem -->

## Problem Statement
-A bike-sharing system is a service in which bikes are made available for shared use to individuals on a short term basis for a price or free. Many bike share systems allow people to borrow a bike from a "dock" which is usually computer-controlled wherein the user enters the payment information, and the system unlocks it. This bike can then be returned to another dock belonging to the same system.

## Technologies Used
- Pandas
- numpy
- Seaborn
- Matplotlib
- Sklearn
- stats



## Data Cleaning
- - Dataset contains 730 rows and 16 columns without any null values
- we have full date and split year and month columns. we can delete date column to avoid data duplication
- we have data type issues. Few of the variable are categorical however, because of numerical classification columns are treated as numerical instead of categorical
- Instant is a seq number and it has no meaning. We can drop that column
- Casual and registered numbers are count of different users as the requirement is to identify the demand for shared bikes. so these columns are not required
- creating the dummy variables after converting the respective variable data type into object

## Analysis Flow
- Univariate analysis was performed on categorical and numerical variables respectively
- Bivariate analysis was performed on numerical and categorical data respectively
- By looking at the pair plot Temp and atemp variable are highly correlated and directly proportional
- - Bookings are more in normal days than holidays
- Season 3 is having booking and then season 4 followed by season 2. Season 1 has very low bookings
- Booking happened during Weathersit 1 (Clear, Few clouds, Partly cloudy, Partly cloudy) with average of 4500 
- during 5,6,7 mothns we can see consistent average booking of 4500 per month and in march it reached max booking of 8000 and in october it has no booking
- After the correlation plot, temp and atemp are highly correlated. Due to this we dropped the atemp variable
- We have applied scaling to the numerical variable to bring them into a normal range by applying minmax scalar

## Model Creation and Analysis
- Divide the data into train and test using train_test_split function. Train will have 70% data and test will have 30% data
- Using SKLearn linear regression model we develop the model to verify the variable and check the variables which are related using Recurrsive Feature Ellimination (RFE)


## Conclusions
- Training model accuracy is 82% 
- Test data model accuracy is 79%
-	Bookings are more in normal days than holidays
-	Season 3 is having booking and then season 4 followed by season 2. Season 1 has very low bookings
-	Booking happened during Weathersit 1 (Clear, Few clouds, Partly cloudy, Partly cloudy) with average of 4500 
-	during 5,6,7 mothns we can see consistent average booking of 4500 per month and in march it reached max booking of 8000 and in october it has no booking




## Contact
Created by [@https://github.com/SuryaV21]
 - feel free to contact me!
