# CryptoClustering

## Cryptocurrency Clustering Analysis

# Overview
This project analyzes and clusters cryptocurrency market data using K-Means clustering. The analysis includes both the original data with all features and a reduced dataset using Principal Component Analysis (PCA) to understand the impact of dimensionality reduction on clustering results.

# Data
The dataset used in this analysis is sourced from Resources/crypto_market_data.csv, containing various price change percentages for different cryptocurrencies over multiple timeframes.

# Steps Involved
# 1. Data Preparation
Loading Data: The dataset is loaded into a Pandas DataFrame and initial exploratory data analysis is performed.
Normalization: Data is normalized using StandardScaler to ensure all features contribute equally to the analysis.

# 2. Clustering Analysis
Using Original Data
K-Means Clustering: K-Means clustering is applied directly to the normalized data.
Elbow Method: The optimal number of clusters is determined using the Elbow method, plotting the inertia values for different k-values.
Using PCA Data
Dimensionality Reduction: PCA is applied to reduce the dataset to three principal components.
K-Means Clustering: K-Means clustering is performed on the reduced dataset.
Elbow Method: The optimal number of clusters is also determined using the Elbow method for the PCA data.

# 3. Visualization
Elbow Curves: Composite plots are created to contrast the Elbow curves for both the original and PCA data.
Cluster Visualization: Scatter plots are generated to visualize the clusters formed in both the original and PCA-reduced data.

# 4. Analysis and Results
The project concludes with a comparison of clustering results with and without using PCA, highlighting the impact of dimensionality reduction on clustering quality.

# Files
Crypto_Clustering.ipynb: Jupyter notebook containing the full analysis and code.
Resources/crypto_market_data.csv: Source data file used for the analysis.
README.md: This file, providing an overview and documentation for the project.

# How to Run
Run Jupyter Notebook:
Launch Jupyter Notebook and open Crypto_Clustering.ipynb to view and run the analysis.

# Conclusion
The analysis demonstrates how PCA can enhance the clustering process by reducing dimensionality, leading to more distinct and compact clusters. The results from both the original and PCA-transformed data are compared to understand the benefits of using fewer features in clustering.
