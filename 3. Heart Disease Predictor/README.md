# Heart Disease Prediction Using Logistic Regression (scikit-learn)

This project uses a **logistic regression model** to predict the presence of heart disease based on clinical and demographic patient data.

It demonstrates the full ML pipeline: **data preprocessing**, **EDA**, **feature scaling**, **hyperparameter tuning**, **model evaluation**, and **prediction**.

---

## Project Context

Heart disease is one of the leading causes of death worldwide. Early detection and intervention can help save lives. This project applies supervised learning to predict whether a patient is likely to have a heart condition, using a cleaned clinical dataset.

---

## Project Pipeline

### 1. Data Loading & Cleaning
- Loaded `heart_cleveland_upload.csv` using Pandas
- Removed rows with **missing values** for simplicity

### 2. Exploratory Data Analysis (EDA)
- Checked **class balance** (target variable: condition present or not)
- Visualized:
  - Age and sex distributions
  - Bar charts and pie charts for heart condition split
  - Boxplots comparing age vs condition
  - Correlation heatmap (with actual values)

### 3. Feature Scaling & Splitting
- Extracted features `X` and target `y`
- Split data into **80% training** / **20% testing**
- Applied **StandardScaler** to normalize feature values

### 4. Model Training
- Trained a **Logistic Regression** model using `scikit-learn`
- Used `GridSearchCV` with **5-fold cross-validation** to tune:
  - Regularization parameter (`C`)
  - Penalty (`l1` / `l2`)
  - Solver (`liblinear`, etc.)

### 5. Evaluation
- Chose the **best model** from grid search
- Evaluated using:
  - **Accuracy**
  - **Precision**
  - **Recall**
  - **F1-Score**
- Displayed full **classification report**

### 6. Prediction
- Used the final trained model to make predictions on test data

---

## Dataset Overview

| Feature | Description |
|---------|-------------|
| `age` | Age of patient |
| `sex` | 0 = female, 1 = male |
| `...` | Various clinical indicators (e.g., cholesterol, blood pressure, etc.) |
| `condition` | Target variable: 1 = heart disease, 0 = no disease |

> ⚠️ Note: Dataset had missing values which were **dropped**.

---

## Results

- **Best Parameters** from GridSearchCV:  
  Example: `{'C': 1, 'penalty': 'l1', 'solver': 'liblinear'}`

- **Best Cross-Validation Accuracy**: ~85%  
- **Test Set Accuracy**: ~75%

- **Classification Report** includes:
  - Class-wise **precision**, **recall**, **F1-score**

---

## Key Visualizations

- **Bar charts**: Heart condition count by sex  
- **Histograms**: Age distribution with/without disease  
- **Pie chart**: Heart condition class balance  
- **Boxplot**: Age spread across condition classes  
- **Heatmap**: Correlation of features

---


