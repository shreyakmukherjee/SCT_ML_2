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
