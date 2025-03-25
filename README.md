# Support Vector Machine (SVM) Lab

This repository contains the implementation of a Support Vector Machine (SVM) model for classification tasks. The main notebook for this lab is [`Main.ipynb`](./Main.ipynb).

## Overview

The notebook demonstrates the following key steps in building and evaluating SVM models:

### 1. **Data Preprocessing**

- **Data Generation**: Synthetic data is generated using `make_classification` with 3 classes and 2 features.
- **Data Visualization**: Scatter plots are used to visualize the generated data.

### 2. **Data Splitting**

- The dataset is split into training and testing sets using `train_test_split` with a 70-30 split.

### 3. **Model Training**

- Two SVM models are trained:
  - **Linear Kernel**: A linear SVM model is trained and evaluated.
  - **RBF Kernel**: A radial basis function (RBF) SVM model is trained and evaluated.

### 4. **Hyperparameter Tuning**

- Hyperparameters `C` and `gamma` are tuned using `GridSearchCV` to optimize the RBF SVM model.
- The best parameters are identified and used to train a tuned RBF SVM model.

### 5. **Support Vector Analysis**

- The support vectors are extracted and analyzed to understand their distribution and influence on the decision boundary.

### 6. **Decision Boundary Visualization**

- Decision boundaries for the linear SVM, RBF SVM, and tuned RBF SVM models are visualized using `plot_decision_regions`.

### 7. **Model Evaluation**

- **Classification Reports**: Detailed classification metrics (precision, recall, F1-score) are generated for all models.
- **Confusion Matrices**: Confusion matrices are plotted to evaluate model performance.

## Key Features

- **Hyperparameter Tuning**: Demonstrates the impact of `C` and `gamma` on model performance.
- **Visualization**: Includes visualizations for data distribution, decision boundaries, and confusion matrices.
- **Support Vector Analysis**: Highlights the role of support vectors in SVM models.

## Dependencies

The following Python libraries are required to run the notebook:

- `scikit-learn`
- `numpy`
- `matplotlib`
- `pandas`
- `mlxtend`

## How to Run

1. Clone the repository.
2. Install the required dependencies.
3. Open `Main.ipynb` in Jupyter Notebook or JupyterLab.
4. Run the cells sequentially to reproduce the results.

## Results

- **Linear SVM**: Provides a baseline accuracy.
- **RBF SVM**: Improves accuracy over the linear model.
- **Tuned RBF SVM**: Achieves the best accuracy with optimized hyperparameters.