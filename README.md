# Housing
Regression modeling and ML project on [Kaggle](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques) housing data.

## Model

#### Algorithms
I use an ensemble of 3 different models to generate final sales price predicition:
- Gradient Boosted Decision Trees (GBDT)
- Linear Regression
- K-Nearest Neighbors

#### Features
I break down features into 3 main categories:

1. House
    - MSSubClass (cat)
    - Utilities (cat)
    - BldgType (cat)
    - HouseStyle (cat)
    - OverallQual
    - OverallCond
    - YearBuilt
    - YearRemoAdd
    - RoofStyle (cat)
    - Exterior1st (cat)
    - Exterior2nd (cat)
    - ExterQual (cat)
    - ExterCond (cat)
    - Foundation (cat)
    - 
1. Location
    - MSZoning (cat): Identifies the general zoning classification of the sale
    - Neighborhood (cat)
    - Condition1 (cat)
    - Condition2 (cat)
    - 
1. Lot
    - LotArea: Lot size in square feet
    - Street (cat): Type of road access to property
    - LandContour (cat)
    - LotConfig (cat)
    - LandSlope (cat)
    - 
