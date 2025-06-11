

![image](https://github.com/user-attachments/assets/d48757d2-edb3-4e59-a9d3-68dd7037e646)

# 💳 Credit Card Fraud Detection using Logistic Regression

This project implements a **Logistic Regression** model to detect fraudulent credit card transactions from an imbalanced dataset. It addresses the challenge of **class imbalance**—where fraud cases are significantly fewer than legitimate ones—by applying **under-sampling** to the majority class before training.

---

## 📂 Dataset

* **Source:** [Kaggle – Credit Card Fraud Detection](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
* **Samples:** 284,807 transactions
* **Fraudulent Transactions:** \~0.17%
* **Features:** 28 anonymized PCA features (`V1`–`V28`), along with `Time`, `Amount`, and `Class` (target)

---

## 🎯 Project Goals

* Perform exploratory data analysis (EDA) and preprocessing
* Address class imbalance using **under-sampling** (reducing majority class)
* Train and evaluate a **Logistic Regression** model
* Use classification metrics appropriate for imbalanced data

---

## 🛠️ Technologies Used

* Python
* Pandas, NumPy
* Scikit-learn
* Matplotlib, Seaborn

---

## 🔍 Workflow Summary

1. **Exploratory Data Analysis (EDA):**

   * Analyzed feature distributions and class imbalance
   * Checked for null or missing values

2. **Preprocessing:**

   * Scaled `Amount` and `Time` features
   * Applied **under-sampling** to balance classes by reducing normal transactions

3. **Modeling:**

   * Trained a **Logistic Regression** model on the under-sampled data

4. **Evaluation:**

   * Evaluated using **Confusion Matrix**, **Precision**, **Recall**, **F1 Score**, and **ROC AUC**
   * Plotted ROC Curve to visualize performance

---

## 📊 Evaluation Metrics

| Metric        | Description                                          |
| ------------- | ---------------------------------------------------- |
| **Accuracy**  | Overall correctness (not ideal for imbalance)        |
| **Precision** | Correct fraud predictions out of all predicted fraud |
| **Recall**    | Ability to detect actual frauds (very important)     |
| **F1 Score**  | Balance between Precision and Recall                 |
| **ROC AUC**   | Model’s ability to distinguish between classes       |

---

## ✅ Results

After applying under-sampling, the Logistic Regression model showed significant improvement in detecting fraudulent transactions, especially in terms of **recall** and **F1 score**. This demonstrates that even simple models, when paired with the right sampling strategy, can perform effectively on real-world imbalanced datasets.

---

## 📌 Conclusion

This project illustrates the effectiveness of **Logistic Regression** when combined with **under-sampling** for fraud detection. It highlights the importance of choosing the right evaluation metrics and handling class imbalance carefully to build reliable and interpretable financial security systems.

