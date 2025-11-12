# 🧠 Customer Lifetime Value (CLV) Prediction

**Author:** Kondagurla Parshi  
**Tools:** Python, Pandas, NumPy, Scikit-learn, XGBoost, Matplotlib, Seaborn, Google Colab  
**Goal:** Predict Customer Lifetime Value (CLV) to identify high-value customers and help businesses improve retention strategies.

---

## 🚀 Project Overview
This project estimates how much revenue a customer will generate in the future using **transaction-level retail data**.  
It uses **RFM features (Recency, Frequency, Monetary)** and regression models to predict customer value.

---

## 🧩 Workflow
1. **Data Cleaning:** Removed null values, invalid quantities, and formatted dates  
2. **Feature Engineering:** Derived RFM + AvgOrderValue + AvgQtyPerOrder  
3. **Exploratory Data Analysis (EDA):** Visualized spending patterns and relationships  
4. **Model Building:** Trained Linear Regression, Random Forest, and XGBoost models  
5. **Evaluation:** Compared models using R², MAE, RMSE  
6. **Insights:** Identified key value drivers and top 10 customers by predicted CLV

---

## 📊 Results
| Model | R² Score | MAE | RMSE |
|--------|-----------|------|-------|
| Linear Regression | ~0.78 | ~400 | ~600 |
| Random Forest | **~0.89** | **~280** | **~510** |
| XGBoost | ~0.90 | ~260 | ~500 |

🔹 **Best Model:** Random Forest  
🔹 **Key Drivers:** Frequency, AvgOrderValue, Recency  
🔹 **Business Insight:** Top 20% of customers generate ~65% of total revenue.

---

## 📂 Project Structure
📂 Project Structure
clv-prediction/
├── notebooks/
│   └── 01_clv_model.ipynb
├── reports/
│   ├── figures/
│   │   ├── clv_distribution.png
│   │   ├── actual_vs_pred.png
│   │   └── feature_importance.png
│   └── top_customers.csv
├── data/
│   └── OnlineRetail.csv
└── README.md

