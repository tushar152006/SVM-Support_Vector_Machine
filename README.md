# SVM-Support_Vector_Machine

Task 7: Support Vector Machines (SVM)

Objective
To understand and implement Support Vector Machines (SVMs) for binary classification problems using both linear and non-linear (RBF) kernels.

Tools & Libraries
- Python
- Scikit-learn
- NumPy
- Matplotlib

Dataset
I use the 'Breast Cancer Dataset' from `sklearn.datasets`, which contains features computed from breast mass images and a binary classification target (malignant or benign).

Steps

1. Load and Prepare Data
- Load the Breast Cancer dataset.
- Split data into features `X` and target `y`.

2. Standardize Features
- Used `StandardScaler` to normalize feature values before training.

3. Train SVM with Linear Kernel
- Applied `SVC(kernel='linear')` to perform linear classification.
- Evaluated using accuracy and classification report.

4. Train SVM with RBF Kernel
- Applied `SVC(kernel='rbf')` with default `gamma='scale'`.
- Compared with linear kernel performance.

5. Visualize Decision Boundary (for 2D projection)
- Used PCA to reduce dimensions and visualize decision boundary in 2D.

6. Hyperparameter Tuning
- Tested different values of `C` and `gamma` for the RBF kernel using cross-validation.
- Reported mean accuracy for each pair.

7. Cross-Validation
- Used `cross_val_score()` to validate model performance across multiple folds.

Evaluation Metrics
- Accuracy Score
- Confusion Matrix
- Classification Report (Precision, Recall, F1-score)
- Cross-validation Mean Score

Files
- `svm_task7.ipynb` – Notebook containing all implementations.
- `svm_decision_boundary.png` – Visualization of the 2D SVM boundary.
- `README.md` – This documentation.

Key Learnings
- SVMs are powerful for both linear and non-linear classification.
- Hyperparameter tuning (`C` and `gamma`) is critical for optimal results.
- PCA helps visualize high-dimensional SVM decision boundaries.


