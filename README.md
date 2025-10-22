# Credit Card Fraud Detection (Random Forest Classifier)

This project detects fraudulent credit card transactions using a **Random Forest Classifier** trained on the Kaggle Credit Card Fraud dataset.  
It includes data preprocessing, visualization, model training, and evaluation — implemented in Google Colab and structured for GitHub.

---

## Repository Structure

```
ML_Credit_Card_Fraud_Detection/
│
├── data/
│   ├── creditcard.csv        # (ignored in GitHub; download from Kaggle)
│   └── README.md             # Dataset info and link
│
├── results/
│   ├── metrics.txt           # Model evaluation summary
│   └── confusion_matrix.png  # Confusion matrix visualization
│
├── visuals/
│   ├── class_distribution.png
│   ├── correlation_heatmap.png
│   ├── feature_boxplots.png
│   ├── roc.png
│   └── confusion_matrix.png
│
├── ML___Credit_Card_Fraud_Detection-.ipynb
├── requirements.txt
└── .gitignore
```

---

## Dataset

- **Source:** [Kaggle – Credit Card Fraud Detection](https://www.kaggle.com/mlg-ulb/creditcardfraud)
- **Size:** 284,807 transactions (492 fraudulent)
- **Target:** `Class` → 1 = Fraud, 0 = Genuine  
- Download the CSV from Kaggle and place it in `data/creditcard.csv`.

---

## Model Overview

- **Algorithm:** Random Forest Classifier  
- **Train/Test Split:** 80/20  
- **Feature Scaling:** StandardScaler  

---

## Model Performance

| Metric | Value |
|--------|--------|
| **Accuracy** | 0.9995962220 |
| **Precision** | 0.9746835443 |
| **Recall** | 0.7857142857 |
| **F1-Score** | 0.8700564971 |
| **Matthews Corr. Coeff.** | 0.8749276812 |

---

## Visualizations

| File | Description |
|------|--------------|
| `class_distribution.png` | Shows fraud vs. normal transactions |
| `correlation_heatmap.png` | Displays correlation among PCA components |
| `feature_boxplots.png` | Shows outliers in transaction amounts |
| `confusion_matrix.png` | Predicted vs. actual fraud cases |
| `roc.png` | ROC-AUC curve for classifier performance |

---

## How to Run

```bash
# Clone the repository
git clone https://github.com/amanjaiswal-07/Credit-Card-Fraud-Detection-ML-.git
cd Credit-Card-Fraud-Detection-ML-

# Install dependencies
pip install -r requirements.txt

# Open in Jupyter or Colab
jupyter notebook "ML___Credit_Card_Fraud_Detection-.ipynb"
```

---

## Requirements

```
pandas
numpy
matplotlib
seaborn
scikit-learn
```

---

## Future Improvements

- Apply class balancing (SMOTE / undersampling)  
- Hyperparameter tuning for Random Forest  
- Compare with Logistic Regression or XGBoost  

---

