# Implementing TFIDF vectorizer

# Objective:

The objective of this project was to build a custom implementation of the Term Frequency-Inverse Document Frequency (TF-IDF) vectorizer and compare its results with Sklearn's implementation. The project aimed to show the importance of the TF-IDF vectorizer in natural language processing tasks and to demonstrate how to create a sparse matrix representation of a text corpus.

# Data:

The project did not use any specific dataset but rather focused on the implementation of the TF-IDF vectorizer. However, a sample text corpus could be used to test the implementation.

# Methodology:

The project implemented the TF-IDF vectorizer from scratch using Python. The implementation included both the fit and transform methods. The custom implementation was then compared with Sklearn's implementation of the TF-IDF vectorizer. To replicate the exact results of Sklearn's implementation, a few tweaks were made to the custom implementation, including sorting the vocabulary generated from idf in alphabetical order, using Sklearn's formula for idf, applying L2-normalization on the output matrix, and ensuring that the final output is a sparse matrix.

# High-level statistics of the dataset:

As the project did not use any specific dataset, there are no high-level statistics to report.

# Observations:

The custom implementation of the TF-IDF vectorizer produced the same vocabulary and idf values as Sklearn's implementation. The output of the custom implementation was a sparse matrix, which was then normalized using L2-normalization to match Sklearn's implementation. The final output of the custom implementation was compared with Sklearn's implementation, and it was observed that the two outputs were identical.

Overall, the project demonstrated the importance of the TF-IDF vectorizer in natural language processing tasks and provided an example of how to implement the TF-IDF vectorizer from scratch. The project also showed how to create a sparse matrix representation of a text corpus and how to normalize the matrix to obtain meaningful results.
