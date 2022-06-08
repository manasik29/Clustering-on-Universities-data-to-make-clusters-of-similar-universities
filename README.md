# Clustering

**1. Heirarchical Clustering**

- It is a bottom to top approach. 

- Find the euclidian distance between two points. Club closest point in one cluster.

- Then find the euclidian distance between two cluster / distance between one cluster and one point. We will again club the shortest distance in one cluster.

- Method to calculate euclidian distance

  - Single Linkage - shortest distance between 2 points in clusters.

  - Average Linkage - largest distance between 2 points in clusters.

  - Complete Linkage - Average of distance between all points in clusters.

  - Centroid Linkage - Find centroids of each clusters and find the distance between their centroids.

- If the data has both binary and numerical data. First convert the binary categorical data to 0 & 1 and standardize the numerical data. And perform heirarchical clustering on it.


**2. K-Means Clustering**

- Mostly used for practical uses. Will be used in industry frequently.

- Assume K = 3 (# of clusters)

- Find centroid for each partition

- Find distance between all data points to all cluster centroids.

- Move/Reassign datapoints to the nearest centroids.

- As the data has now changed so Recompute the centroids.

- Repeat step 3 - 5.

- Continue till we dont have to move any datapoint closer to any other centroid.

**Cluster Profiling**

**How to select K-value**

- Plot Elbow graph/ Scree Plot


**3. DBSCAN**

- 
