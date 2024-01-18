# Marketing Campaign Analysis using k-means clustering

## Introduction

This project involves the analysis of a marketing campaign dataset. The dataset is loaded, cleaned, and processed for further analysis. The project involves feature engineering, data visualization, and data preprocessing.

## Dependencies

The project uses the following Python libraries:

- numpy
- pandas
- datetime
- matplotlib
- seaborn
- sklearn
- yellowbrick
- warnings
- sys

## Dataset

The dataset used in this project is `marketing_campaign.csv`. The dataset is loaded using pandas and preprocessed for further analysis.

## Data Preprocessing

The preprocessing steps include:

- Loading the dataset
- Dropping null values
- Feature engineering
- Dropping redundant features
- Handling outliers

## Data Visualization

The project involves visualizing key features of the dataset using seaborn and matplotlib.

## Label Encoding

The categorical variables in the dataset are label encoded to convert them into numerical features.

## Data Scaling

The dataset is scaled using the StandardScaler from the sklearn library.

## Dimensionality Reduction

Dimensionality reduction is performed using PCA (Principal Component Analysis) to reduce the dimensions to 3.

## Clustering

The Elbow Method is used to determine the optimal number of clusters. Agglomerative Clustering is then applied to the dataset.

## Cluster Analysis

The clusters are analyzed and visualized using various plots. The distribution of the clusters, cluster profiles based on income and spending, count of promotion accepted, and number of deals availed are some of the aspects analyzed.

## Profiling

Profiling is done based on various personal attributes like the number of kids at home, tenure of the customer, age, number of children, family size, parenthood status, education, and living situation.

## Code

The code for the project is provided in the project repository.

## Conclusion

This project provides insights into the marketing campaign dataset through data preprocessing, feature engineering, data visualization, and cluster analysis.
