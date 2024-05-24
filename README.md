## Country Data Clustering Analysis
# Overview
This project involves clustering countries based on various socio-economic and health indicators using KMeans and Agglomerative Clustering techniques. The analysis includes data preprocessing, model building, evaluation using silhouette scores, and visualization of the clusters.

# Dataset
The dataset contains socio-economic and health indicators for multiple countries. It encompasses a wide range of variables including child mortality rates, exports and imports as a percentage of GDP, health expenditure relative to GDP, per capita income, inflation rates, life expectancy, total fertility rates, and GDP per capita (GDPP). These indicators offer insights into various aspects of a country's development, including its economic performance, healthcare system, and population demographics. Analyzing this dataset allows for a comprehensive assessment of the socio-economic and health status of different countries, facilitating comparisons and identifying areas for potential intervention or policy reform.

### Dataset Summary

The `df.describe()` function provides statistical summaries of socio-economic and health factors for 167 countries:

- **Child Mortality Rate**: On average, countries exhibit a moderate child mortality rate, with significant variations observed across nations.
- **Export and Import Figures**: Indicate a diverse range of economic activity, suggesting differences in trade dynamics among countries.
- **Health Expenditure as a Percentage of GDP**: Exhibits considerable variability, highlighting differences in healthcare spending priorities across nations.
- **Income Levels**: Vary widely, with a significant spread from low to high-income countries, reflecting disparities in economic prosperity.
- **Inflation Rate**: Moderate on average, but with significant disparities among nations, indicating differences in monetary policy effectiveness.
- **Life Expectancy**: Shows a promising average, albeit with variations across countries, reflecting differences in healthcare access and quality.
- **Total Fertility Rates**: Suggest diversity in population growth patterns, with implications for demographic trends.
- **GDP per Capita**: Reflects a wide range of economic development levels among countries, indicating differences in economic performance and standards of living.

Overall, the dataset underscores the considerable heterogeneity among nations concerning socio-economic development and health outcomes.

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
  
### Correlation Heatmap

The correlation heatmap provides insights into the relationships between various socio-economic and health factors for 167 countries:

- **Income and Life Expectancy**: There is a strong positive correlation (0.61) between income and life expectancy, indicating that countries with higher incomes tend to have longer life expectancies.
- **Child Mortality and Life Expectancy**: A strong negative correlation (-0.89) is observed between child mortality and life expectancy, suggesting that countries with higher child mortality rates tend to have lower life expectancies.
- **Health Expenditure and Life Expectancy**: A moderate positive correlation (0.50) is found between health expenditure and life expectancy, indicating that countries with healthier populations tend to have longer life expectancies.
- **Trade and Income**: There is a weak positive correlation (0.52) between exports and income, implying that countries with higher exports tend to have higher incomes. Additionally, a weaker negative correlation (-0.12) is observed between imports and income, suggesting that the relationship between a country's imports and its income is not as strong.



# Inferences
After analyzing the optimal number of clusters using silhouette scores for both K-means and agglomerative clustering on the country dataset, it was observed that K-means clustering resulted in tighter and more cohesive clusters compared to agglomerative clustering. The silhouette scores indicated that K-means achieved better separation between clusters and higher cohesion within clusters, leading to more distinct and well-defined groupings of countries. This suggests that K-means may be more suitable for this dataset, as it effectively captured the underlying patterns and structure in the data, resulting in more meaningful and interpretable clusters. Agglomerative clustering, on the other hand, produced clusters that were less compact and more spread out, indicating lower cohesion and potentially overlapping clusters. Overall, based on the analysis, K-means clustering appeared to be more effective in partitioning the countries into distinct and homogeneous groups based on their socio-economic and health factors.


