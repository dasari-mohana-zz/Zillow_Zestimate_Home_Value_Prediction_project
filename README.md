# Zillow_Zestimate_Home_Value_Prediction_project

## Business Objective:

Buying a house that suits their choices is every person's desire, and it is thus known as their dream house. One considers several aspects while purchasing a home, starting from the budget, the location, the number of rooms available, and many more. But how to find a house that satisfies one's requirements?  This is not a quick and easy task.

But no need to worry; homebuyers can nowadays find their dream home with a click of a button. Zillow is a popular estimator for house evaluation available online. It is considered one of the top real estate marketplaces for buying a house in the United States. Zillow's Zestimate allows the homebuyers to search for a home that satisfies their location, area, budget, etc.

The Zillow Zestimate provides the homebuyers with information on the actual worth of the house based on public data. The accuracy of the Zestimate information depends on the location and availability of the data of a specific area. Hence the more data available, the more is the accuracy of the Zestimate.       


## Aim:

To predict the sale prices of the houses and improve the log error i.e. the error due to the difference between the actual and the predicted home values.

## Data Description
The Zillow Zestimate dataset is a dataset from Kaggle, that is used for making future sales predictions and improving the log error.

There are two datasets available they are:
	1. train_2016 – This dataset consists of the target variable i.e. the logerror
	2. properties_2016 – Contents all the features related to the property/home.
	
There are around 60 attributes in the dataset on basis of which the model can be built.

Some of the important features amongst them are as follows:
	
1. train_2016:
  1. parcelid - Unique identification for every parcel
  2. transactiondate - The date on which the home was sold
  3. logerror - The residual between the actual and the predicted sale price of homes. (Target Array)

2. properties_2016:
  1. parcelid - Unique identification for every parcel (common in both the datasets)
  2. bathroomcnt - Total number of bathrooms in the house
  3. bedroomcnt - Total number of bedrooms in the house
  4. buildingqualitytypeid - This gives the quality assessment of the building ranging from best to worst.
  5. finishedsqaurefeet12 - Finished living area of the house.
  6. fips - This stand for Federal Information Processing Standard code
  7. latitude & longitude - longitude and latitude of the home location
  8. propertylandusetypeid - This gives the type of land the property is zoned for.
  9. regionidcity - The city in which the property is situated.
  10. regionidcounty - The county where the property is situated.
  11. regionidzip - This provides the zip code for the location of the property.
  12. taxamount - Property tax for each assessment year

## My Approach

1. Importing the required libraries and reading the dataset.
	a.Merging of the two datasets
	b.Understanding the dataset
	
2. Exploratory Data Analysis (EDA) –
	a.Data Visualization
	
3. Feature Engineering
	a.Duplicate value removal
	b.Missing value imputation
	c.Rescaling of incorrectly scaled data
	d.Standardization
	e.Encoding of categorical variables
	f.Generation of new feature wherever required.
	g.Dropping of redundant feature columns
	h.Checking for multi-collinearity and removal of highly correlated features
	i.Check for the outliners and removal of outliers.
	
4. Model Building
	a.Performing train test split
	b.Feature Scaling
	c.Dropping features if necessary
	d.Linear Regression Model
	e.Elastic Net
	f.Ridge Regression
	g.Lasso Regressor
	h.XGBoost Regressor
	i.Adaboost Regressor
	j.Gradient Boosting Regressor
	k.Decision Tree Regressor
	l.Random Forest Regressor
	
5. Model Validation
	a.Mean Absolute Error
	b.Mean Squared Error
	c.Root Mean Squared Error
	
6. Hypermeter Tuning (GridSearchCV)
	a.For Random Forest Regressor
	
7. Checking for Feature Importance

8. Creating the final model and making predictions

9. Conclusion


