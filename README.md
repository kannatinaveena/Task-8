# 🧠 K-Means Clustering - Customer Segmentation

## 📌 Project Overview

This project applies **K-Means Clustering**, an unsupervised machine learning algorithm, to segment mall customers based on their features such as **Age**, **Annual Income**, and **Spending Score**. The goal is to group similar customers into distinct clusters to enable targeted marketing and business insights.

✅ **Internship Task 8**  
🎯 **Objective:** Perform clustering using K-Means and evaluate the results using visualization and metrics.

---

## 🛠️ Tools & Libraries Used

- Python 🐍
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn

---

## 📁 Dataset

**Dataset Name:** Mall Customer Segmentation Dataset  
**Source:** [Kaggle Dataset](https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python)  
**Features Used:**

- `Age`
- `Annual Income (k$)`
- `Spending Score (1-100)`

---

## 🧪 What and Why (Steps with Explanation)

### ✅ 1. Load & Explore Dataset
We read the dataset using Pandas and explore its structure using `.head()`, `.info()`, and `.describe()`.  
**Why?** Understand the data types, missing values, and overall shape of the dataset.

---

### ✅ 2. Feature Scaling
Used `StandardScaler` to scale features.  
**Why?** K-Means is sensitive to feature scale. Without scaling, income (in thousands) can dominate the clustering.

---

### ✅ 3. Fit K-Means with Assumed K = 5
Fitted K-Means with 5 clusters and added the cluster labels to the DataFrame.  
**Why?** This allows us to analyze clusters and check if customer segments are meaningful.

---

### ✅ 4. Use the Elbow Method
Plotted **inertia vs. K** for K = 1 to 10.  
**Why?** Helps choose the best K using the "elbow" point where adding more clusters doesn’t improve WSS much.

---

### ✅ 5. Visualize Clusters (PCA)
Used **Principal Component Analysis (PCA)** to reduce features to 2D and visualized with color-coded clusters.  
**Why?** Easier to interpret clusters visually in 2D.

---

### ✅ 6. Evaluate Clustering with Silhouette Score
Computed Silhouette Score for K = 5 and other values.  
**Why?** Measures how similar a point is to its own cluster compared to other clusters. Higher score = better separation.

---

### ✅ 7. Plot Cluster Centers
Inverse transformed scaled cluster centers to original scale and plotted.  
**Why?** Shows average customer profile for each cluster.

---

### ✅ 8. Export Results (Optional)
Saved clustered data to `clustered_customers.csv` for later use.

---

## 📊 Visualizations

- **Elbow Curve:** Helps determine optimal number of clusters  
- **PCA 2D Plot:** Customer clusters visualized  
- **Centroid Overlay Plot:** Shows the average point in each cluster  
- **3D Cluster Plot (optional):** Age, Income, and Spending Score

---

## 📈 Evaluation

| Metric              | Description                                             |
|---------------------|---------------------------------------------------------|
| Inertia             | Within-cluster sum of squares (WSS)                     |
| Silhouette Score    | Quality of cluster separation (0.0 to 1.0)              |
| Visual Inspection   | PCA and feature plots to verify clear cluster separation |

---


---

## 🙋 Author

**Name:** Naveena Kannati  
**Internship:** AI & ML Internship  
**Task:** Task 8 - K-Means Clustering  
**Date:** June 2025  
**GitHub:** [@kannatinaveena](https://github.com/kannatinaveena)

---

## 📌 Key Takeaways

- K-Means is simple but powerful for segmentation.
- Feature scaling and evaluation metrics are crucial.
- PCA helps in visualizing high-dimensional clusters.
- Silhouette Score helps judge the quality of clustering.

---

## 📬 Feedback & Contributions

Feel free to fork the repo, raise issues, or submit pull requests. Feedback and learning are always welcome!


