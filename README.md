# 🍃 Leaf Species Classification: Statistical & ML Modeling
[![R-Language](https://img.shields.io/badge/Language-R-blue.svg)](https://www.r-project.org/)
[![ML-Algorithm](https://img.shields.io/badge/Algorithm-Logistic%20Regression-orange.svg)](https://en.wikipedia.org/wiki/Logistic_regression)
[![Status](https://img.shields.io/badge/Status-Completed-green.svg)]()

### 🎯 Project Goal
Can we accurately distinguish between biological species using morphometric measurements? This project develops a predictive model to classify leaf species, focusing on the trade-off between **model complexity** and **biological plausibility**.

---

### 📊 Key Performance Metrics
I compared four different models to find the optimal balance between accuracy and overfitting:

| Model | Accuracy | AUC Score | Decision Boundary |
| :--- | :--- | :--- | :--- |
| **Baseline** | 81.1% | 0.877 | Linear (Too Simple) |
| **Poly Degree 2** | **84.4%** | **0.940** | **Smooth Curve (Best)** |
| **Poly Degree 4** | 86.1% | 0.948 | Overfit (Irregular) |

**Final Selection:** The **Polynomial Degree 2** model was chosen. While Degree 4 had a higher AUC, Degree 2 provides a more "biologically plausible" boundary that generalizes better to new data.

---

###  Model Visualizations
*Note: Upload your images to a folder named "plots" for these to appear.*

#### 1. Decision Regions
> Shows how the Degree 2 model creates a natural curve to separate species.
![Decision Boundary](plots/decision_boundary_poly2.png)

#### 2. ROC Curve Analysis
> An AUC of 0.94 demonstrates the high discriminative power of the model.
![ROC Curve](plots/roc_curve.png)

---

### 🛠️ Tech Stack & Skills
- **Statistical Modeling:** Logistic Regression (Linear & Polynomial).
- **Evaluation:** K-fold Cross-Validation, ROC/AUC, Sensitivity/Specificity.
- **Libraries:** `tidyverse`, `caret`, `pROC`, `ggplot2`.

---

### 🚀 How to Run
1. Clone the repo: `git clone https://github.com/your-username/leaf-classification.git`
2. Open `script.R` in RStudio.
3. Ensure the dataset `leaf_data.csv` is in the same directory.
