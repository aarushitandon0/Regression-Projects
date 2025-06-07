# House Price Prediction – Linear Regression from Scratch

## Project Objective

Build a simple yet powerful regression model to predict the **price of a house** based on its **area (in sq.ft)** using:

- Gradient Descent (custom implementation)
- Min-Max Feature Scaling
- Custom visualizations (loss curve, prediction plot)

This project was implemented **from scratch** using only NumPy and basic Python — no pre-built ML models.

---

## Built With

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge&logo=matplotlib&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)

> ⚠️ **Note**: scikit-learn is *only* used for splitting the data (train_test_split).

---

## Dataset

The dataset is a small CSV file with **50 rows**, containing the following columns:

| Area (sq.ft) | Price (₹)     |
|--------------|---------------|
| 1260         | 8,220,000     |
| 1694         | 12,805,000    |
| 1530         | 11,001,000    |
| ...          | ...           |

This minimal dataset was ideal for quickly iterating and observing how a custom regression model behaves during training.

---

## Output Highlights

- Learned slope (`w`) and intercept (`b`) using gradient descent (parameters w and b)
- Plotted predicted line vs actual points  
- Tracked loss reduction over iterations  





