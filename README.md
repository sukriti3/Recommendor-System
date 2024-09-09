Missing Link Prediction in Directed Graphs

This Python project focuses on predicting missing links in a directed graph by using matrix factorization and gradient descent. The project starts by reading data from a CSV file, which represents an impression network, and constructing a directed graph (DiGraph) using the NetworkX library. Each edge in the graph corresponds to an impression between two nodes (email addresses).

An adjacency matrix is then created from the graph, representing the relationships between nodes. To account for directed relationships, the matrix is adjusted: entries representing one-way connections are set to 1, while reciprocal connections are set to -1.

The core of the project is a function called missing_links, which performs matrix factorization on the adjacency matrix using two randomly initialized matrices, U and V. These matrices are iteratively updated through gradient descent to minimize the error between the predicted matrix (P) and the actual adjacency matrix. A threshold of 0.8 is used to classify potential links, and a count of new links is provided.

A root mean square error (RMSE) function is included to evaluate the accuracy of the predicted matrix. Finally, a new directed graph is generated from the predicted matrix, visualized using Matplotlib and NetworkX.

This project demonstrates the use of matrix factorization in network analysis to predict missing links and the application of machine learning techniques to enhance graph structure predictions.


