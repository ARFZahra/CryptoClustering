Crypto Currency Clustering Challenge

Notebook: Crypto_Clustering.ipynb

This challenge demonstrates the application of unsupervised learning using K-Means clustering on a dataset of cryptocurrencies. 


Methodology:
Data Normalization:
The dataset was first normalized using StandardScaler() from the scikit-learn library to ensure all features contributed equally to the clustering process.

Elbow Method to Determine Optimal k:
The elbow method was used to determine the best value for k, which is the number of clusters. By analyzing the elbow curve, it was determined that k = 4 was the optimal number of clusters.

K-Means Clustering:
The data was then fit with a K-Means model, clustering the cryptocurrencies into 4 distinct groups.
These clusters were visualized in a scatter plot for better understanding.

Principal Component Analysis (PCA):
To reduce the dimensionality of the data, Principal Component Analysis (PCA) was applied, reducing the features down to 3 principal components.
The explained variance of these three principal components was 89%, meaning they retained 89% of the information from the original data.

K-Means Clustering After PCA:
After applying PCA, the elbow method was used again to confirm the best value for k.
As with the original data, k = 4 was found to be the optimal number of clusters.
This confirmed that reducing the features to 3 via PCA was appropriate for this dataset.

Comparison of Results:
The elbow curves and scatter plots were compared before and after PCA.

1. Elbow Curve Comparison:
Both the original and PCA-transformed data indicated that 4 clusters were optimal for KMeans clustering.The PCA-transformed data showed lower inertia, meaning the clusters were more compact. This is a result of dimensionality reduction, where less informative features were filtered out, allowing KMeans to form better-defined clusters.

2. Impact of Using PCA:

Using fewer features (via PCA) resulted in more compact and distinct clusters. PCA allowed KMeans to better differentiate between data points by focusing on the core variance of the data.
The overall clustering pattern was consistent in both the original and PCA-transformed data. However, in the PCA plot, the clusters showed better separation and tighter grouping, highlighting the benefit of dimensionality reduction.
