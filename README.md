# 📊 RFM Segmentation using K-Means Clustering

## 🧠 Overview

This project performs **RFM (Recency, Frequency, Monetary)** analysis and uses **K-Means Clustering** to segment customers based on their purchasing behavior. This segmentation helps businesses identify key customer groups and develop targeted marketing strategies.

## 🎯 Objective

To analyze customer purchase patterns and create distinct customer segments using RFM values and unsupervised learning (K-Means Clustering).

## 📁 Dataset

- **Source**: [OnlineRetail dataset]
- **Fields**:
  - `CustomerID`
  - `InvoiceNo`
  - `InvoiceDate`
  - `Quantity`
  - `UnitPrice`

## ⚙️ Methodology

1. **Data Preprocessing**
   - Removed null values and duplicates
   - Filtered out canceled or returned transactions (negative Quantity/Invoice)
   - Created a `TotalAmount` feature: `Quantity * UnitPrice`

2. **RFM Feature Engineering**
   - **Recency**: Days since last purchase
   - **Frequency**: Number of transactions
   - **Monetary**: Total amount spent

3. **Scaling RFM Values**
   - Applied `StandardScaler` to normalize RFM features before clustering

4. **K-Means Clustering**
   - Used the Elbow Method to determine the optimal number of clusters
   - Applied K-Means algorithm to the scaled RFM data
   - Assigned each customer to a cluster

5. **Visualization & Analysis**
   - Plotted cluster distribution
   - Created 3D scatter plots to visualize customer segments
   - Interpreted characteristics of each cluster

## 📈 Results

- Identified **N** distinct customer segments
- Sample Cluster Interpretation:
  - **Cluster 2**: High-frequency, high-monetary loyal customers
  - **Cluster 0**: Recent but low-frequency buyers
  - **Cluster 1**: At-risk or inactive customers
- These insights can help guide targeted marketing campaigns and retention strategies.

## 🛠 Tools & Technologies

- **Languages**: Python
- **Libraries**: Pandas, NumPy, Matplotlib, Seaborn, Plotly, Scikit-learn
- **IDE**: Jupyter Notebook / Google Colab



## 📎 Folder Structure
rfm-kmeans-segmentation/
│
├── data/                # Raw and processed data files
├── images/              # Plots and visualizations
├── rfm_kmeans_segmentation.ipynb  # Main analysis notebook
├── requirements.txt     # List of required Python packages
└── README.md            # Project documentation


## 📬 Contact
For questions, feedback, or collaboration:
Your Name
📧 Email: mkador169@gmail.com

