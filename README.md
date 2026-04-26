# Biological-Data-Classification-Logistic-Regression-Decision-Boundaries
Project Overview
This project involves building and evaluating statistical classification models to distinguish between two distinct biological species (Species A and Species B) based on their morphological features (leaf length and width).[1] The objective is to demonstrate the application of logistic regression, analyze the bias-variance trade-off, and visualize complex decision boundaries to identify the most robust and generalizable model.[1]
Tech Stack & Libraries Used
•	Language: R [1]
•	Data Manipulation & Cleaning: tidyverse, magrittr [1]
•	Machine Learning & Evaluation: caret, pROC [1]
•	Data Visualization: ggplot2 [1]
Methodology
	1.	Model Training: Fitted a baseline linear logistic regression model alongside non-linear polynomial logistic regression models (degrees 2, 3, and 4) to capture complex data relationships.[1]
	2.	Rigorous Evaluation: Partitioned the data using a 30% unseen hold-out test set to ensure the models were evaluated on real-world generalization capability rather than training data memorization.[1]
	3.	Metric Tracking: Evaluated model performance across four primary metrics: Accuracy, Sensitivity, Specificity, and Area Under the Curve (AUC).[1]
	4.	Visual Diagnostics: Generated scatter plots, Receiver Operating Characteristic (ROC) curves, and decision region contour maps to visually audit model boundaries.[1]
Quantifiable Results & Impact
•	Baseline Linear Model: Achieved 81.1% Accuracy and an AUC of 0.877.[1]
•	Polynomial Degree 2 Model: Improved performance significantly, achieving 84.4% Accuracy and an AUC of 0.940.[1]
•	Polynomial Degree 3 & 4 Models: Achieved the highest metrics (up to 86.0% Accuracy and 0.947 AUC).[1]
Strategic Conclusion
While the Degree 4 polynomial model yielded the highest raw statistical metrics, a bias-variance analysis revealed potential overfitting.[1] The highly irregular decision boundary of the Degree 4 model was deemed biologically implausible for leaf morphology.[1] Therefore, the Degree 2 Polynomial Model was selected as the optimal solution, providing the best balance of high predictive power (0.940 AUC) and real-world interpretability.[1]
Your Next Step:
Once you have committed this README to your GitHub repository, you must add the direct URL link to this specific repository into your resume next to the "Statistical Modelling & Classification Analysis" project title. This proves to employers that your skills are real and verifiable. Let me know when this is done.
