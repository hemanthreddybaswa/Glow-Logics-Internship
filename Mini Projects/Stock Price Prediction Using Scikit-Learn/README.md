
---

# Stock Price Prediction using Machine Learning (Scikit-Learn)

This project demonstrates how **Machine Learning** can be used to analyze historical stock market data and predict **buy/sell signals** using classical ML algorithms implemented with **Scikit-Learn**.

The primary goal of this project is to strengthen understanding of the **end-to-end supervised learning workflow**, including data preprocessing, feature engineering, model training, evaluation, and interpretation.

> 

---

## Project Overview

* **Domain:** Financial Data Analysis / Machine Learning
* **Type:** Supervised Learning (Classification)
* **Framework:** Scikit-Learn
* **Dataset:** Tesla stock historical data (2010 – 2017)

This project predicts whether **buying a stock at a given time is beneficial or not** based on engineered price-movement features.

---

##  Machine Learning Workflow

1. Data Collection
2. Data Cleaning & Preprocessing
3. Feature Engineering
4. Exploratory Data Analysis (EDA)
5. Model Training (Scikit-Learn)
6. Model Evaluation
7. Result Interpretation



---

##  Dataset Description

* **Stock:** Tesla (TSLA)
* **Time Period:** 2010 – 31 December 2017
* **Rows:** 1692
* **Features:**

  * Open
  * High
  * Low
  * Close
  * Adj Close
  * Volume

 Non-trading days (weekends & holidays) are naturally excluded.

---

##  Feature Engineering

To convert raw stock prices into a machine-learning-friendly format, new features were created:

* **Open-Close Difference**
* **Low-High Difference**
* **Binary Target Label** indicating:

  * `1` → Buying is beneficial
  * `0` → Buying is not beneficial

This transforms the problem into a **binary classification task**.

---

## Exploratory Data Analysis (EDA)

EDA was performed to understand:

* Price trends over time
* Volatility patterns
* Feature distributions
* Correlation between engineered features and target labels

Visualizations helped identify meaningful patterns and validate feature choices.

---

##  Models Used (Scikit-Learn)

The following ML models were trained and evaluated:

* **Logistic Regression**
* **Support Vector Classifier (SVC)**
* **XGBoost Classifier**

Each model was tested using the same train-test split to ensure fair comparison.

---

## Model Evaluation Metrics

Models were evaluated using:

* Accuracy Score
* Confusion Matrix
* Classification Report

Due to the nature of stock data, accuracy alone is **not sufficient**, and results were interpreted carefully.

---

## Results & Observations

* Classical ML models can capture **short-term market signals**
* Feature engineering plays a **critical role**
* Financial data is noisy → perfect prediction is unrealistic
* ML is better used as a **decision-support tool**, not a decision maker

---

##  Tech Stack

* **Programming Language:** Python
* **Libraries:**

  * NumPy
  * Pandas
  * Matplotlib
  * Seaborn
  * Scikit-Learn
  * XGBoost

---

##  Project Structure

```
Stock-Price-Prediction-ScikitLearn
|-Stock_Price_Prediction.ipynb
|-README.md
```