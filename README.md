# Assignment 4

This repository contains solutions for Assignment 4. Each question is implemented in a separate Python file,
and all scripts run without errors.

---

## File Descriptions

### Question 1 — Dataset Exploration and Understanding
Loads the Breast Cancer dataset from scikit-learn and constructs the feature matrix `X`
and target vector `y`. Reports the shape of both and the number of samples belonging to each class.
Discusses whether the dataset is balanced or imbalanced and explains why class balance is a important for classification models.

---

### Question 2 — Decision Tree Model Using Entropy
Uses an 80/20 stratified train-test split on the breast cancer dataset. Trains a Decision Tree classifier
using entropy as the splitting criterion and reports the training and test accuracy. Explains what entropy
represents in the context of decision trees and whether the observed results suggest overfitting or good
generalization.

---

### Question 3 — Controlling Tree Complexity and Interpretability
Modifies the Decision Tree by introducing constraints (`max_depth=5` and `min_samples_split=10`) to reduce
overfitting. Reports training and test accuracy for the constrained model and displays the top five most
important features. Saves a visualization of the tree structure and a feature importance bar chart.
Discusses how controlling model complexity affects overfitting and how feature importance contributes to
the interpretability of decision trees.

---

### Question 4 — Neural Network for Binary Classification
Uses the same train-test split from Question 2. Standardizes the input features using `StandardScaler`
and trains a Multi-Layer Perceptron (MLP) with two hidden layers and a sigmoid output unit. Reports
training and test accuracy. Explains why feature scaling is necessary for neural networks and what an
epoch represents during training.

---

### Question 5 — Model Evaluation and Comparison
Rebuilds the constrained Decision Tree from Question 3 and the Neural Network from Question 4.
Computes and displays a confusion matrix for each model side by side. Compares the two models,
identifies which is preferred for this task, and discusses one advantage and one limitation of each model.

---

### Question 6 — Convolutional Neural Network with Fashion MNIST
Loads the Fashion MNIST dataset from TensorFlow/Keras and normalizes the pixel values to the range [0, 1].
Reshapes the images to include the channel dimension. Builds a CNN with two convolutional blocks
(Conv2D + MaxPooling2D), a Dropout layer, and a Dense softmax output layer. Trains the model for 15
epochs and reports test accuracy. Saves training accuracy and loss curves. Explains why CNNs are
preferred over fully connected networks for image data and what the convolution layers are learning.

---

### Question 7 — CNN Error Analysis and Misclassification Study
Loads the trained CNN from Question 6 and generates predictions on the Fashion MNIST test dataset.
Computes and displays the confusion matrix. Identifies the misclassified images and visualizes three examples,
clearly showing the true label and predicted label for each. Discusses one pattern observed in the misclassifications and one realistic method to improve CNN
performance.

---