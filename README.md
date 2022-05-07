# Housing
Regression modeling and ML project on [Kaggle](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques) housing data.

#### Constraints
- Missing data
    - Kitchen
    - Bedroom

## Model

#### Algorithms
I use an average ensemble of 4 different models to generate final sales price prediction:
- Gradient Boosted Decision Tree
- Ridge Regression
- K-Nearest Neighbors
- XGBoost

#### Features
I break features down into 5 main categories: house, lot, location, and sale. I pull features directly from the [features.yml file](./features.yml). Refer to the file for more info on features used and their definitions.

## Methodology

#### 1. Preprocessing

###### Steps
1. `Clean` - clean data, handle null values
1. `Dummy` - create dummy variables for categorical fields
1. `Normalize` - normalize numerical data fields
1. `Select` - feature selection
1. `Split` - split training into fit and score sets

#### 2. Modeling

###### Steps
1. Select model type
    - `Gradient Boosted Decision Tree Regression (gbr)`
    - `Ridge Regression (ridge)`
    - `K-Nearest Neighbor Regression (knn)`
1. `Tune`
    1. Iterate through model parameter combinations
    1. Select model with best correlation coefficient
1. `Predict` - predict target variable for test data using best performing model

## Components

#### Data Manipulation
The numerical data is normalized using a standard scaler and dummy variables are created for categorical fields.

#### Feature Engineering & Selection
Feature Engineering: interaction terms

Feature Selection: backward selection


#### Modeling
Grid search CV (cross-validation)