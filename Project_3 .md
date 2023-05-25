# Objective:
The objective of this project is to implement RandomSearchCV with k-fold cross-validation on KNN (K-Nearest Neighbors) algorithm using custom code. The aim is to find the best hyperparameters for KNN and create a decision boundary plot to visualize the performance of the model.

# Data:
The data is generated using the make_classification function from sklearn.datasets. The dataset consists of 10,000 samples with two features and two informative features. There are no redundant features and one cluster per class. The data is split into training and testing sets using the train_test_split function from sklearn.model_selection.

# Methodology:
The methodology involves implementing a custom RandomSearchCV function that takes in the training data, classifier (KNN), range of hyperparameters, and number of folds as input. The function generates 10 unique hyperparameters within the given range and divides the training data into k folds. For each hyperparameter, the function performs k-fold cross-validation by training the KNN model on k-1 folds and testing on the remaining fold. The mean train and test accuracies are computed and stored in lists. The function returns the train and test accuracy scores for each hyperparameter.

# High-level statistics of the dataset:
The dataset consists of 10,000 samples with two features and two informative features. There are no redundant features and one cluster per class.

# Observations:
The best hyperparameter is chosen based on the hyperparameter vs accuracy plot. The decision boundary plot for the model initialized with the best hyperparameter is created to visualize the performance of the model.
