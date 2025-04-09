# Clustering Training Customer Profiles

## Project Title
**Clustering Analysis of Marine Training Customer (Banten Merchant Marine Polytechnic Cadet and Alumnus) Profiles Using Age, Recency, Frequency, and Monetary Method with K-Means Algorithms from Scratch**

## Overview
This project analyzes marine training customers using clustering based on Age, Recency, Frequency, and Monetary (ARFM) features. K-Means clustering is implemented from scratch to classify customer behavior and purchasing power.

## Dataset Summary
- **Source**: customer_profiles.xlsx
- **Fields**:
  - NRT/Kode Pelaut: Unique customer identifier
  - Tanggal Lahir: Date of birth
  - Tanggal Transaksi: Transaction date
  - Diklat: Type of training
  - Nominal Transaksi: Transaction value

## ARFM Features
- **Age**: Calculated at the time of each transaction
- **Recency**: Days since the latest transaction
- **Frequency**: Number of training sessions taken
- **Monetary**: Total spending

## Preprocessing
- Converted date fields to datetime
- Calculated Age, Recency, Frequency, and Monetary values
- Removed outliers using z-score filtering

## Clustering
- Implemented KMeans algorithm manually
- Chose optimal number of clusters (3) based on Davies–Bouldin Index (best score: 0.52)
- Cluster results:
  - **Cluster 0 (Platinum)**: High frequency & monetary value, average age 24
  - **Cluster 1 (Gold)**: Moderate frequency & value, slightly younger users
  - **Cluster 2 (Silver)**: Lower frequency & spending, similar age group

## Visual Insights
- Histogram plots of Age, Recency, Frequency, and Monetary for all customers
- Clustering visualization via scatter plot
- Davies–Bouldin Score plotted for 2-4 clusters

## Recommendations
- **Personalized Marketing**: Focus on Platinum and Gold clusters for upselling
- **Loyalty Programs**: Reward most loyal and high-spending customers
- **Skill Development**: Encourage Silver cluster to join more training
- **Monitoring**: Regularly update ARFM metrics to adjust strategies

## Conclusion
This analysis offers actionable customer segmentation using classical ARFM modeling and clustering from scratch. The outcome helps the campus design more targeted and effective engagement strategies.
