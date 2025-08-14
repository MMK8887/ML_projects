# SUMMARY

This project performs customer segmentation on the Mall Customers dataset using K-Means clustering and explores DBSCAN as an alternative. The goal is to group customers based on their annual income and spending score to identify distinct customer segments.

The analysis uses the `Mall_Customers.csv` dataset, which contains information about mall customers, including their CustomerID, Genre, Age, Annual Income (k$), and Spending Score (1-100).

## Steps
1. **Data Loading and Exploration**: The dataset was loaded into a pandas DataFrame and initial exploration was performed to understand the data structure and identify potential issues.
2. **Feature Selection**: The 'Annual Income (k$)' and 'Spending Score (1-100)' columns were selected as the features for clustering.
3. **Feature Scaling**: The selected features were scaled using `StandardScaler` to normalize their ranges and ensure equal contribution to the clustering process.
4. **Determining Optimal Number of Clusters for K-Means**: The Elbow method and Silhouette score were used to determine the optimal number of clusters for K-Means clustering. Both methods suggested 5 as a suitable number of clusters.
5. **K-Means Clustering**: K-Means clustering was applied to the scaled features with 5 clusters.
6. **Visualization**: The resulting clusters were visualized using a 2D scatter plot, showing the distribution of customers based on their income and spending score, colored by their assigned cluster.
7. **Cluster Analysis**: The average spending score for each cluster was calculated to understand the characteristics of each segment.
8. **DBSCAN Experimentation**: DBSCAN clustering was applied as an alternative clustering method to explore different segmentation approaches.

## Key Findings
- The optimal number of clusters for K-Means was determined to be 5.
- K-Means clustering identified 5 distinct customer segments based on income and spending score.
- Analysis of the average spending score per cluster revealed variations in spending behavior across the segments.
- DBSCAN clustering with initial parameters showed the potential to identify clusters and noise points, indicating the need for parameter tuning.

## Detailed Cluster Insights
- Cluster 1: Avg. Spending Score ≈ 79.34
- Cluster 2: Avg. Spending Score ≈ 82.13
- Cluster 0: Avg. Spending Score ≈ 49.52
- Cluster 3: Avg. Spending Score ≈ 17.11
- Cluster 4: Avg. Spending Score ≈ 16.49

## Conclusion
- High-spending clusters (1 and 2) represent valuable customer groups for targeted marketing.
- Further demographic analysis could enhance segmentation strategies.