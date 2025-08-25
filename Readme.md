# 🛒 Customer Segmentation with K-Means and DBSCAN

This project applies **unsupervised machine learning** to the [Mall Customers dataset](https://www.kaggle.com/datasets/shwetabh123/mall-customers) to identify distinct customer groups.  
I used **K-Means** as the main clustering algorithm and compare it to **DBSCAN** as part of a bonus analysis.

---

## 📊 Project Overview
Customer segmentation helps businesses:
- Understand **different types of customers** based on spending behavior and income.  
- Target marketing campaigns more effectively.  
- Improve personalization and retention strategies.  

In this project, we:
1. Preprocess the dataset.  
2. Apply **K-Means clustering** to segment customers.  
3. Analyze **average spending per cluster**.  
4. Test **DBSCAN** as an alternative clustering algorithm.  
5. Visualize and interpret the results.  

---

## ⚙️ Technologies Used
- Python (core)
- Libraries: `pandas`, `numpy`, `matplotlib`, `scikit-learn` , `plotly.express`

---

## 📂 Files in this Repository
- `Project2_CustomerSegmentation.ipynb` → Jupyter notebook with full analysis and visualizations.  
- `Mall_Customers.csv` → Dataset (if included).  
- `README.md` → Project documentation.  

---

## 🚀 How to Run
1. Clone the repository or download it.  
2. Install dependencies:
   ```bash
   pip install pandas numpy matplotlib scikit-learn
## 🔎 Results & Interpretation
### K-Means Clustering
- **Cluster 0** → Medium income, medium spending → *Balanced customers*.  
- **Cluster 1** → High income, high spending → *VIP / high-value customers*.  
- **Cluster 2** → Low income, high spending → *Deal-seekers (spend despite lower income)*.  
- **Cluster 3** → High income, low spending → *Potential customers (need incentives)*.  
- **Cluster 4** → Low income, low spending → *Low-value customers*.  

📌 **Business takeaway:**  
- Focus marketing on **Clusters 1 & 2** (highest spending).  
- Use incentives for **Cluster 3** (rich but not spending).  
- Deprioritize **Cluster 4**.  

---

### 📊 Average Spending per Cluster
- Bar chart analysis shows that **Clusters 1 and 2** have the highest spending scores.  
- These clusters are prime targets for marketing campaigns.  

---

### 🧩 DBSCAN (Bonus)
- DBSCAN found fewer clusters and labeled some customers as **noise (-1)**.  
- Results were less interpretable compared to K-Means.  
- **Conclusion:** For this dataset, **K-Means is better** because it produces clean, business-friendly clusters.  

---

### 📈 Visualizations
- Scatter plots → Clusters by **Income vs Spending**.  
- Bar charts → **Average spending per cluster**.  
- Comparison → **K-Means vs DBSCAN results**.  

---

### ✅ Conclusion
- **K-Means** gave 5 well-defined customer groups with clear business meaning.  
- **DBSCAN** was less effective for this dataset.  
- Businesses can use these insights to:  
  - Focus campaigns.  
  - Personalize offers.  
  - Allocate budgets efficiently.  