# Clustering Analysis on the Iris Dataset
The Iris dataset consists of 150 samples from three species of Iris flowers, characterized by four features: sepal length, sepal width, petal length, and petal width. Our goal is to group the samples into clusters based on these features, and to visualize and evaluate the results.This repository provides a comprehensive analysis of clustering algorithms applied to the famous Iris dataset. We explore and compare three clustering techniques:

*K-Means Clustering
*Mean Shift Clustering
*Hierarchical Clustering (HClust)

# K-Means Clustering
Approach: We apply the K-Means algorithm with k=3 clusters, corresponding to the three known species in the Iris dataset.
Results: The K-Means algorithm groups the data into three clusters, which correspond reasonably well to the actual species labels.
Evaluation: Sum of squared distances to clusters is calculated to evaluate the performance
Graphs:
Distance 
![distance](https://github.com/user-attachments/assets/33095ef6-3598-43ed-93fd-de78a0b8d891)
Elbow
![elbow](https://github.com/user-attachments/assets/8fbc50ad-da55-4fcc-b3ce-e4df02c4bbc6)
Cluster
![newplot (1)](https://github.com/user-attachments/assets/d48883ce-99fe-4def-acb0-717d61dc4eba)
TSNE
![newplot](https://github.com/user-attachments/assets/ae251d3b-073b-48f9-84e0-e81d3ca28e8c)
Silhoutte
![silhoutte](https://github.com/user-attachments/assets/b1204786-311b-4890-bf20-4dff4eaf7645)

Table:
Values have been extracted using various processing techniques like , no data processing, nomralization, transformation, PCA, normalization and transformation , and normalization,transformation and PCA.
![kmeans](https://github.com/user-attachments/assets/dab06892-8de2-4896-b737-37281f7d93c1)

Conclusion:
K-Means successfully identified clusters that correspond to the species in the Iris dataset. While the clusters are not perfect, they provide a meaningful grouping of the data.
The CLuster plot clearly shows the separation between clusters, providing a visual understanding of how K-Means has segmented the data.

# Mean Shift Clustering
Approach: The Mean Shift algorithm is a non-parametric clustering method that does not require a predefined number of clusters. It works by shifting the centroids iteratively to converge toward high-density regions in the feature space

Evaluation: The number of clusters is determined automatically by the algorithm based on the data distribution.

Table:
Values have been extracted using various processing techniques like , no data processing, nomralization, transformation, PCA, normalization and transformation , and normalization,transformation and PCA.
![meanshift](https://github.com/user-attachments/assets/c49c425a-e9a3-41ad-9b0f-2a487e4fcd91)

# Hierarchical Clustering 

Approach: Hierarchical clustering builds a tree-like structure of nested clusters (a dendrogram). We use Agglomerative Clustering with different linkage methods (single, complete, average).

Evaluation: The silhouette score is used to assess the quality of clusters based on the cohesion and separation of samples.

Table:
Values have been extracted using various processing techniques like , no data processing, nomralization, transformation, PCA, normalization and transformation , and normalization,transformation and PCA.
![hclust](https://github.com/user-attachments/assets/fb19c959-6312-4307-9c74-e4a435a22d3b)

# Conclusion
*K-Means effectively clustered the Iris data into three distinct groups, with results closely aligning with the true species labels.
*Mean Shift offered a more flexible clustering approach and found a different number of clusters based on the data density, which could be useful for non-standard datasets.

*Hierarchical Clustering provided insight into the nested relationships between clusters

*Each algorithm has its strengths and weaknesses, with K-Means being quick and intuitive, Mean Shift providing flexibility, and Hierarchical Clustering giving a deeper understanding of cluster structure.
