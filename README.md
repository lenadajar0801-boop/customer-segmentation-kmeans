# Customer Segmentation using KMeans Clustering

## Project Overview

This project focuses on segmenting customers based on their purchasing behavior using unsupervised machine learning. It utilizes the Mall Customers dataset to group customers into distinct segments based on their annual income and spending score.

Customer segmentation is widely used in business and marketing to better understand customer behavior and improve targeting strategies.

---

## Objective

To apply KMeans clustering to group customers into meaningful segments based on their income and spending patterns, and to generate actionable business insights.

---

## Dataset

Source: https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial  

Dataset Used:
- Mall_Customers.csv  

Dataset characteristics:

- Contains 200 customer records  
- Includes demographic and behavioral features  
- Features:
  - Gender (categorical)  
  - Age  
  - Annual Income (k$)  
  - Spending Score (1–100)  

- No target variable (unsupervised learning)

---

## Tools & Technologies

- Python  
- Pandas, NumPy  
- Scikit-learn  
- Matplotlib, Seaborn  
- Jupyter Notebook  

---

## Data Preprocessing

### Steps Performed

- Renamed column `Genre` to `Gender`  
- Removed `CustomerID` as it is not relevant for clustering  
- Selected key features:
  - Annual Income (k$)  
  - Spending Score (1–100)  
- Applied StandardScaler for feature scaling  

### Explanation

Feature scaling is necessary because KMeans is a distance-based algorithm. Without scaling, features with larger values would dominate the clustering process.

---

## Model — KMeans Clustering

### Steps Performed

- Applied the Elbow Method to determine the optimal number of clusters  
- Computed WCSS (Within-Cluster Sum of Squares) for K = 1 to 10  
- Plotted K vs WCSS  
- Identified the elbow point  

### Results

Optimal number of clusters:

- K = 5  

---

## Elbow Method

- WCSS measures how compact the clusters are  
- As K increases, WCSS decreases  
- The optimal K is where the decrease starts to slow down  

This point is known as the “elbow” and represents the best balance between simplicity and performance.

---

## Customer Segmentation Results

Customers were grouped into 5 distinct clusters:

### Cluster 1 — Average Customers
- Medium income  
- Medium spending  
- Regular customers with stable behavior  

---

### Cluster 2 — Premium Customers
- High income  
- High spending  
- Most valuable customers  

---

### Cluster 3 — Impulse Buyers
- Low income  
- High spending  
- High spending despite lower income  

---

### Cluster 4 — Potential Customers
- High income  
- Low spending  
- Can be targeted for increased engagement  

---

### Cluster 5 — Low Value Customers
- Low income  
- Low spending  
- Lowest priority segment  

---

## Visualization

- Scatter plot used to visualize clusters  
- Each cluster represented by a different color  
- Centroids plotted to show cluster centers  

This visualization clearly shows the separation of customer groups.

---

## Key Insights

- Customers can be segmented effectively using income and spending behavior  
- Premium customers represent the highest value  
- Potential customers offer growth opportunities  
- Segmentation helps improve marketing strategies  

---

## Business Value

Customer segmentation helps businesses:

- Improve targeted marketing  
- Increase customer retention  
- Identify high-value customers  
- Optimize business decisions  

---

## Future Improvements

- Include additional features such as Age and Gender  
- Apply other clustering techniques (Hierarchical Clustering)  
- Use PCA for dimensionality reduction  
- Build dashboards using Power BI  

---

## Conclusion

KMeans clustering successfully segmented customers into meaningful groups. The model provides valuable insights that can support business decision-making and targeted marketing strategies.

---

## Author

Allen Adajar  
Cost Accountant | Data Analyst | Aspiring Data Scientist  

GitHub: https://github.com/lenadajar0801-boop  
