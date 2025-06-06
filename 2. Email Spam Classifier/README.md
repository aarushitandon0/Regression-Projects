# Spam Detection Using Logistic Regression (from scratch)

This project implements a **binary classifier** to detect spam emails using **Logistic Regression**, built completely from **scratch** using NumPy — without relying on machine learning libraries like `scikit-learn` for training.

---

## Dataset

Used the **Spambase Dataset** from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/spambase), which contains:

- **57 numerical features**, including:
  - Word frequencies (e.g., `word_freq_make`, `word_freq_address`)
  - Character frequencies (e.g., `char_freq_;`, `char_freq_!`)
  - Capital letter statistics (`capital_run_length_average`, etc.)
- **Target column**:  
  - `1` = spam  
  - `0` = not spam

---

## Technologies Used

| Tool | Purpose |
|------|---------|
| **Python** | Core language |
| **NumPy** | Model implementation + math ops |
| **Pandas** | Data loading & preprocessing |
| **scikit-learn** | ONLY used for `train_test_split` |
| **Jupyter Notebook** | Development & experimentation |

---

## Project Pipeline

### 1. Data Loading & Preprocessing
- Loaded data into a Pandas DataFrame
- Scaled features using **min-max normalization**
- Split dataset: **80% training**, **20% testing**

### 2. Model Implementation
- Logistic Regression built manually using NumPy
- Used **Sigmoid activation** function
- Optimized using **Gradient Descent**  
- Cost function: **Binary Cross-Entropy Loss**
- Trained for **2000 epochs**, with **learning rate = 2.7**

### 3. Evaluation
- Made predictions on the test set
- Calculated **accuracy score**

---

## Results

Achieved a **Test Accuracy of ~90.12%**, indicating strong classification performance on the dataset.

---


