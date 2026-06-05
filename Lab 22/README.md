# Clustering World Economies with K-Means & PCA

## Objective

Apply unsupervised machine learning techniques to identify patterns among countries based on socioeconomic development indicators and evaluate how data-driven clusters align with established World Bank income classifications.

## Methodology

* Collected 10 country-level development indicators for approximately 160 countries using the World Bank API (`wbgapi`).
* Cleaned and prepared the dataset for clustering analysis.
* Standardized all features using `StandardScaler` to ensure each variable contributed equally to distance calculations.
* Applied K-Means clustering to group countries with similar economic and development characteristics.
* Fit a baseline K-Means model with **K = 4** clusters and visualized cluster structure using a two-dimensional Principal Component Analysis (PCA) projection.
* Evaluated alternative cluster solutions using both the **elbow method** and **silhouette analysis** across values of **K = 2–10**.
* Compared machine-learning-generated clusters against official World Bank income classifications through cross-tabulation analysis.
* Replicated the clustering workflow on the California Housing dataset to demonstrate the generalizability of the methodology across different domains.

## Key Findings

* Cluster analysis revealed distinct groupings of countries based on shared economic and development characteristics.
* Model selection diagnostics indicated that **K = [INSERT OPTIMAL K]** provided the strongest balance between cluster separation and within-cluster cohesion.
* Comparison with World Bank income classifications showed that the algorithmic clusters **[closely aligned / partially aligned / weakly aligned]** with traditional income group definitions, suggesting that development patterns extend beyond income alone.
* PCA visualization demonstrated meaningful separation between clusters, indicating that countries with similar socioeconomic profiles tend to occupy similar positions in the reduced feature space.
* Application of the same pipeline to California Housing data produced coherent geographic and socioeconomic groupings, highlighting the flexibility of K-Means clustering for exploratory data analysis.
* The project illustrates how unsupervised learning can uncover latent structures in complex economic datasets and provide an alternative perspective to conventional classification systems.
