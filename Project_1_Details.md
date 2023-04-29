# Exploratory Data Analysis on Haberman Cancer Survival Dataset


## Objective:

The objective of this project is to perform exploratory data analysis on the Haberman Cancer Survival dataset to gain insights and identify important features for the classification task.

## Data:
The Haberman Cancer Survival dataset contains data on the survival of patients who had undergone surgery for breast cancer at the University of Chicago's Billings Hospital between 1958 and 1970. The dataset includes 306 instances and 4 features, including the age of the patient, year of operation, number of positive axillary nodes, and the survival status (1 = the patient survived for 5 years or longer; 2 = the patient died within 5 years).
Download Haberman Cancer Survival dataset from Kaggle. You may have to create a Kaggle account to donwload data. (https://www.kaggle.com/gilsousa/habermans-survival-data-set)

## Methodology:
The exploratory data analysis is performed in a Jupyter notebook using Python. The following analyses are conducted:

## High-level statistics of the dataset:
The number of points, number of features, number of classes, and data-points per class are computed and analyzed.
Univariate analysis: Probability density function (PDF), cumulative distribution function (CDF), boxplot, and violin plots are plotted for each feature to understand their distribution and identify outliers.
Bivariate analysis: Scatter plots and pair plots are plotted for each pair of features to identify correlations and separability between the classes.
Final conclusions: The key features that are important for the classification task are summarized and quantified. The exploratory analysis is summarized in 3-5 key observations.

## Observations:
The exploratory data analysis reveals that the number of positive axillary nodes is the most important feature for the classification task. Patients with fewer positive nodes have a higher chance of survival, whereas patients with a higher number of positive nodes have a lower chance of survival. Age and year of operation do not seem to have a significant impact on the survival rate. The dataset is imbalanced, with a higher number of instances belonging to the 1 (survived) class. Overall, the exploratory analysis provides valuable insights for further modeling and analysis.
