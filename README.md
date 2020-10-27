# Project 2 - Ames Housing Data and Kaggle Challenge


## Overview

Concepts applied:
- basic statistics (distributions, confidence intervals, hypothesis testing)
- many Python programming concepts
- programmatically interacting with files and directories
- visualizations
- EDA
- working with Jupyter notebooks for development and reporting
- modeling(Lasso,Ridge,ElasticNet,Linear Regression)
- recursive feature elimination 

### Executive Summary

Partnering up with the City of Ames, we analyse homes sold between 2006 to 2010. Through exploratory data analysis, we have found several outliers in some of the features and would have been excluded from our model to increase the models accuracy.

Pandas,Sklearn and Statemodels are some of the tools that has been used in the exploratory data analysis and model predictions and derive at coefficients for each of the feature to explain their impact on prices. During the exploration of the data, we encountered missing values that had to be dealt with. We have ddecied to most replace missing values with 0 or by replacing them with mean and medians or other forms of inferential data imputing methods. We also converted some of the data into numerical form and one hot encoded them, to aid in the modeling process.

We used a total of 4 models(linear regression, Ridge, Lasso and ElasticNet), a recursive feature elimination was done to retreive the best 30 features that would predict the house prices. We use R2 and Square Root mean errors to compare the performance of model to select the best performer. We then used that best model type to make prediction on our test dataset.

### Problem Statement
To find out what home sellers could do to increase the prices of their houses and for homebuyers to ensure that the houses are appropriately priced.

### Dataset breakdown
[Ames Data Dictionary](http://jse.amstat.org/v19n3/decock/DataDocumentation.txt)

### Conclusion and recommendations
Using the 3 models(Ridge,Lasson,Linear Regression and ElasticNet) and a total of 128 features, it was found that Ridge performance the best with the the closest train and test R2 and RSMSE with only slight signs of underfiting, which may have been due to the limitaions of 30 features or lack of data on outliers towards the higher sales prices. From the 128 features, a recursive feature elimination was down to reduce the number of features to 30, with top 30 features, a Ridge model was performed and the model showed that it was only very slight underfitting in both R2 and RSMSE. The prediction on the test dataset was done and returned a score of 28963.69 which further proves that either/or our current dataset doesnt include enough data points and that 30 features may not be sufficent to predict house prices well.

There are some features in houses that would help homeonwers increase the prices of the houses they are trying to sell, such features include above groud living area. This would mean that owners could consider renovating their house to increase living area just as long as it costs 25000 or less for every square feet increased. Another feature that homeowners should change would be the overall quality of the house, as an increase in rating would lead to an increase in prices by about 17000. Lastly, homeowners can look into increasing the quality of their kitchens, as every increased rating, would increase the price by about 6500, as long as the cost of doing so is lesser. What I would suggest would be to do a the renovations all at the same time to try to increase the ratings and square footage of the different features to maximise the full potential of the house and acheive the best selling price.

Potential homeowers can also use thee features as a guide to see if the houses they are interested in are morderately priced by knowing which features greatly affect the price of the house. Using this information as a bargining chip to lower the prices of houses that are overvalued or buy houses that are undervaled and flip them for profit.




```python

```
