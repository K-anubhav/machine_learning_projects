# Objective: 
The objective of this project is to apply Naive Bayes on Donors Choose dataset. The dataset contains information about various funding proposals from teachers and their status whether they were accepted or rejected. The aim is to build a model that can predict whether a funding proposal will be accepted or not based on various features like teacher_prefix, project_grade_category, school_state, clean_categories, clean_subcategories, price, teacher_number_of_previously_posted_projects, and essay.

# Data: 
The dataset used for this project is the Donors Choose dataset, which contains information about funding proposals from teachers. The dataset is available on Kaggle and can be downloaded from this link: https://www.kaggle.com/c/donorschoose-application-screening/data

# Methodology: 
The methodology used in this project involves applying Multinomial Naive Bayes on the Donors Choose dataset. The dataset is preprocessed and various features are considered for the model building. The hyperparameters are tuned using k-fold cross-validation and the best hyperparameters are used for training the model. The model is evaluated on the test dataset using the area under the curve (AUC) metric and the ROC curve is plotted to visualize the performance of the model.

# High-level statistics of the dataset:
The Donors Choose dataset contains 1,08,183 rows and 16 columns. The dataset is imbalanced with 85.7% of the proposals being accepted and 14.3% being rejected.

# Observations:
The model performed well on the test dataset with an AUC score of 0.705. The top 20 features that contributed to the model's prediction were also identified and are presented in the summary table at the end of the notebook.

# Task: 
The task involves applying Multinomial Naive Bayes on the Donors Choose dataset to predict whether a funding proposal will be accepted or rejected.

# Steps:
1. Minimum data points need to be considered for people having 4GB RAM is 50k and for 8GB RAM is 100k.
2. Features that need to be considered are essay, categorical features (teacher_prefix, project_grade_category, school_state, clean_categories, clean_subcategories) and numerical features (price, teacher_number_of_previously_posted_projects).
3. Two feature sets are considered: 
   Set 1: categorical, numerical features + preprocessed essay (BOW)
   Set 2: categorical, numerical features + preprocessed essay (TFIDF)
4. Multinomial Naive Bayes is applied on both feature sets and the best hyperparameters are tuned using k-fold cross-validation.
5. The model is evaluated on the test dataset using the AUC metric and the ROC curve is plotted.
6. The top 20 features contributing to the model's prediction are identified using the `feature_log_prob_` parameter of `MultinomialNB`. 
7. The results are summarized in a table format at the end of the notebook.
