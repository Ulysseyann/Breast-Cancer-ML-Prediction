#  Breast Cancer Prediction with Machine Learning

This project applies **machine learning algorithms** to predict:
- Whether a breast cancer patient is likely to survive (classification).
- How many months a patient might survive (regression).

It uses **clinical data** with features like tumor size, hormone status, and cancer staging to build robust predictive models.

---

##  Case Studies

###  Case Study A – Classification (Mortality Status)
**Goal**: Predict whether a patient is “Alive” or “Dead”.

#### Models Used:
- Logistic Regression
- K-Nearest Neighbors (KNN)
- Naïve Bayes
- Ensemble (Voting Classifier)

#### Key Metrics:
- **Recall** prioritized due to class imbalance
- Precision, F1-score, and AUC-ROC also considered

#### Best Model: 
 Naïve Bayes (Highest Recall and F1-score)

---

###  Case Study B – Regression (Survival Months)
**Goal**: Predict the number of months a patient is likely to survive.

#### Models Used:
- Decision Tree Regressor (DT-1: Fully grown)
- Decision Tree Regressor (DT-2: Pre-pruned)

#### Evaluation Metrics:
- Mean Squared Error (MSE)
- Mean Absolute Error (MAE)
- R² Score

#### Best Model: 
 DT-2 (Pre-pruned Decision Tree)

---

##  Dataset Info
- Derived from real-world clinical attributes
- Preprocessed with:
  - IQR-based outlier removal
  - Mean/Mode imputation
  - Label encoding for categorical data
  - Stratified train-test split

---

##  Tech Stack

| Tool | Purpose |
|------|---------|
| Python | Programming |
| scikit-learn | Modeling + Evaluation |
| NumPy, Pandas | Data processing |
| Matplotlib, Seaborn | Visualization |
| Jupyter Notebook / Colab | Development |

---

##  Results Highlights

| Model | Task | Best Metric |
|-------|------|-------------|
| Naïve Bayes | Classification | Recall = 0.40 |
| Decision Tree (DT-2) | Regression | MAE = 18.56, MSE = 527.85 |

---

##  Why This Matters
This project demonstrates how **model evaluation, preprocessing, and metric selection** are critical in sensitive domains like healthcare. Wrong predictions can lead to severe ethical and clinical consequences. Hence, models were tuned for **interpretability and recall** over plain accuracy.

---

##  How to Run

1. Clone the repo
```bash
git clone https://github.com/YOUR_USERNAME/breast-cancer-ml-prediction.git
cd breast-cancer-ml-prediction
