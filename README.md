---

# Credit Card Data Sampling Project

## Overview

This project involves sampling credit card data to create a balanced dataset for further analysis and modeling. The aim is to address issues of class imbalance and ensure that the dataset is suitable for training machine learning models.

## Table of Contents

1. [Introduction](#introduction)
2. [Evaluation Metrics](#evaluation-metrics)
3. [Results](#results)
4. [Conclusion](#conclusion)
5. [Usage](#usage)


## Introduction

Credit card datasets often suffer from class imbalance, where fraudulent transactions are significantly outnumbered by non-fraudulent ones. This project applies various sampling techniques to balance the dataset, improving the performance of machine learning models in detecting fraudulent transactions.
  
## Evaluation Metrics

The effectiveness of the sampling techniques was evaluated using the following metrics:
- **Class Distribution**: Ensures the dataset is balanced.
- **Model Performance Metrics**: Evaluates the impact of sampling on model performance using metrics such as Accuracy, Precision, Recall, F1-Score, and Area Under the ROC Curve (AUC).

## Results

The results of applying different sampling techniques are summarized below:

### Random Undersampling
- Balanced class distribution.
- Moderate model performance due to loss of majority class information.

### Random Oversampling
- Balanced class distribution.
- Improved model performance but increased risk of overfitting.

### SMOTE
- Balanced class distribution.
- Enhanced model performance with better generalization.

### ADASYN
- Balanced class distribution.
- Similar performance to SMOTE, with a focus on harder-to-learn instances.

### Cluster Centroids
- Balanced class distribution.
- Moderate model performance, with potential loss of information.

### Model Performance Summary
- **Best Technique**: SMOTE achieved the best balance between class distribution and model performance.

## Conclusion

Sampling techniques effectively address class imbalance in the credit card dataset. SMOTE and ADASYN are particularly effective in improving model performance while maintaining a balanced dataset. These techniques should be considered for handling imbalanced datasets in fraud detection and similar applications.
  

## Usage

To reproduce the results:
1. Clone the repository:
   ```bash
   git clone [repository URL]
   ```
2. Install the required libraries:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the Jupyter notebook:
   ```bash
   jupyter notebook credit_card_sampling.ipynb
   ```  

This README provides a detailed overview of the credit card data sampling project, guiding users through the purpose, methods, results, and how to replicate the study.
