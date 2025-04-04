# 🚀 Predicting ICO Success Using Machine Learning

This project uses various machine learning algorithms to predict whether an Initial Coin Offering (ICO) will succeed or fail. The project follows the CRISP-DM methodology and compares multiple classification models based on performance metrics.

📄 **Full Report:** [Utilising Machine Learning to Forecast ICO Success (PDF)](./Utilising%20Machine%20Learning%20to%20Forecast%20ICO%20success.pdf)

---

## 📊 Project Overview

- **Dataset:** 2,395 ICOs with 16 variables (numeric, categorical, binary)
- **Objective:** Predict the `success` of ICO projects using classification models
- **Target Variable:** Binary factor (`1` = success, `0` = fail)

---

## 🧪 Models Applied

| Algorithm | Technique | Note |
|-----------|-----------|------|
| `KNN` | Majority vote based on k-nearest neighbors | Tuned with k = 49 |
| `Naive Bayes` | Bayes Theorem + Laplace Smoothing | Low F1 score |
| `Decision Tree (C5.0)` | Tree-based with boosting iterations | 🏆 Best model (F1 = 0.501) |
| `SVM` | Linear, polynomial, RBF, sigmoid kernels | Good performance |
| `ANN` | Neural network with 1–3 hidden neurons | Competitive performance |

---

## 📈 Key Evaluation Metrics

- **Accuracy, Precision, Recall, F1 Score**
- **ROC Curve & AUC** comparison across models
- **Feature Importance** (e.g., ICO `Rating` was the strongest predictor)

---

## 🧠 Results Summary

- **Best Model:** Decision Tree with 5 boosting trials  
- **Top Features:** ICO Rating, Team Size, Duration, Reddit presence  
- **ANN and SVM** performed well, but DT slightly outperformed  
- Naive Bayes performed poorly due to low precision

---

## 🛠 Tools Used

- **Language:** R  
- **Libraries:** `tidyverse`, `C50`, `neuralnet`, `e1071`, `kernlab`, `caret`, `ROCR`  
- **Evaluation:** Confusion matrix, ROC curve, AUC, F1 score

---

## 🔜 Future Work

- Handle skewed distributions and outliers  
- Use SMOTE or balancing techniques for class imbalance  
- Try deep learning or ensemble methods

---
