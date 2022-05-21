# Phase 2 Project

## Overview 
In this project, we explored the relationship between Price and other variables in order to identify investment opportunities in King County. The data set includes several columns to describe 21,597 properties in the Seattle, Washington area. 

## Business and Data Understanding
There are many opportunities in real estate for investment. Some investments focus on generating passive income by collecting rent from tenants, while other investments are short term, known as "flipping." The process of flipping involves buying properties in poor condition, renovating them, and selling them for a profit within 6 to 8 months. 

We decided to focus on Real Estate investors who wanted to flip properties. This audience is interested in identifying the properties with the most potential for growth. 

Our data showed that there was a correlation between the Condition of the property and the price at which it was sold. There were also several variables that were important indicators of the price of a property, including Square Feet, Grade, and Location. Many of our variables were approximately normally distributed, but for the ones that weren't we used logarithmic transformations to improve our results.

## Modeling
We decided to build a model that predicted the price of houses in "Good" or better condition, and use it on houses in "Bad" condition. This would give us a "Predicted Price" for the houses in "Bad" condition if they were to be renovated.

Our model is a Multi-Linear Regression model, using several predictors to give us a prediction of the price of the houses if they were renovated. We were able to get to an R-squared of 0.869, showing that this model is accounting for 87% of the variance we see in Price.

We conducted a Logarithmic Transformation to the "Price" column in order to counteract the skew and improve our model, and we removed the top 5% of the most expensive houses to remove the outliers. We formatted the Zip code as a Nominal Categorical variable.

## Conclusion
We identified 10 optimal investment properties. The total investment cost (property + renovation cost) is $3,889,200. The predicted Sale price once the houses were renovated according to the model is $5,435,745. The total predicted profit is $1,546,545. 

We also used Folium to plot the locations of these properties on the map. 