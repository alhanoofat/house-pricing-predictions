# House Prices Prediction <br>

Problem Statement: In the real estate industry, it can be so complicated to determine a house price. That is because it depends on so many characterestics of the house itself. Therefore, in this project, we aquired a dataset containing 79 explanatory features describing almost every aspect of residential homes in Ames, Iowa, USA. After that, we built some regression models to predict each house price. Then, we selected the best model in terms of the test data score provided by Kaggle.

Here is the competition that we joined:
[House prices](https://www.kaggle.com/c/house-prices-advanced-regression-techniques)

A quick overview on two datasets' features, dataset and descriptions<br>

|Feature | Dataset | Description |
|---|---|---|
SalePrice |train|the property's sale price in dollars. This is the target variable that you're trying to predict.
MSSubClass|train/test| The building class
MSZoning|train/test|The general zoning classification
LotFrontage|train/test| Linear feet of street connected to property
LotArea|train/test|Lot size in square feet
Street|train/test| Type of road access
Alley|train/test| Type of alley access
LotShape|train/test| General shape of property
LandContour|train/test| Flatness of the property
Utilities|train/test| Type of utilities available
LotConfig|train/test|Lot configuration
LandSlope|train/test| Slope of property
Neighborhood|train/test| Physical locations within Ames city limits
Condition1|train/test| Proximity to main road or railroad
Condition2|train/test| Proximity to main road or railroad (if a second is present)
BldgType|train/test|Type of dwelling
HouseStyle|train/test| Style of dwelling
OverallQual|train/test| Overall material and finish quality
OverallCond|train/test|Overall condition rating
YearBuilt|train/test|Original construction date
YearRemodAdd|train/test|Remodel date
RoofStyle|train/test| Type of roof
RoofMatl|train/test| Roof material
Exterior1st|train/test| Exterior covering on house
Exterior2nd|train/test| Exterior covering on house (if more than one material)
MasVnrType|train/test| Masonry veneer type
MasVnrArea|train/test| Masonry veneer area in square feet
ExterQual|train/test| Exterior material quality
ExterCond|train/test| Present condition of the material on the exterior
Foundation|train/test|Type of foundation
BsmtQual|train/test| Height of the basement
BsmtCond|train/test|General condition of the basement
BsmtExposure|train/test|Walkout or garden level basement walls
BsmtFinType1|train/test| Quality of basement finished area
BsmtFinSF1|train/test| Type 1 finished square feet
BsmtFinType2|train/test| Quality of second finished area (if present)
BsmtFinSF2|train/test| Type 2 finished square feet
BsmtUnfSF|train/test|Unfinished square feet of basement area
TotalBsmtSF|train/test| Total square feet of basement area
Heating|train/test| Type of heating
HeatingQC|train/test| Heating quality and condition
CentralAir|train/test| Central air conditioning
Electrical|train/test| Electrical system
1stFlrSF|train/test| First Floor square feet
2ndFlrSF|train/test| Second floor square feet
LowQualFinSF|train/test| Low quality finished square feet (all floors)
GrLivArea|train/test| Above grade (ground) living area square feet
BsmtFullBath|train/test| Basement full bathrooms
BsmtHalfBath|train/test| Basement half bathrooms
FullBath|train/test| Full bathrooms above grade
HalfBath|train/test| Half baths above grade
Bedroom|train/test| Number of bedrooms above basement level
Kitchen|train/test| Number of kitchens
KitchenQual|train/test| Kitchen quality
TotRmsAbvGrd|train/test| Total rooms above grade (does not include bathrooms)
Functional|train/test| Home functionality rating
Fireplaces|train/test| Number of fireplaces
FireplaceQu|train/test| Fireplace quality
GarageType|train/test| Garage location
GarageYrBlt|train/test| Year garage was built
GarageFinish|train/test| Interior finish of the garage
GarageCars|train/test| Size of garage in car capacity
GarageArea|train/test| Size of garage in square feet
GarageQual|train/test| Garage quality
GarageCond|train/test| Garage condition
PavedDrive|train/test| Paved driveway
WoodDeckSF|train/test| Wood deck area in square feet
OpenPorchSF|train/test| Open porch area in square feet
EnclosedPorch|train/test| Enclosed porch area in square feet
3SsnPorch|train/test| Three season porch area in square feet
ScreenPorch|train/test| Screen porch area in square feet
PoolArea|train/test|Pool area in square feet
PoolQC|train/test|Pool quality
Fence|train/test| Fence quality
MiscFeature|train/test| Miscellaneous feature not covered in other categories
MiscVal|train/test| $Value of miscellaneous feature
MoSold|train/test| Month Sold
YrSold|train/test| Year Sold
SaleType|train/test| Type of sale
SaleCondition|train/test| Condition of sale


## Conclusion and Recommendations <br>
In this project, We were solving the problem of setting a house price based on the features of that house. We got the dataset of almost 3,000 houses in Iowa State along with 79 of their features. We splitted the data into train and test data. After that, we calculated the baseline by creating a model that predicts the house prices as a constant, which is the mean of all house prices in the train data. Then, we trained several models; Linear regresson after manually selecting the features, Lasso regression on the entire dataset, Ridge regression on the entire dataset, KNN regression, and decision tree regression. After that, we submitted the predictions of each model individually to Kaggle and got the score of each. The best score was for Lasso regression.<br>
For Lasso regression, which worked best for our dataset, here are the features that had the highest effects on the sale price of the houses:<br>
- OverallQual
- GrLivArea
- GarageCars
- GarageArea
- TotalBsmtSF
- 1stFlrSF
- FullBath
- BsmtQual_Ex
- TotRmsAbvGrd
- YearBuilt

In the end, we recommend that anyone considering getting a house to think about this list and priorities their options, because these are the features that have the strongest effects on the sale price <br>
Here is our notebook on kaggle <br>
<a href="https://www.kaggle.com/mzoonalwalmani/project2-part1/edit/run/22752787">House Prices Prediction</a> <br>
Our Kaggle score we got for the best model is : 0.13909
