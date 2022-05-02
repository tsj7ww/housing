# Housing
Regression modeling and ML project on [Kaggle](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques) housing data.

#### Constraints
- Missing data
    - Kitchen
    - Bedroom

## Model

#### Algorithms
I use an ensemble of 3 different models to generate final sales price prediction:
- Gradient Boosted Decision Tree (GBDT)
- Ridge Regression
- K-Nearest Neighbors

#### Features
I break features down into 5 main categories: target, house, lot, location, and sale. I pull features directly from the [features.md file](./features.md) in order to ensure accuracy of the documentation. Refer to the file for more information on features used and their definitions.

## Methodology

#### 1. Preprocessing

###### Steps
1. `Combine` - combine train and test sets for data preprocessing
1. `Clean` - clean data
1. `Dummy` - create dummy variables for categorical fields
1. `Select` - feature selection
1. `Normalize` - normalize numerical data fields
1. `Wrangle` - wrangle data into fit, score, and test sets

#### 2. Modeling (currently Prediction)

###### Steps
1. `Gradient Boosted Decision Tree Regression (gbr)`
1. `Ridge Regression (ridge)`
1. `K-Nearest Neighbor Regression (knn)`
1. `Predict` - predict target variable for test data using an ensemble of previously stated models and taking the average output
