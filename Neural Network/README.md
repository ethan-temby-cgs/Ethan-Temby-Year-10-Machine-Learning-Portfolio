# Neural Network Model (Utilising the Breast Cancer Wisconsin Dataset) 🪐


## Discussion of Core Themes: 

In this example, we used the provided libraries to build, train, and evaluate a more complex neural network model for binary classification. The process involved:

- Importing the necessary libraries. Loading the Breast Cancer Wisconsin dataset and preprocessing it. Splitting the data into training and testing sets and shuffling the training data. Building a neural network classifier using the MLPClassifier class from sklearn. Training the model on the training data. Evaluating the model's performance using accuracy and creating a confusion matrix. Visualizing the confusion matrix heatmap using Matplotlib. Saving the trained model to a file using pickle and loading it back. This example demonstrates a more complex classification task using a neural network model. While neural networks can handle more complex tasks, the general workflow remains consistent: loading data, preprocessing, building a model, training, evaluating, and visualizing results.

## Deep Explanation of Neural Networks:

Neural networks are a fundamental concept in the field of machine learning and artificial intelligence. They are inspired by the structure and functioning of the human brain's interconnected neurons. Neural networks consist of layers of interconnected nodes (neurons) that process and transform input data to produce output predictions. Here's a breakdown of key neural network concepts:

1. **Architecture:**
   A neural network is organized into layers: an input layer, one or more hidden layers, and an output layer. Each layer comprises nodes that are connected to nodes in adjacent layers. Data flows through the network from the input layer, undergoing transformations in the hidden layers, and ultimately producing predictions in the output layer.

2. **Activation Functions:**
   Activation functions introduce non-linearity to the neural network, enabling it to learn complex patterns and relationships in data. Common activation functions include:
   - **ReLU (Rectified Linear Activation):** f(x) = max(0, x), which replaces negative values with zero while leaving positive values unchanged.
   - **Sigmoid:** f(x) = 1 / (1 + exp(-x)), mapping input values to a range of 0 to 1.
   - **Tanh (Hyperbolic Tangent):** f(x) = (exp(x) - exp(-x)) / (exp(x) + exp(-x)), mapping input values to a range of -1 to 1.

3. **Backpropagation:**
   Backpropagation is a key mechanism for training neural networks. It involves iteratively adjusting the weights and biases of the network's connections based on the difference between predicted outputs and actual targets. The process includes:
   - **Forward Pass:** Input data is propagated through the network to produce predictions.
   - **Loss Calculation:** A loss function (e.g., mean squared error for regression or binary cross-entropy for classification) quantifies the discrepancy between predictions and targets.
   - **Backward Pass:** The network computes gradients of the loss with respect to its parameters (weights and biases) using the chain rule of calculus.
   - **Gradient Descent:** The weights and biases are updated in the opposite direction of their gradients, scaled by a learning rate. This process minimizes the loss and improves prediction accuracy.

## Usefulness of the Dataset (Breast Cancer Classification):

The `load_breast_cancer` dataset from `sklearn.datasets` is highly relevant for demonstrating the capabilities of neural networks. It contains features derived from images of breast cancer biopsies, aiming to classify tumors as malignant (cancerous) or benign (non-cancerous). Here's why this dataset is useful in conjunction with neural networks:

1. **Binary Classification Challenge:**
   Neural networks excel in binary classification tasks like this, where the goal is to categorize inputs into one of two classes. The dataset's binary nature aligns well with the final layer's activation function (sigmoid) that outputs probabilities.

2. **Complex Patterns:**
   The dataset contains various features (such as texture, size, and shape) that might not have linear relationships. Neural networks, with their ability to capture complex non-linear patterns using hidden layers and activation functions, are well-suited for such tasks.

3. **High-Dimensional Data:**
   With 30 features in the dataset, it represents a relatively high-dimensional problem. Neural networks can handle such data effectively by learning hierarchical representations through their layers.

4. **Data Preprocessing:**
   The dataset requires preprocessing steps like feature scaling (standardization). This preprocessing is crucial for neural networks to converge faster during training and to ensure balanced learning across features.

5. **Generalization:**
   Neural networks can learn from large datasets and generalize well to new, unseen data. The `load_breast_cancer` dataset's relatively modest size allows for quick experimentation and exploration of neural network architectures.

By using the breast cancer dataset with neural networks, we can showcase the power of these models in solving real-world problems. The deep architecture, activation functions, and backpropagation principles enable the network to learn intricate relationships between the features and predict tumor malignancy accurately. This combination of a relevant dataset and a neural network demonstrates the potential of machine learning to contribute to medical diagnostics and decision-making.

### Libraries Used:

- [Numpy](https://www.youtube.com/watch?v=lLRBYKwP8GQ&t=1073s)
- [Pandas](https://www.youtube.com/watch?v=zN2Hua6oII0&t=8s)
- [matplotlib](https://www.youtube.com/watch?v=nzKy9GY12yo)
- [scikit-learn intro](https://www.youtube.com/watch?v=rvVkVsG49uU)
- [scikit-learn tut](https://www.youtube.com/watch?v=M9Itm95JzL0)
- [pickle](https://www.youtube.com/watch?v=6Q56r_fVqgw)

### 🪪 License

The code and documentation in this repository are licensed under the MIT License.
