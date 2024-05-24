## Country Data Clustering Analysis
# Overview
This project involves clustering countries based on various socio-economic and health indicators using KMeans and Agglomerative Clustering techniques. The analysis includes data preprocessing, model building, evaluation using silhouette scores, and visualization of the clusters.

# Dataset
The dataset contains socio-economic and health indicators for multiple countries. It encompasses a wide range of variables including child mortality rates, exports and imports as a percentage of GDP, health expenditure relative to GDP, per capita income, inflation rates, life expectancy, total fertility rates, and GDP per capita (GDPP). These indicators offer insights into various aspects of a country's development, including its economic performance, healthcare system, and population demographics. Analyzing this dataset allows for a comprehensive assessment of the socio-economic and health status of different countries, facilitating comparisons and identifying areas for potential intervention or policy reform.

## Requirements

The following Python packages are required:

- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- plotly


## Project Structure

1. Import Libraries
2. Load Dataset
3. Data Exploration
   1. Correlation Heatmap
   2. Pairplot
4. Data Preprocessing
5. KMeans Clustering
   1. Finding Optimal Number of Clusters
   2. Silhouette Score
   3. KMeans Clustering with Optimal Clusters
   4. PCA for Visualization
6. Agglomerative Clustering
   1. Silhouette Score
   2. Agglomerative Clustering with Optimal Clusters
   3. PCA for Visualization


# Conclusion
After analyzing the optimal number of clusters using silhouette scores for both K-means and agglomerative clustering on the country dataset, it was observed that K-means clustering resulted in tighter and more cohesive clusters compared to agglomerative clustering. The silhouette scores indicated that K-means achieved better separation between clusters and higher cohesion within clusters, leading to more distinct and well-defined groupings of countries. This suggests that K-means may be more suitable for this dataset, as it effectively captured the underlying patterns and structure in the data, resulting in more meaningful and interpretable clusters. Agglomerative clustering, on the other hand, produced clusters that were less compact and more spread out, indicating lower cohesion and potentially overlapping clusters. Overall, based on the analysis, K-means clustering appeared to be more effective in partitioning the countries into distinct and homogeneous groups based on their socio-economic and health factors.


