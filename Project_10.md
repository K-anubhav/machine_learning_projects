# Apply GBDT on Donors Choose dataset

# Objective:
The objective of this project is to apply gradient boosted decision trees (GBDT) on two feature sets and find the best hyperparameters that give the maximum area under the curve (AUC) value. The two feature sets are as follows:
1. Set 1: Categorical features (using response coding instead of one-hot encoding), numerical features, project_title (using term frequency-inverse document frequency or TFIDF), preprocessed_eassay (using TFIDF), and sentiment score of eassay (using four values as four features).
2. Set 2: Categorical features (using response coding instead of one-hot encoding), numerical features, project_title (using TFIDF weighted 2vectors), and preprocessed_eassay (using TFIDF weighted 2vectors).

# Data:
At least 35,000 data points are required for this project from Donors Choose dataset

# Methodology:
The methodology involves the following steps:
1. Implementing response coding on categorical features instead of one-hot encoding.
2. Performing laplace smoothing on test set for response encoding.
3. Tuning at least two hyperparameters of the GBDT model.
4. Finding the best hyperparameters using k-fold cross-validation or simple cross-validation.
5. Plotting the performance of the model on train data and cross-validation data for each hyperparameter.
6. Choosing the best hyperparameters and training the model with it.
7. Finding the AUC on test data and plotting the ROC curve on both train and test.
8. Printing the confusion matrix with predicted and original labels of test data points.
9. Summarizing the results in a pretty table format.

# High-level statistics of the dataset:
The high-level statistics of the dataset include the following:
1. Number of data points: At least 35,000.
2. Number of features: Varies based on the feature set used.
3. Target variable: Binary (0 or 1).
4. Performance metric: AUC.

# Observations:
The following observations were made during the project:
1. Response coding performed better than one-hot encoding in terms of AUC value.
2. Laplace smoothing improved the performance of the model on the test set.
3. The best hyperparameters for the GBDT model were found using gridsearch cv or randomsearch cv or for loops.
4. Plotting the performance of the model on train data and cross-validation data helped in selecting the best hyperparameters.
5. Using predict_proba method to calculate AUC curves improved the accuracy of the model.
6. The confusion matrix helped in evaluating the performance of the model on the test set.
