# 🛍️ Customer Segmentation using KMeans Clustering

This repository contains a notebook that performs **customer segmentation** on mall customers using the **KMeans clustering** algorithm. The goal is to identify different customer groups based on features like **Age**, **Annual Income**, and **Spending Score**.

📌 **Task Objective:**
Group similar customers together for targeted marketing based on:
- 🎂 Age
- 💸 Annual Income (k$)
- 💳 Spending Score (1-100)

---

## 🔧 Features

- 🔹 Data cleaning and preprocessing
- 🔹 Label encoding for categorical values
- 🔹 Feature selection and engineering
- 🔹 Elbow method to find optimal clusters
- 🔹 KMeans clustering and analysis
- 🔹 Multiple visualizations:
  - 📉 Elbow Method Plot
  - 📊 2D & 3D Cluster Visualizations
  - 🔥 Heatmap
  - 🎯 Gender & Age distribution across clusters
  - 🔄 Pairwise Feature Relationships

---

## 📂 Dataset

- **Source:** [Mall Customer Segmentation Dataset](https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python)
- **File Used:** `Mall_Customers.csv`

---

## 🛠️ Workflow

1. **Data Preprocessing** 🔧  
   - Renamed columns for clarity  
   - Encoded `Gender` to numeric  
   - Handled missing values (if any)

2. **Clustering Preparation** 🧮  
   - Selected features: `Age`, `Annual Income`, `Spending Score`  
   - Scaled values (optional)  
   - Determined `K` using the **Elbow Method**

3. **Model Training** 🤖  
   - Applied `KMeans(n_clusters=5)`  
   - Assigned cluster labels to data  

4. **Evaluation** 📊  
   - No external accuracy/loss (unsupervised learning)  
   - Cluster analysis using visuals and group statistics

---

## 🧠 Methodology

- **Data Preprocessing & Cleaning** 🧹  
  Handled missing values and standardized column names.

- **Label Encoding** 🔢  
  Converted categorical variables like Gender into numerical format.

- **Feature Selection** 🎯  
  Selected features: `Age`, `Annual Income`, and `Spending Score`.

- **Elbow Method** 🔍  
  Determined optimal number of clusters (K) using the Elbow Curve.

- **KMeans Clustering** 🔄  
  Applied `KMeans` with `K=5` to segment customers into meaningful groups.

- **Cluster Labeling & Analysis** 🏷️  
  Added cluster labels to dataset and visualized patterns.

- **Export Results** 💾  
  Saved the final clustered data as `clustered_customers.csv`.


---

## 🔍 Clustering Evaluation  
Although KMeans is unsupervised, we evaluate using internal metrics:

| Metric                | Description                                      |
|-----------------------|--------------------------------------------------|
| **Inertia**           | ✔️ Printed from Elbow Method                     |
| **Silhouette Score**  | 👍 Measures how well-clustered the data is       |
| **Davies-Bouldin Index** | ✔️ Optional for further evaluation             |

---

## ✅ Results

📋 **Cluster Summary (Means):**

| Cluster | Age (Mean) | Income (Mean) | Spending Score (Mean) |
|--------|-------------|----------------|------------------------|
|   0    |     25.3    |     25.4       |         80.2          |
|   1    |     45.7    |     78.5       |         18.7          |
|   2    |     32.1    |     55.1       |         55.5          |
|   3    |     27.9    |     60.3       |         35.2          |
|   4    |     40.8    |     88.6       |         90.1          |

📁 Final clustered data is saved as: `clustered_customers.csv`

---

## 📸 Visual Outputs

<div align="center">


<table>
  <tr>
    <td>
      <strong>📊 Elbow Method for Optimal K</strong><br>
      <img src="output_images/Elbow Method for Optimal K.png" width="400">
    </td>
    <td>
      <strong>📈 2D Cluster Plot (Annual Income vs Spending Score)</strong><br>
      <img src="output_images/2D Cluster Plot (Annual Income vs Spending Score).png" width="400">
    </td>
  </tr>
  <tr>
    <td>
      <strong>📉 3D Cluster Visualization</strong><br>
      <img src="output_images/3D Cluster Visualization.png" width="400">
    </td>
    <td>
      <strong>📦 Cluster Distribution (Bar plot)</strong><br>
      <img src="output_images/Cluster Distribution (Bar plot).png" width="400">
    </td>
  </tr>
  <tr>
    <td>
      <strong>🧑‍🤝‍🧑 Gender Distribution across Clusters</strong><br>
      <img src="output_images/Gender Distribution across Clusters.png" width="400">
    </td>
    <td>
      <strong>📊 Age Distribution per Cluster (Box plot)</strong><br>
      <img src="output_images/Age Distribution per Cluster (Box plot).png" width="400">
    </td>
  </tr>
  <tr>
    <td>
      <strong>🔥 Feature Correlation Heatmap</strong><br>
      <img src="output_images/Feature Correlation Heatmap.png" width="400">
    </td>
    <td>
      <strong>🔍 Pairwise Relationships (Pairplot)</strong><br>
      <img src="output_images/Pairwise Relationships (Pairplot).png" width="400">
    </td>
  </tr>
</table>

</div>

---

## 🚀 Getting Started

1. Clone the repository  
   `git clone https://github.com/shreyakmukherjee/customer-segmentation-kmeans.git`  
   `cd customer-segmentation-kmeans`

2. Install dependencies  
   `pip install -r requirements.txt`

3. Run the notebook  
   Open `customer_segmentation.ipynb` in Jupyter or Colab.

---

## 🧠 Algorithm Used  
`KMeans` from `sklearn.cluster`

---

## 📌 License  
This project is licensed under the MIT License – see the LICENSE file for details.

---

## ✍️ Author  
👤 **Shreyak Mukherjee**  
📂 GitHub: [shreyakmukherjee](https://github.com/shreyakmukherjee)  
🔗 LinkedIn: [linkedin.com/in/shreyakmukherjee](https://www.linkedin.com/in/shreyak-mukherjee-203558275/)  
Feel free to connect or explore more projects!

---
