# Unsupervised Machine Learning: Clustering Analysis Project

## Overview
This project is focused on **Exploratory Data Analysis** using unsupervised machine learning techniques to analyze and segment a dataset with clustering algorithms. The **K-Means** , **Agglomerative Hierarchical Clustering (AHC)**, **DBSCAN** and **BIRCH** models have been applied to form clusters, meeting the objective of product segmentation for targeted marketing and logistics. 

Model performance is evaluated using:
- **Silhouette Coefficient**
- **Davies-Bouldin Index**

Additionally, runtime and memory usage are assessed to recommend the best model for deployment.

---

## Problem Statement
The goal of this project is to:
- **Explore and analyze** the international trade dataset to discover underlying patterns.
- **Group similar transactions** and segment products using unsupervised machine learning techniques.
- **Determine the optimal number of clusters** through evaluation metrics such as Silhouette Coefficient and Davies-Bouldin Index, dendrograms (AHC), and elbow method (K-Means).
- **Identify cluster characteristics** to:
  - Segment products.
  - Analyze preferred shipping methods.
  - Uncover product groupings and potential supply chain outliers.

---

## Dataset
The dataset comprises **15,000 entries**, with a random sample of **5,001 rows** selected for analysis. It contains the following variables:

### Key Variables
- **Index**: 
  - `Transaction_ID`
  - `Invoice_Number`
- **Categorical**:
  - `Country`
  - `Import_Export`
  - `Product`
  - `Category`
  - `Shipping_Method`
  - `Port`
  - `Payment_Terms`
  - `Supplier`
  - `Customs_Code`
  - `Invoice_Number`
- **Non-Categorical**:
  - `Value`
  - `Weight`
  - `Quantity`

---

## Objectives
1. **Clustering Performance Evaluation**:
   - Measure clustering performance using **Silhouette Coefficient** and **Davies-Bouldin Index**.
2. **Clustering Algorithm Application**:
   - Implement **K-Means** and **Agglomerative Hierarchical Clustering (AHC)** models.
3. **Cluster Optimization**:
   - Determine the optimal number of clusters using:
     - Elbow Method (K-Means)
     - Dendrogram Analysis (AHC)
4. **Cluster Analysis**:
   - Analyze cluster characteristics to identify:
     - Patterns in the data.
     - Key product segments.
     - Preferred shipping methods.
     - Outliers and high-value segments.

---

## Methods
- **Clustering Models**:
  - **K-Means Clustering**
  - **Agglomerative Hierarchical Clustering (AHC)**
- **Evaluation Metrics**:
  - **Silhouette Coefficient**
  - **Davies-Bouldin Index**
- **Optimization Techniques**:
  - **Elbow Method** (K-Means)
  - **Dendrogram Analysis** (AHC)
- **Cluster Characterization**:
  - Examine key variables (`Category`, `Value`, `Weight`) to describe clusters.

---

## Results
1. **Optimal Number of Clusters**:
   - **K-Means**: Determined via Elbow Method.
   - **AHC**: Determined via Dendrogram Analysis.
2. **Cluster Characteristics**:
   - Identified distinct clusters with unique characteristics (e.g., premium vs. budget segments).
3. **Model Comparison**:
   - **K-Means**:
     - Faster runtime.
     - Low memory usage.
   - **AHC**:
     - Higher memory usage.
     - Suitable for hierarchical data structures.

---

## Conclusion
The clustering analysis successfully segmented the dataset into meaningful groups, providing actionable insights for targeted marketing and logistics optimization. **K-Means** is recommended for large datasets due to its efficiency, while **AHC** is better suited for smaller datasets requiring hierarchical structure analysis.
