
# Mental State Classification using EEG

## Table of contents:
- [Introduction](#introduction)
- [Methodology](#methodology)
- [Used Technologies](#used-technologies)
- [Results](#results)
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

The methodology for this project involves the following steps:

#### Data Search: 
Find datasets containing EEG signals labeled with different mental states.
#### Data Processing: 
Clean and pre-process the data to remove noise and normalize features.
#### Feature Extraction:
Extract relevant features from the EEG signals that can be used to distinguish between different mental states. These features may include statistical measures, frequency domain features, and phase synchronization.
#### Feature Selection: 
Select the most important features to improve model performance and reduce overfitting. This can be done using various techniques like variance, correlation, mutual information, and ROC AUC.
#### Machine Learning Model Evaluation:
Evaluate different machine learning models, such as Naive Bayes, Support Vector Machines (SVM), Decision Trees, Random Forests, and K-Nearest Neighbors (KNN), to classify mental states.
#### Model Training:
Train the best performing model on the entire dataset.
#### Testing: 
Test the trained model on unseen data to evaluate its generalizability.
---

## Used Technologies

- Data Acquisition: EEG recording device (e.g., Muse headband)
- Data Processing Libraries: MNE-Python, EEGLab
- Feature Extraction Libraries: EEGLab, SciPy, NumPy
- Feature Selection Libraries: scikit-learn
- Machine Learning Libraries: scikit-learn, TensorFlow
---

## Results

The Random Forest model emerged as the best performer, achieving an average accuracy of 97.4% using 10-fold cross-validation. This technique helps prevent overfitting and provides a more reliable estimate

---

## Report

![Report](link/to/your/block_diagram.png)

## Research Poster
![Poster](link/to/your/block_diagram.png)
![ResearchPoster-Team 4](https://github.com/Omar-Saad-ELGharbawy/CDSS-Final-Project/assets/84602951/19717ad6-43cf-438c-a5f9-f4a7febfa905)


---

