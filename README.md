# MSCS_634_Lab_5
This lab introduces clustering techniques using Hierarchical and DBSCAN Clustering algorithms.

## Purpose

This lab explores clustering techniques on the Wine dataset to uncover natural groupings in the data without using the original labels. I applied **Hierarchical Agglomerative Clustering** and **DBSCAN** to analyze the dataset’s structure, visualize clusters in reduced dimensions (PCA), and evaluate cluster quality using metrics like silhouette, homogeneity, and completeness scores.

---

## Key Insights

- **Hierarchical Clustering** produced clear, well-separated clusters with meaningful structure, supported by dendrogram analysis. Choosing the number of clusters (`n_clusters`) significantly influenced the results.
- **DBSCAN** identified clusters based on data density and was able to detect noise points (outliers). However, its effectiveness depended heavily on tuning parameters `eps` and `min_samples`.
- PCA visualizations helped to intuitively assess cluster separability and compare clustering results.
- Silhouette scores were useful for validating cluster cohesion, but DBSCAN sometimes returned undefined scores when clusters were not well-formed.
- Homogeneity and completeness scores highlighted how well clusters aligned with the original class labels, showing varied results depending on the algorithm and parameters.

---

## Challenges and Decisions

- Selecting appropriate parameters for DBSCAN (`eps` and `min_samples`) was challenging and required multiple experiments to balance noise detection and meaningful cluster formation.
- Deciding the optimal number of clusters for hierarchical clustering involved interpreting dendrograms and visual assessments.
- Standardizing the features was necessary to ensure fair distance computations and improve clustering performance.
- Handling noise points from DBSCAN and interpreting their meaning required careful analysis since they could represent outliers or data irregularities.

---
