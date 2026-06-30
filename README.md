# E-Commerce-Sales-Analytics-Predictive-Model
E-Commerce Sales Analytics &amp; Predictive Modeling
An end-to-end data science project exploring 5,000 transaction records to identify revenue drivers, test business operational hypotheses, and construct a machine learning model to predict customer satisfaction metrics.

## 📊 Key Business Insights
**Revenue Powerhouse:** Electronics emerged as the primary revenue generator (~$1.8M), while the Beauty vertical significantly lagged (~$0.75M).
**Operations Myth Dispelled:** Statistical analysis proved a near-zero correlation (`-0.017`) between logistics duration (delivery days) and customer ratings, shifting strategic focus away from forcing high-cost 1-day shipping.
**Payment Trends:** Card payments dominate universally (~600 orders/region). Digital wallets are heavily underutilized (<250 orders/region), leading to a strategic recommendation for targeted digital wallet promotional incentives to mitigate Cash on Delivery (COD) risks.

## 🤖 Machine Learning Pipeline & Optimization
A **Random Forest Classifier** was trained to predict high vs. low customer satisfaction. 
**Iteration 1 (Baseline):** Suffered from severe class imbalance, causing an accuracy trap of 71% but a failure to capture high ratings (Class 1 Recall: 2%).
**Iteration 2 (Optimized):** Implemented custom feature engineering (`discount_percentage`, `price_per_item`) and tuned hyperparameters (`max_depth=8`, `class_weight='balanced'`). This successfully broke model bias, driving Target Class Recall up to **27%** with a realistic, deployment-ready overall accuracy of **61%**.

## 🚀 How to Run the Project
1. Clone this repository:
   ```bash
   git clone [https://github.com/YOUR_USERNAME/ecommerce-sales-analytics.git](https://github.com/YOUR_USERNAME/ecommerce-sales-analytics.git)
