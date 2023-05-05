# Application of Bootstrap samples in Random Forest

# Objective:
The objective of this project is to demonstrate the application of the Bootstrap Aggregating (Bagging) technique in building high variance models for predicting house prices using regression trees. Additionally, the project aims to compute the Train Mean Squared Error (MSE) value and the Out-of-Bag (OOB) score for each model, compute the confidence intervals of the Train MSE and OOB score, and finally use the trained models to predict the price of a single query point.

# Data:
The dataset used in this project is the Boston Housing dataset, which contains 506 observations and 13 attributes describing aspects of houses in the Boston area.

# Methodology:
The project uses the Bagging technique to build 30 high variance models by randomly selecting 60% of the data points and replicating a subset of those points to create each sample. Each sample has a different set of columns to ensure that each sample has at least 3 features/columns/attributes. For each model, a regression tree is built on the sample data, and the predicted values of each data point in the dataset are computed. Using the predicted values of each model, the Train MSE value is computed. Additionally, the OOB score is calculated by predicting the house price of each data point using the models built on the samples that do not include that data point.

## Step-wise approach:
### Task 1:
Step 1: Create 30 samples by randomly selecting 303 data points and replicating a subset of those points from the sample. Make sure each sample has different columns and each sample has at least 3 features/columns/attributes.
Step 2: Build a regression tree on each of the 30 samples and compute the predicted values of each data point in the dataset using each model. Compute the Train MSE value using the predicted values.
Step 3: Compute the OOB score by predicting the house price of each data point using the models built on the samples that do not include that data point.

### Task 2:
Repeat Task 1 for 35 times and store the Train MSE and OOB score for each iteration. Using the 35 values as a sample, find the confidence intervals of the Train MSE and OOB score using the Central Limit Theorem.

### Task 3:
Predict the house price of a single query point using the trained models. 
The query point is xq=[0.18,20.0,5.00,0.0,0.421,5.60,72.2,7.95,7.0,30.0,19.1,372.13,18.60]. Follow the steps in Task 1, Step 2 to predict the price of the query point.

# High-level statistics of the dataset:
The Boston Housing dataset contains 506 observations and 13 attributes. 
The minimum and maximum values for the target variable, i.e., house price, are $5,000 and $50,000, respectively, with a mean value of $22,532.80 and a standard deviation of $9,188.01. 
The attributes in the dataset include per capita crime rate by town, the proportion of residential land zoned for lots over 25,000 sq.ft, the proportion of non-retail business acres per town, the Charles River dummy variable (1 if tract bounds river; 0 otherwise), nitric oxides concentration (parts per 10 million), 
average number of rooms per dwelling, proportion of owner-occupied units built before 1940, weighted distances to five Boston employment centres, index of accessibility to radial highways, 
full-value property-tax rate per $10,000, pupil-teacher ratio by town, 1000(Bk - 0.63)^2 where Bk is the proportion of Black people by town.
