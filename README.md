# 🚢 Clustering Marine Training Customers  
**K-Means from Scratch on ARFM Profiles (Age, Recency, Frequency, Monetary)**  
_Banten Merchant Marine Polytechnic | Cadet & Alumni Profiles Analysis_

## 📌 Project Overview

This project clusters customer profiles of cadets and alumni from **Banten Merchant Marine Polytechnic** based on their training transaction history. By applying the **ARFM method (Age, Recency, Frequency, Monetary)** and clustering them using a **K-Means algorithm built from scratch**, we aim to identify behavioral patterns and segment customers for better strategic decisions.

### 🎯 Objectives:
- Segment customers based on ARFM profiles
- Discover patterns of training behavior
- Provide actionable insights for targeted communication and loyalty programs

---

## 📊 Dataset Description

- **Source**: `customer_profiles.xlsx`  
- **Entries**: 2,300+ customer transactions  
- **Fields**:
  - `NRT/Kode Pelaut` (Customer ID)
  - `Tanggal Lahir` (Date of Birth)
  - `Tanggal Transaksi` (Transaction Date)
  - `Diklat` (Training Type)
  - `Nominal Transaksi` (Transaction Amount)

---

## 🧠 Feature Engineering

We derived 4 key features for clustering:

- **Age**: Age at the time of transaction  
- **Recency**: Days since last transaction  
- **Frequency**: Total number of transactions  
- **Monetary**: Total amount spent

These features were standardized and outliers were removed prior to clustering.

---

## 🛠️ Clustering Method

- **Algorithm**: K-Means (custom implementation from scratch using NumPy)  
- **Distance Metric**: Euclidean Distance  
- **Evaluation Metric**: Davies-Bouldin Index (Best score: **K = 3**)

---

## 🧩 Cluster Insights

| Cluster | Label     | Age (avg) | Recency (avg) | Frequency | Monetary (avg) |
|--------|------------|------------|----------------|------------|----------------|
| 0      | 🥇 Platinum | 24         | 73 days        | 4 times    | Rp 4.68M       |
| 1      | 🥈 Gold     | 23         | 95 days        | 3 times    | Rp 3.19M       |
| 2      | 🥉 Silver   | 24         | 59 days        | 5 times    | Rp 6.12M       |

- **Platinum**: High spenders, moderately frequent  
- **Gold**: Medium spenders with loyal patterns  
- **Silver**: High-frequency, high-spending, relatively recent

---

## 📢 Recommendations

1. **Personalized Communication**  
   Prioritize Cluster 0 and 2 for engagement and upsell strategies.

2. **Loyalty Program**  
   Reward Cluster 1 customers to increase lifetime value and retention.

3. **Cross-Selling Opportunities**  
   Use training packages or bundles to encourage Cluster 1 & 2 growth.

4. **Continuous Monitoring**  
   Run clustering periodically to adapt to behavioral shifts.

---

## 📦 Tech Stack

- Python (Pandas, NumPy, Seaborn, Plotly)
- Scikit-learn for validation metrics (Davies-Bouldin)
- Custom K-Means algorithm (no external ML libraries)

---

## ✍️ Author

**Alexander Tiopan**  
_Senior Business Analyst | Data Enthusiast | Customer Behavior Explorer_  
📧 alexandertiopan1212@gmail.com  
📂 Repository: [Clustering_Training_Customer](https://github.com/alexandertiopan1212/Clustering_Training_Customer)

