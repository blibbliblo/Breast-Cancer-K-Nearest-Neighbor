# Breast-Cancer-K-Nearest-Neighbor

Breast Cancer Classification with K-Nearest Neighbors (KNN)

Project Goal
 - To build and optimize a KNN classifier for breast cancer diagnosis (Benign/Malignant) using features from digitized FNA images

Dataset
 - [Breast Cancer Wisconsin (Diagnostic)](https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data) dataset: 569 instances, 32 features

Steps
 - Data Cleaning: removed "Unnamed: 32" column (all NaNs) and "id" column
 - Data Split: split data into training and testing (80:20)
 - Custom Feature Scaling: manual standardization (mean=0 and std=1) based on training data
 - Custom KNN Model: used KNN class with euclidean_distance for classification (no scikit-learn)
 - Hyperparameter Optimization: tuned k (number of neighbors) from 1 to 50 to find the best accuracy
 - Visualization: plotted data distribution and model predictions on scaled test data

Results & Conclusion
 - Preprocessing (adress NaN) improved accuracy
 - Achieved optimal accuracy with k=3
 - Scaling and processing becomes essential when dealing with distance-based models like KNN
