# K-Means Testing (Clustering)- _A Method of Unsupervised Learning_ 🖇️

#### Completed Portfolio Task Available In Above Jupyter Notebook

## Code Explanation:

The provided code demonstrates the use of the K-means clustering algorithm on the Iris dataset, a classic dataset in machine learning. The goal is to cluster iris flowers based on their sepal dimensions using the K-means algorithm.

1. **Import Libraries:** The necessary libraries are imported. `numpy` is used for numerical operations, `sklearn.datasets` to load the Iris dataset, `sklearn.preprocessing` to standardize the features, and `matplotlib.pyplot` for data visualization.

2. **Load the Iris Dataset:** The Iris dataset is loaded using `load_iris()`. The dataset contains sepal and petal dimensions of iris flowers, and the species they belong to.

3. **Extract Features and Species Names:** The `iris.data` contains the feature data, while `iris.target_names` stores the species names.

4. **Custom KMeans Class:** A custom class `KMeans` is defined to implement the K-means clustering algorithm. It has `n_clusters` as the number of clusters, `max_iter` as the maximum number of iterations, and `tol` as the tolerance for convergence.

5. **`fit` Method:** The `fit` method initializes centroids by randomly selecting data points. It iterates `max_iter` times, calculating distances from each data point to centroids, assigning data points to the nearest centroid, updating centroids, and checking for convergence.

6. **`predict` Method:** The `predict` method calculates distances and assigns data points to the nearest centroid using the trained centroids.

7. **Standardize Features:** The `StandardScaler` is applied to standardize the features for effective clustering. Standardization ensures that all features are on the same scale.

8. **Instantiate KMeans and Fit Data:** An instance of the `KMeans` class is created with `n_clusters` set to 3. The K-means algorithm is then fitted on the standardized features.

9. **Predict Cluster Labels:** The algorithm's predicted cluster labels are obtained using the `predict` method.

10. **Data Visualization:** The clustered data is visualized using a scatter plot. Each point is colored based on its predicted cluster, and the centroids are marked in red with 'X' markers.

### Iris Dataset Explanation:

The Iris dataset contains samples of iris flowers, each characterized by four features: sepal length, sepal width, petal length, and petal width. The dataset is commonly used for classification and clustering tasks. It consists of 150 samples, with 50 samples for each of the three species: Setosa, Versicolor, and Virginica.

### Unsupervised Learning and K-means Clustering:

Unsupervised learning is a type of machine learning where the algorithm is trained on input data without any labeled output. The goal is to explore the inherent patterns or structures in the data. K-means clustering is a popular unsupervised learning technique that aims to partition a dataset into K distinct, non-overlapping clusters.

K-means algorithm steps:

1. **Initialization:** Randomly initialize K centroids.

2. **Assignment:** Assign each data point to the nearest centroid, forming clusters.

3. **Update Centroids:** Recalculate the centroids by taking the mean of the data points in each cluster.

4. **Iteration:** Repeat steps 2 and 3 until convergence or a maximum number of iterations is reached.

K-means aims to minimize the within-cluster sum of squared distances, effectively grouping similar data points together. The algorithm can help discover underlying structures, categorize data, or find natural groupings in the absence of labeled data.

In the provided code, K-means is applied to cluster iris flowers based on their sepal dimensions. The standardized sepal length and width are used for clustering, and the algorithm assigns flowers to clusters based on similarity in these features.

Overall, the code exemplifies how K-means clustering can be applied to real-world data like the Iris dataset for pattern discovery and insight generation in unsupervised learning scenarios.

### Libraries Used:

- numpy
- sklearn.datasets
- sklearn.preprocessing
- matplotlib.pyplot

### License 🪪:

The code and documentation in this repository are licensed under the MIT License.
