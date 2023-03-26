# Capstone-2-Rossmann-Sales-Prediction-Regression-Model
## **Supervised machine learning** is the types of machine learning in which machines are trained using well "labelled" training data, and on basis of that data, machines predict the output.

## **Machine Learning Regression** is a technique for investigating the relationship between independent variables and a dependent variable. It’s used as a method for predictive modelling in machine learning, in which an algorithm is used to predict continuous outcomes.  

## **Sales forecasting** refers to the process of estimating demand for or sales of a particular product over a specific period of time. This project involves solving a real-world business problem of sales forecasting and building up a machine learning model for the same.

## **Problem Statement**

Rossmann operates over 3,000 drug stores in 7 European countries.Store sales are influenced by many factors, including promotions, competition, school and state holidays, seasonality, and locality etc. With thousands of individual stores and varied sales it is very difficult to understand customer behaviour and various other factors in general which are influencing sales and growth.

## **Business Objective**

We are provided with historical sales data for 1,115 Rossmann stores.Our goal here is to forecast the sales for six weeks for each store and to find out the factors influencing sales and recommend ways in order to over all company's growth and sales.

## **Approach** 

***Know your data***
* Merged dataset contains 1017209 rows and 18 columns.
* All columns are of Object,Integer or Float data types.
* There are lot of missing values in some columns which need to be handled moving forward.

***Data Wrangling***
*   Less than 1% data is missing in CompetitionDistance column, which is replaced with median as it will not affect data skewness.
*   More than 30% data is missing in CompetitionOpenSinceMonth and CompetitionOpenSinceYear columns which is replaced with mode values i.e. with most recurring values.
*  More than 40% data is missing from Promo2SinceWeek,Promo2SinceYear and PromoInterval columns which we have replaced with 0.
*  Changed data types of several columns from float to integer for better data representation.
*  Replaced object type '0' with integer type 0.

**Data Analysis and Visualization**

1. Sales trends over years
2. Sales treands of each year seperately,for better understanding.
3. Sales over different days of a week
4. Relationship between store type, assortment levels and sales 
5. Count of each store type
6. Total Customer counts for each store types 
7. Overall Sales treands for different store types
8. Customers preferance over different types of assortments
9. Sales of different types of assortments
10. Affect of promo over sales
11. Affect of extended promotions over overall sales  
12. Sales during state holidays
13. Sales during school holidays 
14. Checking for multicollinearity between independent features using correlation heatmap
15. Pair Plot visualization

**Solution to Business Objective**

  From our analysis we have found few areas of improvements which may definitely help in company's overall growth.These are - 
* Product promotions really boosted overall sales but it is also observed that extended promotions have negatively impacted sales in longer run.It is advisable not to use extended promotion much as they are cost ineffective and resulting in neagtive growth.
* B type stores has more assortments as compared to others as a result the revenue per store is significantly more than the others store types.Focus can be shifted towards establshing more B type stores.
* Store type A and D had most share of market so there is quite a lot of scope of improvements for type B and C to penetrate the market. 
* Some necessary changes can be done to improve sales even during holidays, as we observed demand on those days too, but due to closure of shops on holidays results in sudden decline of sales on those particular days.

**Hypothesis Testing**
 - Hypothetical Statement - 1
     - Null hypothesis (H0): Data follows a normal distribution.
     - Alternate Hypothesis (H1): Data does not follow a normal distribution.

 - Hypothetical Statement - 2
     - Null hypothesis (H0): Continous Data is highly correlated
     - Alternate Hypothesis (H1): Continous Data not correlated

 - Hypothetical Statement - 3
     - Null hypothesis (H0): Categorical Data is highly correlated
     - Alternate Hypothesis (H1): Categorical Data not correlated

**Feature Engineering & Data Pre-processing**
 - Handling missing values
 - Feature manipulation and selection
 - Handling outliers
 - Data Transformation
 - Data Splitting
 - Categorical Encoding
 - Data Scaling
 - Dimentionality Reduction
 - Handling imbalance

**ML Model Implementation,cross validation and hyperparameter tuning**
 - Model 1 - Linear Regression
 - Model 2 - Ridge Regression
 - Model 3 - Decision tree

**Saving Best performing model for deploynment**
 - Saving Model
 - Calling model and check model performance

## **Conclusion**

* There is a sudden jump in sales during november and december. This may be due to festivals like easter, christmas eve and new year.
*  Most of the store are closed on weekend ie saturday and sunday,but specially on sunday, as a result huge spike in sales could be observed on monday.
*  Product promotions really boosted overall sales but it is also observed that extended promotions have negatively impacted sales in longer run.
*  During Public holiday, easter and christmas most of the store remain close which result in significant drop in sales on those days.
*  Only Type b stores had all three kinds of assortment levels. It seems that like b type stores has more assortments as compared to others as a result the revenue per store is significantly more than the others store types.
* In 2014 from July to September we can notice close to 0 sales, this might be the time most shops were under refurbishment.
* Store type A and D had most share of market so there is quite a lot of scope of improvements for type B and C to penetrate the market. 

    **Recommendations**
* More stores should be encouraged for promotion. 
* Store type B should be increased in number.
* There's a seasonality involved, hence the stores should be encouraged to promote and take advantage of the holidays.
