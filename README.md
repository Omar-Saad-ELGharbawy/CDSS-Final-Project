EEG Feature Extraction
# Mental State Classification using EEG

## Table of contents:
- [Introduction](#introduction)
- [Methodology](#methodology)
- [Data Set and Feature Extraction](data-set-and-feature-extraction)
- [Feature Selection Algorithms](feature-selection-algorithms)
- [Machine Learning Algorithms](machine-learning-algorithms)
- [Results and Discussion](#results-and-discussion)
- [Report](report)
- [Research Poster](research-poster)


---

## Introduction

### Problem Definition
Automatic detection of mental states, whether related to cognition or emotions, has numerous potential applications across various domains, including healthcare, education, neuroscience, and robotics.

### Solution Approach
This project focuses on classifying mental states using EEG signals collected from the Muse headband, offering a cost-effective and versatile solution for mental state classification.

---

## Methodology

1. **Searching for Data**: Utilized existing EEG databases for model training.
2. **Data Processing**: Cleaned and normalized data to remove noise.
3. **Feature Extraction**: Extracted features from EEG signals using statistical and time-frequency techniques.
4. **Feature Selection**: Selected the most important features using variance, correlation, mutual information filter, and univariate ROC AUC methods.
5. **Model Training**: Trained machine learning models (Naive Bayes, SVM, Decision Tree, Random Forest, KNN) on the selected features.
6. **Model Evaluation**: Evaluated models using cross-validation techniques and various performance metrics.

---

## Literature Review

EEG signals have been widely used to classify mental states and diagnose neurological diseases. Previous studies have employed machine learning techniques such as SVM, ANN, and Random Forest to achieve high accuracy in mental state classification.

---

## Data Set and Feature Extraction

The data set comprised EEG signals collected from Muse headbands, with feature extraction focusing on statistical, Shannon entropy, log-energy entropy, and frequency domain features.

---

## Feature Selection Algorithms

Utilized filter-based feature selection methods including Variance, Correlation, Mutual Information Filter, and Univariate ROC AUC to reduce data complexity and improve model performance.

---

## Machine Learning Algorithms

Evaluated various machine learning models including Naive Bayes, SVM, Decision Tree, Random Forest, and KNN, with Random Forest performing the best in terms of accuracy and generalization.

---

## Results and Discussion

Achieved a high accuracy of 97.6% using the Random Forest model, indicating the effectiveness of the selected features and model in classifying mental states. Future research could explore more complex models and additional features for further improvement.

---

## Report

![Report](link/to/your/block_diagram.png)

## Research Poster
![Poster](link/to/your/block_diagram.png)
![ResearchPoster-Team 4](https://github.com/Omar-Saad-ELGharbawy/CDSS-Final-Project/assets/84602951/19717ad6-43cf-438c-a5f9-f4a7febfa905)


---

