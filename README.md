# Face Recognition using Eigenface Approach

## Problem Statement

Implementing a face recognition system based on the Eigenface approach. The Eigenfaces algorithm, rooted in Principal Component Analysis (PCA), is a popular method for facial recognition introduced by Sirovich and Kirby in 1987 and later formalized by Turk and Pentland in 1991.

### Objective

The primary goal of this project is to develop a face recognition system capable of identifying individuals in a dataset of facial images using the Eigenface algorithm. Eigenfaces represent the principal components of the face images, enabling efficient face recognition based on the linear combination of these components.

## Implementation

The implementation is done using Python, with the help of popular libraries such as NumPy, scikit-learn, OpenCV, and Matplotlib.

### Dataset

The Olivetti Faces dataset is used for training and testing the face recognition system. The dataset consists of 400 facial images of 40 subjects, each with 10 different images under varying conditions.

### Steps

1. **Loading the Data:** The Olivetti Faces dataset is loaded, containing 400 facial images and corresponding target labels.

2. **Data Preprocessing:** The images are reshaped into vectors, and the dataset is split into training and testing sets.

3. **Principal Component Analysis (PCA):** PCA is applied to extract the principal components (eigenfaces) from the training data. The number of components is chosen based on the explained variance or a predetermined threshold.

4. **Visualizing Eigenfaces:** The eigenfaces are visualized to understand the features captured by each principal component.

5. **Training Classifiers:** Various classifiers, including Support Vector Machines (SVM), Logistic Regression, Naive Bayes, K-Nearest Neighbors (KNN), and Decision Trees, are trained on the transformed data using PCA.

6. **Model Evaluation:** The performance of each classifier is evaluated using accuracy, confusion matrix, and classification report. Cross-validation scores are also calculated.

7. **Adding Noise:** To assess robustness, noise is added to images, and the effect on recognition accuracy is observed.
