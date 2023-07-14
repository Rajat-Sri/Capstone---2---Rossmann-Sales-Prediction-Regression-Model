# Capstone-2-Rossmann-Sales-Prediction-Regression-Model
## **Supervised machine learning** is the types of machine learning in which machines are trained using well "labelled" training data, and on basis of that data, machines predict the output.

## Project Overview: 
In this project, we are working with a company called Rossmann that owns many drug stores in Europe. Our goal is to analyze their sales data and build a model that can predict sales for the next six weeks. By understanding what factors influence sales, we can provide recommendations to help the company grow and improve overall sales.

## Problem Statement: 
The problem we're trying to solve is predicting sales for Rossmann stores. We want to understand how factors like promotions, competition, holidays, and other factors affect sales. This knowledge will help us understand customer behavior and provide recommendations to boost sales.

## Data Understanding: 
We start by looking at the data we have. It includes information about the sales and various features of the stores, such as promotions, competition distance, and store types. We want to understand the structure of the data, the different types of information it contains, and if there are any missing values.

## Data Wrangling: 
We clean up the data by handling missing values. For example, if some data about competition distance is missing, we can estimate it using the median value of other distances. We also handle missing values related to competition opening and promo2 information. Additionally, we remove unnecessary columns with a lot of missing data.

## Data Analysis and Visualization: 
We explore the data to find patterns and insights. We look at sales trends over the years, sales on different days of the week, and how factors like store types and assortment levels relate to sales. We also examine the impact of promotions, sales during holidays, and other factors. By visualizing the data, we can better understand these relationships.

## Feature Engineering and Data Pre-processing: 
Feature selection techniques are applied to identify important features. Outliers are detected and treated using techniques such as Z-score and trimming. Data transformation, such as log transformation, is applied to handle skewed data. The dataset is split into training and testing sets, categorical variables are encoded, and data scaling is performed using techniques like StandardScaler.

## ML Model Implementation: 
We build three different models to predict sales: Linear Regression, Ridge Regression, and Decision Tree. These models use the available data to make predictions about future sales. We evaluate the performance of each model using metrics such as mean absolute error, mean squared error, and R2 score, which tells us how well the models fit the data.

## Cross-Validation and Hyperparameter Tuning: 
To ensure our models are reliable, we use techniques like cross-validation, which checks how well the models generalize to new data. We also tune the hyperparameters of the models, which are settings that can be adjusted to improve their performance.

## Model Selection and Evaluation: 
After evaluating the models, we choose the Decision Tree model as the best one based on its performance. This model shows how different factors contribute to sales and provides accurate predictions. We consider metrics like the R2 score, which tells us how much of the variation in sales is explained by our model.

## Conclusion and Recommendations: 
In conclusion, we have gained insights into what factors influence sales for Rossmann stores. We recommend increasing promotions, focusing on specific store types, and leveraging seasonal opportunities to boost sales. By understanding these patterns, Rossmann can make informed decisions to improve their overall growth and sales.
