# Objective:
The objective of this project is to implement Logistic Regression with L2 regularization using Stochastic Gradient Descent (SGD) without using any external libraries like scikit-learn.

# Data:
No specific dataset is used in this project as the focus is on the implementation of the logistic regression model.

# Methodology:
The model is implemented in a step-by-step manner using different functions. The first step is to initialize the weight vector and intercept term to zeros. Next, a loss function is defined, which calculates the log loss of the predicted labels with respect to the true labels.

After the initialization of weights and the definition of the loss function, we perform training by iterating through each epoch and each batch of data points. For each batch, we calculate the gradient of the loss function with respect to each weight in the weight vector and the gradient of the intercept term. Using these gradients, we update the weights and the intercept term.

We then calculate the log loss for the train and test sets with the updated weights and intercept term. This process is repeated until the loss is not updating, and the loss values are appended to a list for further analysis.

# High-level statistics of the dataset:
As no specific dataset is used in this project, there are no high-level statistics to report.

# Observations:
As the focus of this project is on the implementation of the logistic regression model, there are no specific observations to report. However, it is important to note that the performance of the model heavily depends on the tuning of hyperparameters such as the learning rate, regularization parameter, and batch size. Proper tuning of these parameters is crucial for achieving optimal performance.
