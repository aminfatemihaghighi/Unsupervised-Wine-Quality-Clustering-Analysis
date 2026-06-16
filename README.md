# Unsupervised Wine Quality Clustering Analysis

## Project Overview
This repository contains a machine learning project focused on exploratory data analysis (EDA) and unsupervised learning. The objective is to apply clustering algorithms to segment wine samples based on their physicochemical attributes and uncover natural structures within the dataset.

## Technical Stack
* **Language:** Python
* **Libraries:** Scikit-learn, Pandas, NumPy, Matplotlib, Seaborn
* **Algorithms Applied:** K-means Clustering, Hierarchical Clustering

## Methodology & Analysis
1. **Exploratory Data Analysis (EDA):** Cleaned decimal inconsistencies, generated boxplots to detect outliers, and plotted feature distribution histograms. 
2. **Correlation Analysis:** Utilized a correlation heatmap to analyze relationships between parameters. Notable insights include a strong positive correlation between fixed acidity and density ($0.68$), and a negative correlation between alcohol content and density ($-0.49$).
3. **Optimizing Cluster Selection:** Evaluated the optimal number of data segments using two complementary verification techniques:
    * **Elbow Method:** Plotted within-cluster sum of squares (WSS) versus $k$, revealing a distinct elbow point at $k = 3$ with a distortion score of approximately $288,310.69$.
    * **Silhouette Analysis:** Calculated silhouette metrics across multiple cluster counts, peaking at a score of $0.60$ for $2$ clusters, indicating highly distinct and well-defined boundaries.

## Key Conclusions
The project successfully groups data based on chemical profiles, demonstrating how unsupervised metrics balance cluster compactness with separation. This pipeline provides a framework that can be directly adapted to segment traveler profiles or demand zones in mobility networks.
