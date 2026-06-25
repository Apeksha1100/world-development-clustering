# world-development-clustering

## Project Overview

This project analyzes global development indicators and groups countries with similar characteristics using Machine Learning clustering techniques.

The objective is to identify meaningful patterns among countries based on economic, health, tourism, technology, and business-related indicators. Clustering helps identify developed, developing, and emerging economies through a data-driven approach.

---

## Problem Statement

Countries across the world differ significantly in terms of economic growth, healthcare, business environment, tourism, and technological development.

Manual comparison of countries is complex and time-consuming. This project uses unsupervised machine learning techniques to group similar countries and uncover hidden patterns in global development data.

---

## Objectives

- Analyze world development indicators.
- Clean and preprocess real-world data.
- Perform Exploratory Data Analysis (EDA).
- Apply multiple clustering algorithms.
- Compare clustering performance using evaluation metrics.
- Identify meaningful country groups.
- Deploy the final clustering model.

---

## Dataset Information

The dataset contains various world development indicators for multiple countries.

### Features

- Country
- GDP
- Health Expenditure Per Capita
- Business Tax Rate
- Internet Usage
- Mobile Phone Usage
- Tourism Inbound
- Tourism Outbound
- Life Expectancy (Male and Female)
- Ease of Doing Business

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn
- PCA
- K-Means Clustering
- Hierarchical Clustering
- DBSCAN
- Gaussian Mixture Model (GMM)
- Mean Shift

---

## Project Workflow

### 1. Data Preprocessing

- Handled missing values
- Removed duplicates
- Cleaned inconsistent formats
- Converted data into numerical format
- Treated outliers

### 2. Exploratory Data Analysis

- Box Plots
- Histograms
- Correlation Heatmap
- Scatter Plots
- Outlier Analysis

### 3. Feature Engineering

Created new features:

- Average Life Expectancy
- Total Tourism

Removed redundant features to improve clustering performance.

### 4. Feature Scaling

Applied StandardScaler to normalize the data.

### 5. Dimensionality Reduction

Used Principal Component Analysis (PCA) to reduce dimensions while retaining 95% of the variance.

### 6. Clustering Algorithms

Implemented and compared:

- K-Means
- Hierarchical Clustering
- DBSCAN
- Gaussian Mixture Model (GMM)
- Mean Shift

### 7. Model Evaluation

Models were evaluated using Silhouette Score.

---

## Results

| Algorithm | Silhouette Score |
|------------|-----------------|
| K-Means | 0.24 |
| Hierarchical Clustering | 0.21 |
| Gaussian Mixture Model | 0.18 |
| DBSCAN | 0.02 |
| Mean Shift | 0.00 |

K-Means achieved the highest Silhouette Score and was selected as the final clustering model.

---

## Key Insights

- Developed countries showed higher GDP, healthcare spending, internet usage, and business performance.
- Developing countries formed a separate cluster with moderate indicators.
- Emerging economies were grouped together based on growth-related characteristics.
- PCA improved cluster visualization and reduced dimensionality effectively.

---

## Repository Structure

```text
├── world-development-clustering.ipynb
├── world_development (1).py
├── P659_World_development_dataset.xlsx
├── clustering_kmeans.pkl
├── clustering_pca.pkl
├── clustering_scaler.pkl
├── features.pkl
├── README.md
```

---

## Deployment Files

The following files were saved for deployment:

- clustering_kmeans.pkl
- clustering_scaler.pkl
- clustering_pca.pkl
- features.pkl

These files allow the clustering pipeline to be loaded without retraining the model.

---

## Challenges Faced

- Handling missing values
- Cleaning inconsistent data formats
- Managing outliers in GDP and tourism indicators
- Selecting the optimal number of clusters
- Dealing with overlapping country characteristics
- Dimensionality reduction using PCA
- Comparing multiple clustering algorithms

---

## Conclusion

This project successfully analyzed world development indicators using unsupervised machine learning techniques.

Multiple clustering algorithms were implemented and compared. K-Means produced the best clustering performance and generated meaningful country groups representing different levels of development.

The project demonstrates how machine learning can support economic analysis, policy planning, investment research, and global benchmarking.

---

## Future Scope

- Integration with World Bank API
- Real-time global development dashboard
- Regional clustering by continent
- Year-wise trend analysis
- Deep Learning-based clustering techniques
- Interactive visualization using Streamlit

---

## Author

Apeksha Sonawane

Data Science and Analytics Enthusiast
