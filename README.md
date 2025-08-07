# 🧪 Melanoma vs Nevi Classification

This project aims to develop a deep learning model to differentiate between **melanoma** (a potentially deadly form of skin cancer) and **nevi** (commonly known as moles, usually benign). It is based on the HAM10000 dataset and focuses on binary classification for clinical decision support.

---

## 🔬 Clinical Relevance

- **Melanoma** is an aggressive skin cancer that can spread quickly if not detected early.
- **Nevi**, on the other hand, are **benign skin lesions** that rarely require treatment.
- Early and accurate differentiation between the two can **improve survival rates**, reduce unnecessary biopsies, and assist dermatologists, especially in regions lacking expert diagnostic services.

---

## 📊 Model Performance

| Metric                  | Value    |
|-------------------------|----------|
| Test Accuracy           | 88.87%   |
| Test Loss               | 0.2476   |
| ROC AUC Score           | 0.9291   |
| Optimal Threshold (ROC) | 0.7661   |
| Optimal Threshold (F1)  | 0.2671   |

**Classification Report:**

| Class        | Precision | Recall | F1-score | Support |
|--------------|-----------|--------|----------|---------|
| Melanoma (0) | 0.82      | 0.56   | 0.66     | 111     |
| Nevi (1)     | 0.93      | 0.98   | 0.95     | 671     |

- **Macro Avg F1-score:** 0.81
- **Weighted Avg F1-score:** 0.91

> 📌 Limitation: While the model performs very well overall, recall for melanoma (0.56) could be improved further, as missing melanoma cases can have severe consequences.

---

## 🧠 Techniques Used

- Transfer learning with EfficientNetB3
- Custom image preprocessing: **Gamma Correction** and **Contrast Stretching**
- Evaluation: ROC Curve, Optimal Thresholding for ROC & F1
- Loss Function: `binary_crossentropy`
- Performance metrics: Accuracy, ROC AUC, Classification Report

---
