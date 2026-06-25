
# 🛍️ Customer Segmentation in Retail — ML Project

Developed a Machine learning pipeline for customer segmentation on the **H&M dataset** (31M+ transactions, 1.37M customers). Benchmarks 4 clustering algorithms with a custom advanced 4-layer feature engineering approach that goes beyond traditional RFM, to identify actionable customer segments.

## 📦 Dataset

**H&M Personalized Fashion Recommendations** (Kaggle, Sept 2018 – Sept 2020)


## ⚙️ Pipeline

Raw Data → Preprocessing → 4-Layer Feature Engineering → Normalisation + PCA → Clustering → Evaluation


## 📁 Notebooks

| Notebook | Description |
|----------|-------------|
| `ML01_preprocessing_features` | Data cleaning + 4-layer feature engineering |
| `ML02_clustering` | K-Means, DBSCAN, GMM, Agglomerative Clustering |
| `ML03_evaluation_visualization` | Metrics, PCA/t-SNE plots, ANOVA, heatmaps |

## 🧠 Approach

- **Layer 1 — RFM:** Recency days, purchase frequency, monetary total  
- **Layer 2 — Temporal:** Purchase trend slope, inter-purchase gap, most active month  
- **Layer 3 — Product affinity:**  Top garment category, preferred colour, department, avg price tier & basket size  
- **Layer 4 — Loyalty:** Unique articles count, repeat purchase rate  

## 🏆 Results

**K-Means (K=5)** won across all metrics → 5 segments: Champions, Loyal Customers, Non-Member High Spenders, At-Risk Customers, Inactive Customers.

All 12 features validated via one-way ANOVA (p < 0.05).
