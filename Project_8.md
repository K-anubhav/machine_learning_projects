# Apply Decision Trees on Donors Choose dataset

# Objective:
The objective of this project is to analyze a Donors Choose dataset of project proposals and predict whether a project will be approved or not based on its features.

# Data:
The dataset used in this project contains information about project proposals submitted to DonorsChoose, a US-based non-profit organization that connects public school teachers with donors who want to support classroom projects. The dataset includes both numerical and categorical features, such as project title, project description, teacher name, school state, grade level, project subject category, and others.

# Methodology:
The project uses a Decision Tree Classifier to predict whether a project will be approved or not based on its features. Two feature sets were used for the classifier:
- Set 1: categorical, numerical features + preprocessed_essay (TFIDF) + Sentiment scores (preprocessed_essay)
- Set 2: categorical, numerical features + preprocessed_essay (TFIDF W2V) + Sentiment scores (preprocessed_essay)

The hyperparameters for the Decision Tree Classifier were tuned using GridSearchCV to find the best `depth` in range [1, 3, 10, 30], and the best `min_samples_split` in range [5, 10, 100, 500], which will give the maximum AUC value. The performance of the model was evaluated using k-fold cross validation and plotted using a 3D scatter plot or a heatmap.

The features with non-zero feature importance were selected and used to train a model of choice, which could be either Decision Tree, Logistic Regression or Linear SVM. The hyperparameters of the model were tuned and its performance was evaluated and summarized.

High-level statistics of the dataset:
- Number of data points: 109248
- Number of features: 51
- Number of data points with missing values: 190

# Observations:
- Set 2 features performed better than Set 1 features, achieving a higher AUC score.
- The best hyperparameters for the Decision Tree Classifier were a `depth` of 30 and a `min_samples_split` of 500, achieving an AUC score of 0.68 on the test set.
- The features with non-zero feature importance were `teacher_prefix`, `project_grade_category`, `project_subject_categories`, `project_subject_subcategories`, `school_state`, `clean_categories`, `clean_subcategories`, `price`, `quantity`, `sentiment_scores`, and `sentiment_polarity`.
- The performance of the model with the selected features varied depending on the choice of the model and the hyperparameters, with Logistic Regression achieving the best AUC score of 0.71 on the test set.
