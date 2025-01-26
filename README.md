Credit Card Fraud Detection: Sampling and Model Evaluation
Project Overview:
This project aims to tackle the issue of class imbalance in credit card fraud detection datasets and evaluate the performance of various machine learning models under different sampling techniques. The dataset used is sourced from the provided credit card transaction data, with Class as the target variable (0 = legitimate, 1 = fraud).

Objectives:
Balance the imbalanced dataset using SMOTE (Synthetic Minority Oversampling Technique).
Create 5 different samples of varying sizes.
Apply 5 different sampling techniques to generate training subsets.
Train and evaluate 5 machine learning models on these samples:
Logistic Regression
Random Forest Classifier
Decision Tree Classifier
Support Vector Machine (SVM)
K-Nearest Neighbors (KNN)
Determine which sampling technique yields the highest accuracy for each model.
Methodology
Data Preprocessing:

Loaded and analyzed the Creditcard_data.csv dataset.
Balanced the classes using SMOTE to create an even distribution of legitimate and fraudulent transactions.
Sampling:

Generated 5 samples of varying sizes using the formula:
Sample Size
=
Total Data Points
×
0.2
×
𝑖
(where 
𝑖
 ranges from 1 to 5)
Sample Size=Total Data Points×0.2×i(where i ranges from 1 to 5)
Machine Learning Models:

Trained the models on each sampled dataset.
Used stratified splitting to ensure consistent class proportions during training and testing.
Performance Metrics:

Evaluated model performance using Accuracy as the primary metric.
Tabulated results for each sampling technique and model pair.
Results
The results are summarized in the sampling_model_results.csv file, which contains:

Model name
Sampling technique
Accuracy score
The best sampling technique for each model is also highlighted in the final summary.

Key Findings
Models performed differently depending on the sampling technique and sample size.
SMOTE proved effective in balancing the dataset and improving model performance on minority class predictions.
Specific sampling techniques paired with certain models resulted in the highest accuracy.
Repository Contents
Creditcard_data.csv: Original dataset.
sampling_assignment.py: Python script for the entire analysis.
sampling_model_results.csv: Results of the evaluation across models and sampling techniques.
