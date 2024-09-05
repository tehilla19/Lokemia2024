# Project: Classification of AML and ALL Using RNA-seq Data

## Project Objective
The goal of this project is to develop a classifier to distinguish between Acute Myeloid Leukemia (AML) and Acute Lymphoblastic Leukemia (ALL) using RNA-seq data. We aim to achieve optimal model performance by utilizing various data analysis, dimensionality reduction, and model training techniques.

## Project Steps

### 1. Exploratory Data Analysis (EDA):
   * We explored the data to understand its distribution, examine relationships between variables, and identify general patterns.
   * Created graphs and visualizations to present the data structure and better understand its distribution.

### 2. Outlier Detection and Removal:
   * Used methods such as Isolation Forest and OneClassSVM to identify and remove outliers from the training and testing data.
   * Visualized the outliers and cleaned data using PCA.

### 3. Dimensionality Reduction:
   * Applied PCA to reduce the number of dimensions and improve model performance.
   * Implemented an autoencoder for automatic dimensionality reduction and to extract additional features that enhance model classification.

### 4. Model Training:
   * Trained several classifiers (such as Gradient Boosting, SVM, Random Forest) on the data after outlier removal and dimensionality reduction.
   * Used GridSearchCV for hyperparameter tuning to select the optimal settings for each classifier.
   * Performed performance evaluation using cross-validation and prediction on test data.

### 5. Results and Best Parameters

#### Support Vector Machine (SVM):
   * **Best Accuracy**: 95%
   * **Best Hyperparameters**:
     * C: 1.0
     * kernel: 'rbf' (Radial Basis Function)
     * gamma: 'scale'

#### Random Forest:
   * **Best Accuracy**: 91%
   * **Best Hyperparameters**:
     * n_estimators: 100
     * max_depth: 4
     * min_samples_split: 2

#### Gradient Boosting Classifier:
   * **Best Accuracy**: 91.2%
   * **Best Hyperparameters**:
     * n_estimators: 50
     * learning_rate: 0.1
     * max_depth: 3

Each model was tuned using GridSearchCV for hyperparameter optimization, and cross-validation was performed to ensure the robustness of the results.
