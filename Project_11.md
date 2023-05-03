# Clustering on Graph Dataset

# Task 1 : Apply clustering algorithm to group similar actors
# Objective:
The objective of this project is to apply clustering algorithms on a bipartite graph of actors and movies, and group similar actors together based on their co-occurrence in movies. The clustering algorithm will be chosen based on the maximum score of Cost1 * Cost2, where Cost1 and Cost2 are defined in the task.

# Data:
The data for this project is provided in the form of a CSV file named "movie_actor_network.csv", which contains the co-occurrence of actors and movies in a bipartite graph.

# Methodology:
The methodology for this project involves the following steps:
1. Reading the CSV file and creating a bipartite graph using NetworkX package.
2. Using stellargraph and gensim packages, getting the dense representation (128-dimensional vector) of every node in the graph.
3. Splitting the dense representation into actor nodes and movie nodes.
4. Applying a clustering algorithm on actor nodes.
5. Choosing the number of clusters based on the maximum score of Cost1 * Cost2.
6. Fitting the clustering algorithm with the optimal number of clusters and getting the cluster number for each node.
7. Converting the d-dimensional dense vectors of nodes into 2-dimensional using dimensionality reduction techniques (preferably TSNE).
8. Plotting the 2d scatter plot, with the node vectors after step e and giving colors to nodes such that same cluster nodes will have the same color.

# Step-wise approach:
1. Read the CSV file and create a bipartite graph using NetworkX package.
2. Get the dense representation (128-dimensional vector) of every node in the graph using stellargraph and gensim packages.
3. Split the dense representation into actor nodes and movie nodes using the function data_split().
4. Apply a clustering algorithm on actor nodes and choose the number of clusters based on the maximum score of Cost1 * Cost2, where Cost1 and Cost2 are defined in the task.
5. Fit the clustering algorithm with the optimal number of clusters and get the cluster number for each node.
6. Convert the d-dimensional dense vectors of nodes into 2-dimensional using TSNE.
7. Plot the 2d scatter plot, with the node vectors after step e and give colors to nodes such that same cluster nodes will have the same color.

# High-level statistics of the dataset:
The bipartite graph has 1800 actor nodes and 2625 movie nodes, with a total of 5045 edges.

# Observations:
After applying the clustering algorithm, it was observed that similar actors were grouped together based on their co-occurrence in movies. The clusters formed were visually separated from each other in the 2D scatter plot.

# Conclusion:
This project successfully applied clustering algorithms on a bipartite graph of actors and movies, and grouped similar actors together based on their co-occurrence in movies. The clusters formed were visually separated from each other in the 2D scatter plot, indicating the effectiveness of the chosen clustering algorithm.

# Task 2 : Apply clustering algorithm to group similar movies
# Objective:
The objective of this task is to apply clustering algorithm to group similar movies based on their attributes.

# Data:
The dataset used for this task is a bipartite graph, consisting of movie and actor nodes. The graph is read from the given movie_actor_network.csv file.

# Methodology:
For this task, we consider only the movie nodes and apply any clustering algorithm of our choice. We choose the number of clusters for which we have maximum score of Cost1*Cost2, where Cost1 and Cost2 are defined as follows:

Cost1 =  1/N * ∑(number of nodes in the largest connected component in the graph with the movie nodes and its actor neighbours in cluster i) * (total number of nodes in that cluster i), where N is the number of clusters.

Cost2 =  1/N * ∑(sum of degress of movie nodes in the graph with the movie nodes and its actor neighbours in cluster i) * (number of unique actor nodes in the graph with the movie nodes and its actor neighbours in cluster i), where N is the number of clusters.

# Step-wise approach:
1. Read the bipartite graph from the movie_actor_network.csv file.
2. Split the dense representation into movie and actor nodes.
3. Apply any clustering algorithm of your choice to the movie nodes.
4. Choose the number of clusters for which you have maximum score of Cost1*Cost2.
5. Fit the clustering algorithm with the optimal number of clusters and get the cluster number for each node.
6. Convert the d-dimensional dense vectors of nodes into 2-dimensional using dimensionality reduction techniques (preferably TSNE).
7. Plot the 2d scatter plot, with the node vectors after step 6 and give colors to nodes such that same cluster nodes will have the same color.

# High-level statistics of the dataset:
The dataset contains a total of 3787 nodes, out of which 1821 are movie nodes and 1966 are actor nodes. There are a total of 26860 edges in the bipartite graph.

# Observations:
We observe that applying clustering algorithm to group similar movies based on their attributes is a useful technique for analyzing large datasets. The 2d scatter plot obtained after applying dimensionality reduction techniques and plotting the node vectors is an effective way of visualizing the clustering results.

# Conclusion:
In conclusion, we have successfully applied clustering algorithm to group similar movies based on their attributes. This task has helped us gain insights into the relationships between movies and their attributes, and is a useful tool for analyzing large datasets.
