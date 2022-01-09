# Bike Sharing Assignment
> Building Machine Learning model to predict the Bike hire using Supervised learning and linear Regression model


## Table of Contents
* [Data Understanding](#Data-Understanding)
* [Data Preparation and Data Cleaning](#Data-Preparation-and-Data-Cleaning)
* [Creating Dummy Variable](#Creating-Dummy-Variable)
* [Exploratory Data Analysis and data visualisation](#Exploratory-Data-Analysis-and-data-visualisation)
* [Rescaling the features](#Rescaling-the-features)
* [Building the model](#Building-the-model)
* [Evaluate  and rebuild the model](#Evaluate-and-rebuild-the-model)
* [Model assessment and Prediction](#Model-assessment-and-Prediction)

<!-- You can include any other section that is pertinent to your problem -->

## Data Understanding
-	understand each feature and the importance and how they can impact the target variable. Which are independent variable and dependent variable so on

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Data Preparation and Data Cleaning:
-	Check for missing values and junk values, if any columns have more than 50% missing values then drop those columns. 
And fill the missing values with mean/mode
-	Assess which are important and which are unwanted feature.
Remove all unwanted columns from the dataset

## Creating Dummy Variable:
-	I identify the categorical variables, and convert them into numerical representation by crating dummy variables and  It is import to drop first column because it reduces the number columns for building correlation among dummy variables. The first column can be derived from the remaining variable and it has no added value, hence it is better to remove it.
-	Always if N levels of predictor variable are there then we need n-1 dummy variables
-	
## Exploratory Data Analysis and data visualisation:
-	Understand the impact of each and every feature how they change the target variable.. data visualisation will help to understand correlation between variables. Plotting pair-plot and boxplot and correlation matrix we can understand the relation.
Rescaling the features:
-	Usually the collected data will be in different levels, units and magnitude. If the scaling is not done one may end up build incorrect modelling because different units and mangitudes. Since the numeric variable are represented in different ranges it will be hard to work on larger numbers so we need to first rescale the value to lesser range for building easy and fast model
-	We will have two rescaling methods
o	Minmaxscaling ( we can use this to remove outliers as the all the data are scaled between 0-1)
o	Standardization scaling

## Building the model:
-	split dataset into the train and test data
-	add constant
-	create linear model using Ordinary Least Square
-	fit the model
-	
## Evaluate  and rebuild the model:
-	when there are multicollinearity we need to use different approaches to build the model
o	we can build the model with all the variable
o	We can build model by adding variable one by one and check R^2 value to check significance
o	Use RFE method to improve R^2 value by eliminating the feature which has high P value and High VIF (which indicate. Significance and Variance)  

## Model assessment and Prediction
-	using Residual Analysis a check error terms are normally distributed or not by plotting the distplot 
-	Predict the value of target variable using the final model

## Conclusions
 The linear regression model suggest the following are the 3 major indicator to predict the bike hire

Temp : Temperature with highest value of coefficient of '0.568327' indicates the a unit increase in temperature will increse the bike hires by 0.0568327 units.
Yr : Year with second highest coefficient value indicate each year to year potential grow in the number of bike hire by '0.231340' units
weathersit_3: Weather situation 3 indicates the negative correlation means with a unit increase in weather_sit3 there is a decrease in the bike hire by 0.316638 units

To increase the number of Bike hire it is suggested to consider the above key features and also the follwing features

windspeed: A coefficient value of ‘-0.153306’ indicated that, a unit increase in windspeed variable decreases the bike hire numbers by 0.155191 units.
season_4 (winter): A coefficient value of ‘0.119733’ indicated that w.r.t season_4, a unit increase in season_4 variable increases the bike hire numbers by 0.119733 units.


<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Contact
Created by [@Arunkumaranup] - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project --># ML_Bike_Sharing_Assignment
