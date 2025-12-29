# 🎬 Customer Churn Prediction for a Subscription-Based Streaming Platform

## 📌 Project Overview
Customer churn is one of the most critical challenges for subscription-based businesses, especially in highly competitive digital streaming platforms. This project focuses on building a **data-driven machine learning solution** to predict customer churn and uncover actionable business insights that can help improve customer retention.

Using customer behavioral and subscription data, this project explores patterns of user engagement, develops predictive models, and translates model outputs into meaningful business recommendations.

---

## 🎯 Objectives

### Primary Objective
- Build a machine learning model to **predict customer churn early**, enabling proactive retention strategies.

### Secondary Objectives
- Identify key behavioral and customer-related factors influencing churn.
- Analyze the relationship between user engagement and churn risk.
- Provide actionable insights to support business decision-making.

### Business Value
- Support **proactive retention strategies** instead of reactive churn handling.
- Reduce potential revenue loss caused by customer churn.
- Improve the effectiveness of customer engagement and retention programs.

---

## 📂 Dataset Description

The dataset represents customer behavior on a **subscription-based video streaming platform**.

**Dataset Summary:**
- Total records: ~5,000 customers
- Total features: 14 behavioral & customer attributes
- Target variable: `churned`
  - `1` → Churned customer
  - `0` → Active customer

**Key Feature Groups:**
- User engagement (watch hours, average watch time, last login days)
- Subscription details (subscription type, monthly fee)
- Account characteristics (number of profiles)
- Payment method and demographics

---

## 🔍 Exploratory Data Analysis (EDA)

Key insights from EDA include:
- Churn is a **non-trivial and significant issue**, not a rare event.
- Churned users show:
  - Lower watch hours and average daily engagement
  - Longer inactivity periods since last login
- Basic subscription users have higher churn rates than premium tiers.
- Users with less conventional payment methods (e.g., gift cards, crypto) exhibit higher churn.

These insights highlight that **user engagement behavior is the strongest signal of churn risk**.

---

## 🤖 Modeling Approach

Two models were developed and evaluated:

### 1. Baseline Model
- **Logistic Regression**
- Used as a benchmark for interpretability and baseline performance.

### 2. Advanced Model
- **Random Forest Classifier**
- Chosen to capture non-linear relationships in user behavior.

**Evaluation Metrics:**
- Accuracy
- Precision
- Recall
- F1-score
- ROC Curve & AUC

---

## 📊 Model Performance

- The **Random Forest model outperformed Logistic Regression** across all evaluation metrics.
- It demonstrated stronger capability in capturing complex behavioral patterns.
- ROC Curve analysis shows excellent separability with an **AUC score of 1.00**.

📌 **Final Model Selected:** Random Forest Classifier

---

## 🔎 Model Interpretability

Feature importance analysis reveals:

- **User engagement is the primary driver of churn**
  - Most influential features:
    - `avg_watch_time_per_day`
    - `watch_hours`
    - `last_login_days`
- Accounts with multiple profiles tend to be more engaged and less likely to churn.
- Demographic and pricing-related features (age, monthly fee, subscription type) have relatively low impact.

💡 **Key Insight:**  
Churn is driven more by **behavioral patterns** than by pricing or demographics.

---

## 💼 Business Recommendations

1. **Strengthen User Engagement Programs**  
   Enhance personalized content recommendations and content discovery features to increase daily watch time.

2. **Early Intervention for Inactive Users**  
   Identify users with increasing inactivity and trigger re-engagement actions (notifications, emails, exclusive content).

3. **Promote Multi-Profile Usage**  
   Encourage users to create multiple profiles to increase household-level engagement.

4. **Prioritize Behavioral Signals Over Pricing Changes**  
   Focus retention efforts on improving user experience and engagement rather than relying heavily on discounts.

---

## 📘 What I Learned

- Customer churn can be detected **before revenue loss occurs** using behavioral data.
- Engagement metrics are far more predictive than demographics or pricing.
- Random Forest models are effective for capturing complex user behavior patterns.
- Translating machine learning results into business insights is as important as model accuracy.
- A strong data science project connects **data → model → insight → business action**.

---

## 🛠️ Tech Stack
- Python
- Pandas & NumPy
- Matplotlib & Seaborn
- Scikit-learn
- Jupyter / Google Colab

---

## 🚀 Author
**Sandy Sanjaya**  
Junior Data Scientist | Data & Machine Learning Enthusiast  

📌 Feel free to connect with me on **LinkedIn** and explore more projects on my **GitHub**.
