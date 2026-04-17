# 🌲 Breast Cancer Classification – Random Forest

A machine learning project that classifies breast tumors as **Malignant (M)** or **Benign (B)** using a **Random Forest** classifier. This is part of a hands-on group exercise comparing multiple ML algorithms on the same dataset.

---

## 📁 Dataset

**Wisconsin Breast Cancer Dataset** (`data.csv`)

- **569 samples** — 212 Malignant, 357 Benign
- **30 numeric features** derived from digitized images of fine needle aspirate (FNA) of breast masses

---

## 📂 Project Structure

```
├── data.csv                        # Wisconsin Breast Cancer dataset
├── random_forest_cancer.ipynb      # Main Jupyter notebook
└── README.md                       # This file
```

---

## 📊 Expected Results

| Metric | Benign | Malignant |
|--------|--------|-----------|
| Precision | ~97–99% | ~95–97% |
| Recall | ~97–99% | ~94–96% |
| F1-Score | ~97–98% | ~95–96% |
| **Overall Accuracy** | **~96–97%** | |

---

## 📈 Visualizations

### Confusion Matrix
Shows the number of correct and incorrect predictions broken down by class (Benign vs Malignant).

### Feature Importances
Bar chart of the top 10 most influential features used by the Random Forest — typically `concave points_worst`, `perimeter_worst`, and `radius_worst` rank highest.

---

## 🛠 Tech Stack

| Tool | Purpose |
|------|---------|
| Python 3.x / Pyodide | Runtime |
| scikit-learn | Random Forest model & evaluation metrics |
| pandas | Data loading and manipulation |
| matplotlib | Plotting |
| seaborn | Confusion matrix heatmap |

---

## 📌 Key Notes

- **No feature scaling required** — Random Forests are tree-based and not sensitive to feature magnitudes
- `random_state=42` is set for full reproducibility
- `stratify=y` in the train/test split ensures both sets maintain the original class distribution
- The model uses 100 trees (`n_estimators=100`) which balances performance and speed well for this dataset size



