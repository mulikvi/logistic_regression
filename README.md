# Logistic Regression on the Iris Dataset

This project demonstrates the implementation of a logistic regression classifier on the Iris dataset, addressing both linearly separable and non-linearly separable binary classification problems. The project includes the following steps:

## Steps Involved

### 1. **Data Preprocessing**
- The Iris dataset is loaded and preprocessed:
  - Features are rescaled.
  - The dataset is shuffled to ensure randomness during training.
- The dataset is split into two binary classification tasks:
  - **Task A**: Class 0 vs. Class 1 (linearly separable).
  - **Task B**: Class 1 vs. Class 2 (non-linearly separable).

### 2. **Model Implementation**
- A custom `logisticClassify2` class is defined for logistic regression:
  - Includes methods for training using **Stochastic Gradient Descent (SGD)**.
  - Methods for **prediction** and **visualization of decision boundaries** are provided.

### 3. **Boundary Visualization**
- The decision boundaries for both classification tasks (A and B) are visualized:
  - This helps to observe how the logistic regression model performs on linearly separable data vs. non-linearly separable data.

### 4. **Model Training**
- The logistic regression model is trained using **Stochastic Gradient Descent (SGD)** on both binary classification tasks (A and B).
- The training process includes the plotting of:
  - Convergence of the **error rate** over epochs.
  - Convergence of the **negative log-likelihood (NLL) loss** during training.

### 5. **Regularization**
- **L2 Regularization** (Ridge regularization) is applied to mitigate overfitting:
  - Particularly useful for datasets with small feature sets like the Iris dataset.
  - L2 regularization penalizes large coefficients but does not lead to sparsity, helping the model generalize better.

### 6. **Results**
- After training, the model’s performance on both datasets is evaluated:
  - **Decision boundaries** and **classifier errors** are plotted.
  - The classifier performs well on the linearly separable data (Task A) but shows less effective results on the non-linearly separable data (Task B).

## Requirements

- `numpy`
- `matplotlib`
- `mltools` (custom tools)

