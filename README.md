# Heart Disease Prediction with Logistic Regression

A machine learning tutorial demonstrating an end-to-end Logistic Regression pipeline applied to the UCI Heart Disease (Cleveland) dataset.

**Tutorial topic:** Binary classification — predicting the presence of heart disease from 13 clinical features.  
**Author:** Matthew Jeremiah Messiah 

**Student Id:** 24136779 


---

## Overview

This repository contains:

- `heart_disease_tutorial.pdf` — A written tutorial (<2000 words) walking through the full pipeline with explanations aimed at readers who want to apply Logistic Regression in their own work.
- `heart_disease_logistic_regression.ipynb` — A fully reproducible Jupyter notebook covering data loading, EDA, preprocessing, model training, evaluation, and interpretation.

The tutorial covers:
- Why Logistic Regression suits binary classification
- How to prevent data leakage during preprocessing
- How to evaluate beyond accuracy (ROC-AUC, precision, recall)
- How to interpret model coefficients in a clinical context
- The effect of the regularisation hyperparameter C on performance

---

## Dataset

**UCI Heart Disease Dataset (Cleveland)**  
Source: https://archive.ics.uci.edu/dataset/45/heart+disease  
303 patient records, 13 features, binary target (disease present / absent).

The dataset is fetched automatically via the `ucimlrepo` package — no manual download required.

---

## Requirements

- Python 3.8+
- Jupyter Notebook or JupyterLab

Install all dependencies with:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn ucimlrepo
```

---

## How to Run

1. Clone this repository:

```bash
git clone https://github.com/mattmessie/Heart-Disease-Prediction-with-Logistic-Regression.git
cd Heart-Disease-Prediction-with-Logistic-Regression
```

2. Install dependencies:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn ucimlrepo
```

3. Launch the notebook:

```bash
jupyter notebook heart_disease_logistic_regression.ipynb
```

4. Run all cells from top to bottom. Figures will be saved automatically as `.png` files in the working directory.

---

## Repository Structure

```
Heart-Disease-Prediction-with-Logistic-Regression/
│
├── heart_disease_logistic_regression.ipynb   # Full reproducible notebook
├── heart_disease_tutorial.pdf                # Written tutorial
├── README.md                                 # This file
└── LICENSE                                   # MIT Licence
```

---

## Results Summary

| Metric | Value |
|---|---|
| 5-Fold CV Accuracy | ~84% |
| Test Accuracy | ~85% |
| ROC-AUC | ~0.92 |

---

## References

- Detrano, R. et al. (1989). International application of a new probability algorithm for the diagnosis of coronary artery disease. *American Journal of Cardiology*, 64(5), 304–310.
- Pedregosa, F. et al. (2011). Scikit-learn: Machine Learning in Python. *JMLR*, 12, 2825–2830. https://scikit-learn.org
- UCI ML Repository — Heart Disease Dataset: https://archive.ics.uci.edu/dataset/45/heart+disease
- James, G. et al. (2021). *An Introduction to Statistical Learning* (2nd ed.). Springer. https://www.statlearning.com
- Hosmer, D.W. & Lemeshow, S. (2000). *Applied Logistic Regression* (2nd ed.). Wiley.

---

## Licence

This project is licensed under the MIT Licence — see [LICENSE](LICENSE) for details.
