# Sampling Techniques on Imbalanced Credit Card Dataset

## Objective
The objective of this assignment is to understand the importance of sampling techniques in handling imbalanced datasets and to analyze how different sampling strategies affect the performance of various machine learning models.

---

## Dataset
The dataset used is a credit card dataset containing transaction details with a highly imbalanced target variable:
- Class 0: Non-fraudulent transactions (majority class)
- Class 1: Fraudulent transactions (minority class)

Due to the imbalance, machine learning models may become biased toward the majority class, making sampling techniques necessary.

---

## Sampling Techniques Used
The following five sampling techniques were applied to balance the dataset:

1. Sampling1 – Random Under Sampling  
2. Sampling2 – Random Over Sampling  
3. Sampling3 – SMOTE (Synthetic Minority Over-sampling Technique)  
4. Sampling4 – NearMiss  
5. Sampling5 – Tomek Links  

Each technique balances the dataset in a different way to study its effect on model performance.

---

## Machine Learning Models Used
Five different machine learning models were trained on each sampled dataset:

- M1 – Logistic Regression  
- M2 – K-Nearest Neighbors (KNN)  
- M3 – Decision Tree Classifier  
- M4 – Random Forest Classifier  
- M5 – Support Vector Machine (SVM)  

---

## Results
The accuracy of each model under different sampling techniques is summarized below:

| Model | Sampling1 | Sampling2 | Sampling3 | Sampling4 | Sampling5 |
|------|-----------|-----------|-----------|-----------|-----------|
| M1 | 66.67 | 91.70 | 90.39 | 50.00 | 98.70 |
| M2 | 16.67 | 98.47 | 84.72 | 83.33 | 98.70 |
| M3 | 66.67 | 98.91 | 97.82 | 16.67 | 98.26 |
| M4 | 33.33 | 100.00 | 99.34 | 16.67 | 98.70 |
| M5 | 16.67 | 68.56 | 67.69 | 16.67 | 98.70 |
---

## Analysis
- Sampling5 (Tomek Links) provides consistently high accuracy across almost all models.
- Sampling2 (Random Over Sampling) performs exceptionally well, especially with Random Forest.
- Sampling4 (NearMiss) results in lower accuracy for most models due to excessive removal of majority class samples.
- Tree-based models benefit significantly from balanced datasets.

---

## Conclusion
This study shows that sampling techniques play a crucial role in improving model performance on imbalanced datasets. Over-sampling and hybrid methods such as Random Over Sampling and Tomek Links generally provide better accuracy compared to under-sampling techniques. The best sampling technique depends on the machine learning model used, and no single method is universally optimal.

---


