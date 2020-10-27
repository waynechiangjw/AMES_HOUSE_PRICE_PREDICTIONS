# Project 2 - Ames Housing Data and Kaggle Challenge


## Overview

Concepts applied:
- Basic statistics (distributions, confidence intervals, hypothesis testing)
- Many Python programming concepts
- Programmatically interacting with files and directories
- Visualizations
- Exploratory Data Analysis
- Working with Jupyter notebooks for development and reporting
- Modeling(Lasso,Ridge,ElasticNet,Linear Regression)
- Recursive feature elimination 

### Executive Summary

Partnering up with the City of Ames, we analyse homes sold between 2006 to 2010. Through exploratory data analysis, we have found several outliers in some of the features and would have been excluded from our model to increase the models accuracy.

Pandas,Sklearn and Statistics Models are some of the tools that have been used in the exploratory data analysis and model predictions and derive at coefficients for each of the features to explain their impact on prices. During the exploration of the data, we encountered missing values that had to be dealt with. We have decided to most replace missing values with 0 or by replacing them with mean and medians or other forms of inferential data imputing methods. We also converted some of the data into numerical form and one hot encoded them, to aid in the modeling process.

We used a total of 4 models(linear regression, Ridge, Lasso and ElasticNet), a recursive feature elimination was done to retrieve the best 30 features that would predict the house prices. We use R2 and Square Root mean errors to compare the performance of the model to select the best performer. We then used that best model type to make predictions on our test dataset.


### Problem Statement
We are a team of Data Scientists engaged by the City of Ames to help predict the prices of houses based on their characteristics. The team would be using linear regression models based on data given by the City to predict housing sale prices. 

This analysis and prediction would help potential buyers and sellers by giving them a better understanding of the property market, enabling them to make better informed decisions.(i.e. Buying undervalued houses and renovating them to sell them for profit)

In this project, there will be several linear regression techniques such as Linear Regression, Lasso Regression, Ridge Regression and ElasticNet Regression. Recursive feature elimination will also be deployed to identify the top 30 features that are the best predictors of house prices in the City of Ames.  We will be using R2 and Square Room error to compare the performance of the different models.

### Dataset breakdown
[Ames Data Dictionary](http://jse.amstat.org/v19n3/decock/DataDocumentation.txt)

### Conclusion and recommendations
Using the 3 models(Ridge,Lasso,Linear Regression and ElasticNet) and a total of 128 features, it was found that Ridge performance the best with the the closest train and test R2 and RMSE with only slight signs of underfitting, which may have been due to the limitations of 30 features or lack of data on outliers towards the higher sales prices. From the 128 features, a recursive feature elimination was done to reduce the number of features to 30, with top 30 features, a Ridge model was performed and the model showed that it was only very slight underfitting in both R2 and RMSE. The prediction on the test dataset was done and returned a score of 28963.69 which further proves that either/or our current dataset does not include enough data points and that 30 features may not be sufficient to predict house prices well.


There are some features in houses that would help homeowners increase the prices of the houses they are trying to sell, such features include above ground living areas. This would mean that owners could consider renovating their house to increase living area just as long as it costs 25000 or less for every square feet increased. Another feature that homeowners should change would be the overall quality of the house, as an increase in rating would lead to an increase in prices by about 17000. Lastly, homeowners can look into increasing the quality of their kitchens, as every increased rating, would increase the price by about 6500, as long as the cost of doing so is lesser. What I would suggest would be to do the renovations all at the same time to try to increase the ratings and square footage of the different features to maximise the full potential of the house and achieve the best selling price. 

Potential homeowners can also use these features as a guide to see if the houses they are interested in are moderately priced by knowing which features greatly affect the price of the house. Using this information as a bargaining chip to lower the prices of houses that are overvalued or buy houses that are undervalued and flip them for profit.





```python

```
