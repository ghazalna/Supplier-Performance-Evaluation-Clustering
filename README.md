# Supplier-Performance-Evaluation-Clustering
This project aims to evaluate and segment supplier performance using real-world inventory data. By analyzing delivery metrics and stock behavior, we apply unsupervised machine learning to group suppliers into meaningful performance categories. This helps supply chain analysts quickly identify high-performing suppliers and those that may pose risks.
# 📦 Supplier Performance Evaluation & Clustering

## 📊 Dataset Description
This project uses a real-world inventory monitoring dataset containing:

- **Product ID** – unique identifier (used as a proxy for supplier)
- **Supplier Lead Time (days)** – time required for delivery
- **Stockout Frequency** – how often a product runs out of stock
- **Order Fulfillment Time (days)** – average order processing duration
- **Warehouse Capacity** – available space per item
- **Stock Levels** – average amount of inventory held
- **Reorder Point** – the threshold to trigger a replenishment

Since the dataset does not contain actual supplier IDs, we assume that each `Product ID` is sourced from a unique supplier.

---

## 🎯 Project Goals

- Evaluate supplier performance using key operational metrics
- Cluster suppliers based on performance similarities
- Identify low-performing and high-performing supplier groups
- Communicate insights visually for business decision-makers

---

## 🧠 Key Performance Indicators (KPIs)

These KPIs are used to evaluate and compare supplier behavior:

| KPI                    | Description                                                  |
|------------------------|--------------------------------------------------------------|
| **Avg Lead Time**      | Average number of days it takes a supplier to deliver        |
| **Stockout Frequency** | How often the product runs out of stock                      |
| **Fulfillment Time**   | Days required to fulfill an order after it's placed          |
| **Avg Warehouse Cap**  | Average warehouse space allocated for that product           |
| **Avg Stock**          | Average inventory level for the product                      |

These KPIs help identify patterns and performance levels among suppliers.  
For example, low lead time and stockout frequency typically signal a reliable supplier.

---

## 🛠️ Methods Used

- **Exploratory Data Analysis (EDA)** – to understand distributions and relationships
- **Feature Engineering** – aggregated KPIs per supplier (via Product ID)
- **Standardization** – data normalization using `StandardScaler`
- **K-Means Clustering** – to segment suppliers
- **Silhouette Score** – to find the optimal number of clusters
- **Visualization** – histograms, boxplots, barplots, and heatmaps

---

## 💡 Why Use Clustering?

Clustering groups suppliers based on actual performance data instead of arbitrary thresholds. It helps businesses:
- Find hidden performance patterns
- Spot high-risk suppliers early
- Make data-driven sourcing and planning decisions
- Save time by summarizing thousands of rows into meaningful categories

---

## 📈 Results Summary

We applied K-Means clustering and found **3 distinct clusters**:

- **Cluster 1 – High-Performing Suppliers**  
  ✅ Fast lead times  
  ✅ Quick order fulfillment  
  ✅ Low stockout risk

- **Cluster 0 – Average Suppliers**  
  📊 Balanced performance with room for improvement

- **Cluster 2 – High-Risk Suppliers**  
  ❌ Long lead times  
  ❌ High stockout frequency  
  ❌ Slower fulfillment time

We visualized the differences using barplots, boxplots, and correlation heatmaps.

---

## ✅ Business Benefits

- Helps supply chain teams track and improve supplier efficiency
- Supports supplier negotiations with data-driven insights
- Improves inventory control and replenishment planning
- Enables better risk assessment and procurement strategy

---

## 📁 Project Structure

```
/Supplier_Performance_Clustering
│
├── supplier_analysis.ipynb       # Main analysis notebook
├── data/                         # Cleaned dataset
├── visuals/                      # Charts and graphics
├── models/                       # (Optional) saved clustering model
└── README.md                     # Project overview
```



---

## 📬 Contact

Have questions or suggestions?  
Feel free to open an issue or contact me on GitHub.

---

> ✅ This project highlights applied data science skills in the context of supply chain performance monitoring and business optimization.
