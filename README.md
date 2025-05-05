# 🛍️ Customer Purchase Prediction

This project predicts whether a customer will purchase a product based on various behavioral and demographic features using different machine learning algorithms.

> 📁 Original notebook: [Problem_Statement_02.ipynb](https://github.com/shreyakmukherjee/Predict-Customer-will-purchase-a-product-or-not-/blob/main/Problem_Statement_02.ipynb)

---

## 📌 Problem Statement

Build a classification model to predict whether a customer will purchase a product, based on:

- Age
- Gender
- Annual Income
- Number of Purchases
- Product Category
- Time Spent on Website
- Loyalty Program Membership
- Discounts Availed

The target variable is:
- **Purchase Status**: `0` (No Purchase), `1` (Purchase)

---

## 📊 Exploratory Data Analysis (EDA)

- No missing values in the dataset.
- Feature distribution visualizations and correlation heatmaps were used to understand key influencing factors.
- Key influential features identified: `Loyalty Program`, `Discounts Availed`, `Time Spent on Website`, and `Annual Income`.

---

## 🧹 Data Preprocessing

- **Scaling**: `StandardScaler` used for normalization.
- **Splitting**: 80% training, 20% testing.

---

## 🤖 Models Used

| Model                  | Accuracy | Precision | Recall | F1 Score |
|-----------------------|----------|-----------|--------|----------|
| Decision Tree         | 89.7%    | 91.5%     | 83.6%  | 87.3%    |
| Logistic Regression   | 83.7%    | 87.6%     | 71.9%  | 78.9%    |
| SVM                   | 87.0%    | 88.7%     | 79.7%  | 84.0%    |
| Naive Bayes           | 83.7%    | 88.3%     | 71.1%  | 78.8%    |
| **Random Forest**     | **95.3%**| **99.1%** | 89.8%  | **94.3%**|

✅ **Random Forest Classifier** performed the best and is recommended for deployment.

---

## 📌 Conclusion

The model successfully identifies customer purchase intent with high accuracy. Behavioral features such as website engagement and loyalty status are strong predictors of purchasing behavior.

---

## 📎 How to Run

```bash
# Clone the repository
git clone https://github.com/shreyakmukherjee/Predict-Customer-will-purchase-a-product-or-not-.git
cd Predict-Customer-will-purchase-a-product-or-not-

# Open the notebook
jupyter notebook Problem_Statement_02.ipynb
