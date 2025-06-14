## Coding Workflow

### Data Loading and Preprocessing

- Loaded the heart disease dataset from CSV.
- Cleaned the data by handling missing values and encoding categorical variables.
- Converted relevant columns (e.g., TRUE/FALSE to 1/0).
- Created a binary target variable for classification tasks.

### Feature Engineering

- Selected appropriate features for regression and classification.
- Created new target variables as required by the assignment.

### Train-Test Split and Scaling

- Split the dataset into training and testing sets for both regression and classification tasks.
- Standardized features using appropriate scaling techniques.

### Regression Modeling

- Implemented ElasticNet regression to predict cholesterol levels.
- Tuned regularization parameters (`alpha` and `l1_ratio`) using grid search.
- Evaluated model performance using R² and RMSE metrics.
- Visualized performance across hyperparameters using heatmaps.
- Identified and reported the optimal configuration.

### Classification Modeling

- Trained and evaluated Logistic Regression and k-Nearest Neighbors (k-NN) classifiers to predict heart disease presence.
- For Logistic Regression, experimented with different penalties and solvers.
- For k-NN, tuned the `n_neighbors` hyperparameter and compared results.
- Used accuracy, F1 score, AUROC, and AUPRC as evaluation metrics.
- Plotted ROC and Precision-Recall curves for the best models.

### Model Interpretation

- Analyzed model coefficients and feature importances for interpretability.
- Compared model performances based on evaluation metrics and visualizations.

