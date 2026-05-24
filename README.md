# 🛒 CartPredict: E-Commerce User Behavior & Model Comparison

This repository contains the code, dataset, and documentation for **CartPredict**, a Data Science Mini-Project. The project focuses on analyzing e-commerce user interactions to predict purchase intent, with a strong emphasis on **comparing multiple machine learning algorithms** to identify the most accurate and efficient predictive model.

---

## 📌 Project Overview
The project goes beyond basic prediction by conducting a comparative study of different classification algorithms. The primary objective is to evaluate which machine learning model works best for predicting whether a browsing session will result in an "purchase" action based on underlying behavioral metrics.

* **Domain:** E-Commerce / User Analytics
* **Objective:** To perform Exploratory Data Analysis (EDA) on user sessions and systematically train, evaluate, and compare multiple classification models to find the optimal solution.

---

## 🗂️ Dataset Details
* **File:** `user_behaviour.csv`
* **Description:** The dataset contains User Behaviour data with 455,401 observations across 25 features. 
* **Target Variable:** The binary outcome of whether the user ordered (`1` for Yes, `0` for No).

---

## 🛠️ Tech Stack & Tools
* **Language:** Python
* **Data Manipulation:** Pandas, NumPy
* **Data Visualization:** Matplotlib, Seaborn
* **Machine Learning:** Scikit-Learn 
* **Environment:** Jupyter Notebook (`CartPredict.ipynb`)

---

## ⚙️ Methodology & Pipeline

1. **Data Preprocessing & Cleaning:** * Handled missing values and standardized numerical features for model compatibility.
2. **Exploratory Data Analysis (EDA):** * Visualized session durations and conducted correlation analysis to identify key purchasing indicators.
3. **Model Development & Comparison:** * Split the dataset into training and testing sets.
   * Trained multiple classification algorithms (Logistic Regression, KNN, Random Forest, XGBoost) to benchmark their predictive capabilities against each other.
4. **Evaluation:** * Assessed and compared each model's performance using metrics including Accuracy, Precision, Recall, and the F1-Score to determine the superior algorithm.

---

## 📈 Key Results & Insights
* **Best Performing Model:** After comparing the algorithms, the **Logistic Regression** outperformed the rest, achieving the highest F1-Score (0.46) and accuracy of 93% on the testing data.
* **Behavioral Drivers:** Feature importance analysis revealed that **basket_add_detail and basket_icon_click** were the strongest indicators of user conversion.
* **Linearity of Purchase Intent:** Contrary to initial expectations that complex ensemble models like XGBoost would dominate, Logistic Regression emerged as the most balanced model. This suggests that in the analyzed e-commerce environment, purchase intent is driven by a linear accumulation of specific actions (such as basket_add_details and basket_icon_click) rather than highly complex, non-linear interactions.
