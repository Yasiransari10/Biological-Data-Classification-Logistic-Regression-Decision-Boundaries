# 🍃 Biological Data Classification: Logistic Regression & Decision Boundaries

## Project Overview
[span_3](start_span)This project involves building and evaluating statistical classification models to distinguish between two distinct biological species based on their morphological features (leaf length and width)[span_3](end_span). [span_4](start_span)The objective is to demonstrate the application of logistic regression and analyze the bias-variance trade-off[span_4](end_span).

## Tech Stack & Libraries Used
* **[span_5](start_span)Language:** R[span_5](end_span)
* **[span_6](start_span)[span_7](start_span)Data Manipulation:** `tidyverse`, `magrittr`[span_6](end_span)[span_7](end_span)
* **[span_8](start_span)[span_9](start_span)Machine Learning:** `caret`, `pROC`[span_8](end_span)[span_9](end_span)
* **[span_10](start_span)Visualization:** `ggplot2`[span_10](end_span)

## Methodology
1. **[span_11](start_span)[span_12](start_span)Model Training:** Fitted a baseline linear logistic regression model alongside non-linear polynomial logistic regression models (degrees 2, 3, and 4)[span_11](end_span)[span_12](end_span).
2. **[span_13](start_span)[span_14](start_span)Rigorous Evaluation:** Partitioned the data using a 30% unseen hold-out test set to ensure the models were evaluated on real-world generalization capability[span_13](end_span)[span_14](end_span).
3. **[span_15](start_span)Metric Tracking:** Evaluated model performance across Accuracy, Sensitivity, Specificity, and Area Under the Curve (AUC) [cite: 209-215].

## Quantifiable Results & Impact
| Model | Accuracy | Sensitivity | Specificity | AUC |
| :--- | :--- | :--- | :--- | :--- |
| **Baseline** | 81.1% | 85.3% | 75.9% | 0.877 |
| **Polynomial Degree 2** | **84.4%** | **85.3%** | **83.3%** | **0.940** |
| **Polynomial Degree 4** | 86.1% | 86.8% | 85.2% | 0.948 |


## Strategic Conclusion
[cite_start]The **Degree 2 Polynomial Model** was selected as the optimal solution[span_15](end_span). [span_16](start_span)[span_17](start_span)While higher-degree models yielded slightly better raw metrics, they resulted in overly irregular decision boundaries that were deemed biologically implausible and indicative of overfitting[span_16](end_span)[span_17](end_span). [span_18](start_span)The Degree 2 model provides the best balance of predictive power and real-world interpretability[span_18](end_span).
