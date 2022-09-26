# Description

This repository contains the code for the project on "Analysis of Grain and Seed Oil Production in Ukraine Prior to Recent Russion Invasion". This project
resulted in a paper which was submitted to the IBDAP 2022 conference.

## Project Goal

The goal of the project was to identify the most suitable machine leanring algorithm to predict the production level of grain or seed oil in Ukraine.

## Methods & Tools Used

There were two parts to this project. The first part is the exploratory data analysis that gave us insights into which variables have (or don't have) influence on the amount of grain and seed oil being produced in Ukraine in a year. There were three components of the EDA: i) data preprocessing - understanding the data and dealing with the missing/null values in the table(s), ii) identifying outliers - are the numerical variables in the data set (close to being) normally distributed or are they highly skewed? and iii) correlation analysis/heatmap - how correlated are the predictor variables to the dependent variable (production) and to each other? The last component of EDA is how the first part of the project segued into the second part. This is because the correlation heatmap created the ground for Feature Selection because the data is input into the machine learning models. The second part of the project was actually building and testing different machine learning models. Three linear models (multivariable reg., lasso reg., ridge reg) and three non-linear models (decision tree, random forest, kNN) were trained and tested. Each model was run for 1000 iterations (with 1000 different train-test splits of the same input data) and the average testing error was taken at the end.

## Results

Lasso Regression was found to be the best performing model out of the six, as it had both the smallest training and testing errors. 

## How Is This Project Useful?
