# 📊 Customer Churn Prediction with PySpark🎯📁📌

Welcome to the Churn Prediction project! This repository presents a complete, hands-on machine learning pipeline developed using **PySpark** to predict customer churn with high accuracy. The project demonstrates how to optimize classification decisions using a **custom threshold** and export actionable insights that could be used directly by business teams to reduce churn and improve retention.

---

## 🚀 Project Overview

* **Goal:** Predict which customers are likely to churn and generate a prioritized list for business action
* **Dataset:** Telecom customer churn dataset (or your specified dataset)
* **Tools & Libraries:** PySpark, Spark MLlib, matplotlib, scikit-learn, pandas, seaborn
* **Scope:** Covers end-to-end workflow from data cleaning to model evaluation and actionable prediction export

---

## 🧠 ML Pipeline Stages

1. **Data Preprocessing:**

   * Imputed and handled missing values appropriately
   * Encoded categorical features using StringIndexer and OneHotEncoder
   * Assembled numeric and encoded categorical features into a single dense feature vector

2. **Model Building:**

   * Trained a Random Forest Classifier using PySpark MLlib
   * Tuned hyperparameters to balance model complexity and generalization

3. **Evaluation Metrics:**

   * ROC AUC Score for classifier performance
   * Precision, Recall, and F1 Score to evaluate classification quality
   * Interpretation of the PR-F1 tradeoff for threshold optimization

4. **Threshold Tuning:**

   * Computed precision, recall, and F1 score across a range of thresholds (0.0 to 1.0)
   * Identified and applied a custom threshold (`0.295`) that maximized the F1 score, ensuring a balance between precision and recall

5. **Prediction and Export:**

   * Applied the optimal threshold to classify customers as high or low churn risk
   * Filtered high-risk predictions and exported results to a CSV file for downstream use
   * Each output includes the customer ID and churn probability

---

## 📈 Visualizations

* **ROC Curve**: Evaluates the model's ability to distinguish churners vs non-churners
* **Precision-Recall Curve**: Illustrates trade-off between precision and recall across thresholds
* **F1 Score Curve**: Helps determine the ideal threshold that optimally balances model precision and recall
* **Confusion Matrix**: Summarizes true vs predicted classes to evaluate classification correctness
* **Threshold Curves**: Precision, recall, and F1 trends plotted across all threshold values to guide business decision-making

---

## 📤 Output

* **predicted\_churners\_custom\_threshold.csv**

  * Contains customers identified as high churn risk using a threshold of 0.295
  * Columns include: `customerID`, `churn_prob`, and `custom_prediction`
  * Intended to be used directly by business analysts, marketers, or retention teams

---

## ✅ Summary

This project demonstrates a full cycle of predictive modeling in PySpark:

* Importing, cleaning, and transforming raw data
* Engineering features for machine learning models
* Training and evaluating a classifier on real-world data
* Applying a custom threshold based on F1 optimization
* Producing a filtered output suitable for real-world action

Ideal for showcasing applied machine learning knowledge in portfolios, interviews, or academic reports.

---

## 🧑‍💻 Author

**Vijay Kumar Geesala**
Master of Data Science, University of North Texas
GitHub: [vjkumargeesala](https://github.com/vjkumargeesala)

---

## 📬 Contact

If you'd like help with this repo, need support understanding the pipeline, or want to collaborate on ML projects:
📧 [vjkumargeesala@gmail.com](mailto:vjkumargeesala@gmail.com)
