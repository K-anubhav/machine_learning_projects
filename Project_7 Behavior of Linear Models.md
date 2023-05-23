# Objective:
This project includes various tasks related to understanding and analyzing linear models. The main objectives of the project are:

- To observe how linear models work in case of data imbalance
- To understand the behavior of linear models when the features have different variances
- To analyze how outliers affect linear regression models
- To understand the effect of regularization on linear models
- To compare the performance of various linear models on a given dataset

# Data:
The project uses various synthetic datasets with different levels of class imbalance, feature variance, and outlier effects.

# Methodology:
The project involves multiple tasks, each focusing on a specific aspect of linear models. The tasks are described below:

- Task A: 
Behavior of Linear Models in Imbalanced Data
In this task, we observe how linear models behave when the data has a class imbalance. We created four random datasets that are linearly separable and have different levels of class imbalance. We use Support Vector Machines (SVMs) and Logistic Regression to classify the data and plot the hyperplane for different learning rates and regularization parameters. We also represent the support vectors in different colors to understand the position of the hyperplane. 

- Task B: 
Effect of Feature Variance on Linear Models
In this task, we observe how linear models work when the features have different variances. We apply Logistic Regression and SVM on a dataset with three features that have different variances. We also standardize the dataset and compare the results to see the impact of feature scaling. 

- Task C: 
Outlier Effect on Linear Regression
In this task, we analyze how outliers affect the performance of linear regression models. We use Stochastic Gradient Descent (SGD) to train linear regression models on a synthetic dataset with outliers. We train the models with different regularization parameters and add outliers one at a time to see how they affect the prediction hyperplane. We plot the results for different regularizers in a 3x5 grid of subplots.

- Task D: 
Comparison of Linear Models
In this task, we compare the performance of different linear models on a given dataset. We use Linear Regression, Ridge Regression, Lasso Regression, Elastic Net Regression, and SVM to train models on a synthetic dataset and compare their performance based on various metrics.

- Task E: 
To implement the decision_function() method of a kernel Support Vector Machine (SVM) with a radial basis function (RBF) kernel. The decision_function() method is used to predict the class of a new data point by calculating its distance from the decision boundary. The output value of the decision_function() method determines whether the new data point belongs to the positive or negative class. By implementing this method, you will be able to classify new data points using the trained SVM model.

- Task F: 
To apply the stochastic gradient descent (SGD) algorithm to find the weight vector W and the intercept b, using the training data (fcv, ycv). The data here is one-dimensional, so the weight vector W will also be one-dimensional, with a shape of (1,).
To apply SGD, we need to first modify the labels of the training data ycv. Based on the given image, we need to calculate the values of y+ and y- for each data point in the training data, and replace the corresponding labels in ycv with these values.
After modifying the labels, we can use SGD to optimize the weight vector W and the intercept b. The objective is to minimize the loss function, which measures the difference between the predicted and actual labels. The SGD algorithm updates the weight and intercept values iteratively by computing the gradient of the loss function with respect to these values and adjusting them in the direction of the negative gradient.

Once the optimization process is complete, we will have the final values of the weight vector W and the intercept b, which can be used to predict the labels of new data points using the linear model: y = W * x + b.

# Observations:
The project's main observations are:

- Linear models can perform poorly in imbalanced datasets, and the hyperplane position can be biased towards the majority class.
- Feature scaling can significantly affect the performance of linear models when features have different variances.
- Outliers can have a significant impact on the performance of linear regression models, and regularization can help mitigate their effect.
- Different linear models can perform differently on a given dataset, and their performance depends on various factors such as the dataset size, feature complexity, and regularization parameters.
