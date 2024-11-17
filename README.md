# Overview
This project explores spatial modeling, clustering, and visualization to predict lung cancer rates across parishes in Louisiana using socio-economic and environmental factors. The methodology includes geospatial regression, clustering, and interactive mapping, enabling insights into the relative importance of contributing factors within spatial clusters.

## Project Stages
### 1. Prediction of Lung Cancer Rates Using Geospatial Models
Factors Considered:

#### Socio-Economic: Smoking, Poverty, Income, Insurance
Environmental: PM 2.5 (Air Pollution)

#### Methods Used:
Multiscale Geographically Weighted Regression (MGWR): Incorporates local variations in relationships between predictors and lung cancer rates.
Spatial Autoregressive Models (SAR): Accounts for spatial dependency among observations.
Ordinary Kriging: A geostatistical interpolation technique.
Universal Kriging: Incorporates external variables into the interpolation process.

#### Results:
Based on the results, Universal Kriging was identified as the best-performing model for prediction.

### 2. Spatial Clustering with K-Means
Using the predicted values from Universal Kriging, spatial clustering was performed:

Methodology: K-Means Clustering
Optimal Clusters: Determined using the Elbow Method, resulting in 6 clusters.

### 3. Interactive Visualization with Folium
The predicted lung cancer rates were plotted based on their respective spatial clusters in an interactive map using the Folium library. This visualization allows for intuitive exploration of geographic and cluster-based patterns.

### 4. Relative Importance of Variables in Each Cluster
Using the P-values of the predictors in each cluster, the relative importance of socio-economic and environmental factors was determined within each spatial cluster. This analysis highlights the localized impact of predictors, providing deeper insights into the drivers of lung cancer rates in different regions.

## Tools & Technologies
Python Libraries: Folium, Pandas, scikit-learn, and Geopandas
Geospatial Analysis Tools: MGWR, SAR, and Kriging methods
Clustering Algorithm: K-Means
Results and Insights
Universal Kriging achieved the highest prediction accuracy (R-squared = 0.8981).
Spatial clustering revealed distinct patterns in lung cancer rates, providing actionable insights into regional variations.
The interactive map allows stakeholders to explore these patterns and identify priority areas for intervention.
The variable importance analysis within clusters provides a localized understanding of the predictors' impact.

## Future Work
Expand analysis by integrating additional environmental and health-related factors.
Incorporate temporal analysis to evaluate trends over time.
Explore advanced machine learning models for further accuracy improvements.

## Author
This project was conducted by Mridula Mavuri, a Master's student and Research Assistant specializing in geospatial modeling and deep learning. The work focuses on understanding and predicting lung cancer rates using data-driven techniques, combining advanced spatial modeling, clustering, and visualization methods.
