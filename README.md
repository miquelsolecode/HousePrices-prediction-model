# HousePrices-prediction-model

Housing price prediction model:

INTRODUCTION: 

A lot of times, investors will use Machine learning models to predict fluctuations on prices, stock, market value... But sometimes they use this models to create an image of the price something should have based on certain characteristics, and price it properly to maximaze it’s exploitation; for this case, we got a database with properties in the State of California, along with it’s characteristics in its block, like population, population, median income, its proximity to the coast... and the median House value, the trait we are traying our future model to predict.



DATA CLEANING AND PREAPARATION: 

First, we got rid of those columns with information we knew we wouldn’t be needing, like the total number of bedrooms (kind of redundant, since total number of rooms is another feature), or the proximity the property has to the sea (since its criteria was confusing); and then we proceeded to make a box plot of each existent feature left to see its Distribution.
Doing this, we discovered that each column had a normal amount and spread of outliers, and that specifically the column of population had 2 outliers way out of the “normal range for an outlier” seeing the variation spread of all the features, so we got rid of these outliers in order to make the model more accurate.


MODEL CREATION AND PERFORMANCE ANALYSIS:
We used a traint-test based model as a base to create multiple regression models, each one with both Standard and Minmax scalers, and best te accuracy of the model based mainly on the R squared value, supporting our choice by making a scatter plot out of each model to have a visual representation. Our conclusion was that the model with better performance was the polinomial regression one.
