
# 🛍️ Customer Segmentation in Retail — ML Project

Developed a Machine learning pipeline for customer segmentation on the **H&M dataset** (31M+ transactions, 1.37M customers). Benchmarks 4 clustering algorithms with a custom advanced 4-layer feature engineering approach that goes beyond traditional RFM, to identify actionable customer segments.

## 📁 Notebooks

| Notebook | Description |
|----------|-------------|
| `ML01_preprocessing_features` | Data cleaning + 4-layer feature engineering |
| `ML02_clustering` | K-Means, DBSCAN, GMM, Agglomerative Clustering |
| `ML03_evaluation_visualization` | Metrics, PCA/t-SNE plots, ANOVA, heatmaps |

## 🧠 Approach

- **Layer 1 — RFM:** Recency, frequency, monetary value  
- **Layer 2 — Temporal:** Purchase trend slope, inter-purchase gap  
- **Layer 3 — Product affinity:** Category, colour, department diversity  
- **Layer 4 — Loyalty:** Unique articles, repeat purchase rate  

## 🏆 Results

**K-Means (K=5)** won across all metrics → 5 segments: Champions, Loyal Customers, Non-Member High Spenders, At-Risk Customers, Inactive Customers.

All 12 features validated via one-way ANOVA (p < 0.05).
