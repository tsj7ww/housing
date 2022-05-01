# Housing
Regression modeling and ML project on [Kaggle](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques) housing data.

#### Constraints
- Missing data
    - Kitchen
    - Bedroom

## Model

#### Algorithms
I use an ensemble of 3 different models to generate final sales price prediction:
- Gradient Boosted Regression (GBDT)
- Linear Regression
- K-Nearest Neighbors

#### Features
I break features down into 5 main categories: target, house, lot, location, and sale. I pull features directly from the [features.md file](./features.md) in order to ensure accuracy in the documentation. Refer to the file for more information of features used and their definitions.