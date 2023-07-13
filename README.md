# EHR-Pancreatic Data Classification Project

This project focuses on developing classification algorithms for predicting the sensitization type in EHR-Pancreatic data, with two distinct categories: Widespread and Segmental. The dataset exhibits an imbalanced distribution of classes, making the classification task challenging. In order to address this issue and improve the model's performance, we explore different techniques and evaluate the results using various performance metrics.

# Dataset Description
The EHR-Pancreatic dataset contains multiple features and a corresponding target variable, Sensitization type. The goal is to predict whether a given sample belongs to the Widespread or Segmental class. The dataset suffers from class imbalance, which means that one class has significantly more samples than the other, potentially leading to biased model predictions.

# Classification Algorithms
This project employs three different classification algorithms:

Three-layer Neural Network: A simple neural network architecture consisting of three layers: an input layer, a hidden layer, and an output layer. The neural network aims to learn the underlying patterns and relationships in the data to classify the sensitization type accurately.

Two-layer Convolutional Neural Network (CNN): CNNs are effective in capturing spatial dependencies in data, making them suitable for analyzing images or sequential data. In this project, we employ a two-layer CNN architecture to extract relevant features and classify the sensitization type.

Two-layer Long Short-Term Memory (LSTM): LSTMs are well-suited for analyzing sequential data due to their ability to retain and learn long-term dependencies. We utilize a two-layer LSTM architecture to model temporal relationships in the EHR-Pancreatic data and predict the sensitization type.

# Techniques Applied
To improve the performance and robustness of the classification algorithms, we apply the following techniques:

K-fold Cross-Validation: We partition the dataset into k subsets (folds) and perform k iterations. In each iteration, we use k-1 folds for training and the remaining fold for testing. This technique helps evaluate the model's performance on different subsets of the data and mitigates the impact of random variations in the training and testing splits.

Leave-One-Subject-Out Cross-Validation: In this approach, we systematically leave out one subject's data from the training set and use it for testing. This technique ensures that the model generalizes well to unseen subjects by evaluating its performance on each subject independently.

K-Stratified Cross-Validation: Similar to k-fold cross-validation, this technique divides the data into k folds. However, it ensures that each fold contains approximately the same proportion of samples from each class, thus addressing the class imbalance issue.

# Performance Metrics
To assess the classification algorithms' performance, we compute the following metrics:

F-measure: Also known as the F1 score, it combines precision and recall into a single metric. It provides a balanced measure of the algorithm's accuracy by considering both false positives and false negatives.

Precision: Precision measures the ratio of correctly predicted positive instances to the total number of instances predicted as positive. It indicates the algorithm's ability to avoid false positives.

Recall: Recall, also known as sensitivity or true positive rate, measures the ratio of correctly predicted positive instances to the total number of actual positive instances. It indicates the algorithm's ability to identify all positive instances.

ROC Curve with Confusion Matrix: The receiver operating characteristic (ROC) curve visualizes the trade-off between true positive rate (TPR) and false positive rate (FPR) for different classification thresholds. Additionally, the confusion matrix provides a tabular representation of the classification results, showing the counts of true positives, true negatives, false positives, and false negatives.

# Conclusion
This project aims to develop effective classification algorithms for predicting the sensitization type in EHR-Pancreatic data. By utilizing three different algorithms, applying various cross-validation techniques, and computing multiple performance metrics, we strive to improve the accuracy and generalization capability of the models. The provided code and documentation in this repository enable others to understand and reproduce the results, as well as further enhance the classification models for EHR-Pancreatic data.


