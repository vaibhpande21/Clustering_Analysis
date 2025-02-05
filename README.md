# Scaler Learner Clustering

## Project Overview
Scaler is an online tech-versity offering intensive computer science and data science courses through live classes delivered by industry experts. The goal of this project is to analyze and cluster Scaler learners based on job profiles, company details, and other key features to identify meaningful groups with similar characteristics.

## Dataset
The dataset consists of multiple features related to learners, including:
- **CTC (Compensation)**
- **Years of Experience**
- **Designation**
- **Class** (Education Level)
- **Tier** (Institution Tier)

## Approach
### 1. **Data Preprocessing**
- Standardized numerical features using `StandardScaler`.

### 2. **Dimensionality Reduction & Visualization**
- **PCA (Principal Component Analysis)** for variance analysis.
- **t-SNE (t-Distributed Stochastic Neighbor Embedding)** for non-linear separability.
- **UMAP (Uniform Manifold Approximation and Projection)** to identify density variations.

### 3. **Clustering Techniques**
- **K-Means Clustering**
  - Used elbow method and silhouette score to determine optimal clusters.
  - Final model: `k=6`.
- **Gaussian Mixture Models (GMM)** for probabilistic clustering.
- **Hierarchical Clustering** using Ward’s method and dendrogram analysis.
- **DBSCAN** for density-based clustering (did not perform well due to varying densities).

### 4. **Cluster Interpretation**
- Clusters were analyzed using radar plots to understand feature importance.

## Actionable Insights & Recommendations
1. **Early Career Support**: Identified a segment of learners with low salaries and experience. Scaler can provide targeted mentorship and specialized career guidance.
2. **Industry Growth Monitoring**: Some clusters indicated slow salary progression despite promotions. Scaler could tailor advanced learning paths for these industries.
3. **Anomaly Detection**: Certain clusters exhibited anomalous trends. Further analysis can help refine data quality and improve clustering accuracy.

## Results & Visualization
- Interactive scatter plots and 3D visualizations were used to interpret clusters.
- PCA and t-SNE plots helped understand the structure of the data.

## Technologies Used
- **Python** (pandas, numpy, scikit-learn, plotly, scipy, umap)
- **Machine Learning Algorithms** (K-Means, GMM, Hierarchical, DBSCAN)
- **Data Visualization** (Plotly, Matplotlib, Seaborn)

## Future Work
- Improve clustering by engineering additional features.
- Implement deep learning techniques for better segmentation.
- Perform model validation using real-world employment trends.

---
?? **Author:** Vaibhav 
