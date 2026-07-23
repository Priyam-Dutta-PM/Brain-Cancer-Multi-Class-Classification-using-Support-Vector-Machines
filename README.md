# Brain-Cancer-Multi-Class-Classification-using-Support-Vector-Machines
Gene expression-based brain cancer classification using SVM with PCA, RFE, and hyperparameter tuning.
# 📈 Results

The Support Vector Machine classifier demonstrated strong performance in classifying five brain tumor categories using gene expression data. Multiple feature selection techniques were evaluated, and all achieved consistent classification performance, highlighting the robustness of the SVM model.

## Overall Test Performance

| Metric | Score |
|--------|------:|
| Accuracy | **92.31%** |
| Precision | **93.27%** |
| Recall | **92.31%** |
| F1-score | **92.31%** |

---

## Feature Selection Comparison

| Feature Selection Method | Accuracy | Precision | Recall | F1-score |
|-------------------------|---------:|----------:|--------:|---------:|
| Variance Threshold | **92.31%** | **93.27%** | **92.31%** | **92.31%** |
| Principal Component Analysis (PCA) | **92.31%** | **93.27%** | **92.31%** | **92.31%** |
| Recursive Feature Elimination (RFE) | **92.31%** | **93.27%** | **92.31%** | **92.31%** |

---

## Hyperparameter Optimization

Grid Search Cross-Validation was performed to determine the optimal SVM hyperparameters.

| Feature Set | Best Parameters | Best Cross-Validation Accuracy |
|-------------|----------------|-------------------------------:|
| Variance Threshold | C = 10, RBF Kernel | **96.19%** |
| PCA | C = 10, RBF Kernel | **96.19%** |
| RFE | C = 1, RBF Kernel | **100.00%** |

---

## ROC-AUC Performance by Tumor Type

| Brain Tumor Class | ROC-AUC |
|-------------------|--------:|
| Glioblastoma | **1.0000** |
| Normal | **1.0000** |
| Medulloblastoma | **0.9773** |
| Pilocytic Astrocytoma | **0.9710** |
| Ependymoma | **0.9281** |

---

## Key Findings

- The SVM classifier achieved an overall **test accuracy of 92.31%** across five brain tumor classes.
- Variance Threshold, PCA, and Recursive Feature Elimination produced **identical classification performance**, indicating that the classifier remained robust under different feature selection strategies.
- Hyperparameter tuning using Grid Search improved cross-validation accuracy, with the **RFE feature set achieving 100% cross-validation accuracy** using an RBF kernel.
- ROC-AUC scores exceeded **0.92 for every tumor class**, with perfect discrimination for **Glioblastoma** and **Normal** tissue samples.
- The model generalized well despite the high-dimensional nature of gene expression data, demonstrating the suitability of Support Vector Machines for bioinformatics classification tasks.

---

## Repository Outputs

- ✅ Exploratory Data Analysis
- ✅ Feature Selection (Variance Threshold, PCA, RFE)
- ✅ Hyperparameter Optimization (GridSearchCV)
- ✅ Confusion Matrix
- ✅ Classification Report
- ✅ ROC Curves
- ✅ ROC-AUC Comparison
- ✅ Performance Metrics Comparison
- ✅ Test Prediction Analysis
