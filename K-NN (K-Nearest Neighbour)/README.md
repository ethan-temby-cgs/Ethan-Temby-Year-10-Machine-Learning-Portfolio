# K-NN (K-Nearest Neighbour) 🙋‍♂️

## Code Explanation:

The provided code is an implementation of the k-nearest neighbors (k-NN) algorithm using the Wine dataset. This algorithm is a classification method used for assigning an input data point to a specific class based on the majority class of its k nearest neighbors in the feature space.

1. **Importing Libraries:**
   - `numpy`, `pandas`: These libraries are used for numerical operations and data manipulation, respectively.
   - `sklearn.datasets`: This module provides datasets for practicing machine learning.
   - `sklearn.model_selection`: It includes functions for splitting datasets into training and testing sets.
   - `sklearn.preprocessing`: This module provides tools for scaling and preprocessing data.
   - `sklearn.neighbors`: It contains the k-NN classifier.
   - `sklearn.metrics`: This module provides metrics for evaluating model performance.
   - `matplotlib.pyplot`: This library is used for data visualization.

2. **Loading and Preparing the Dataset:**
   - The `load_wine()` function from `sklearn.datasets` is used to load the Wine dataset, which contains 13 attributes related to wine characteristics and a target variable.
   - The loaded data is converted into a pandas DataFrame, making it easier to manipulate.

3. **Splitting the Dataset:**
   - The features (`X`) are extracted from the DataFrame, excluding the target variable.
   - The target variable (`y`) is extracted separately.
   - The `train_test_split()` function is used to split the dataset into training and testing sets. Here, 70% of the data is used for training and 30% for testing.

4. **Standardizing Features:**
   - The `StandardScaler()` is applied to standardize the feature data. Standardization transforms features to have zero mean and unit variance, which helps in improving model convergence and performance.

5. **Initializing and Training the k-NN Classifier:**
   - The value of `k` (number of neighbors) is set to 7.
   - An instance of the `KNeighborsClassifier` is created with the chosen `k` value.
   - The `fit()` method is used to train the k-NN classifier on the standardized training data.

6. **Making Predictions and Evaluation:**
   - The `predict()` method is used to predict the class labels of the test set based on the trained k-NN classifier.
   - The performance of the model is evaluated using a confusion matrix and a classification report. The confusion matrix provides a count of true positive, true negative, false positive, and false negative predictions. The classification report includes metrics such as precision, recall, and F1-score for each class.

7. **Visualizing Decision Boundaries:**
   - A scatter plot is created using `matplotlib` to visualize the decision boundaries of the trained k-NN classifier.
   - The x-axis represents the "Alcohol" feature, and the y-axis represents the "Malic Acid" feature.
   - The colors of the data points are based on their true class labels.

## Dataset: Wine Dataset:
The Wine dataset is a classic dataset often used for practicing classification algorithms. It contains the chemical analysis results of wines from three different cultivars. The dataset consists of 13 attributes, such as alcohol content, malic acid concentration, and color intensity, which are used to classify the wines into one of three classes.

## Technique: k-Nearest Neighbors (k-NN) Algorithm:
The k-NN algorithm is a simple, instance-based machine learning algorithm used for classification and regression tasks. It assigns a label to an unseen data point based on the majority class of its k nearest neighbors in the feature space. The choice of `k` affects the algorithm's sensitivity to noise and its ability to capture underlying patterns. The k-NN algorithm is non-parametric, meaning it doesn't assume a specific functional form for the underlying data distribution.

In this code, k-NN is used as a classifier. It involves training on the training dataset, making predictions on the testing dataset, and evaluating its performance. The decision boundaries of the k-NN classifier are visualized, showing how the algorithm separates different classes in the feature space.

Remember that k-NN can be sensitive to the choice of `k` and the scaling of features. It's essential to experiment with different values of `k` and preprocessing techniques to optimize its performance for different datasets.


### License 🪪:

The code and documentation in this repository are licensed under the MIT License.
