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

**Cluster Profiling** - Naming the cluster according to the common characteristics of the points in it.

**How to select K-value**

- Plot Elbow graph/ Scree Plot


**3. DBSCAN**

- DBSCAN - Density Based Spatial Clustering of Application with Noise.

**Disadvantages of K-Means** - 
 
1. Cannot be used on data with noise(outliers).

2. K-Means does not perform well on non-spherical data. DBSCAN does.

3. We have to priorly determine the value of k in K-Means.

- DBSCAN is used for non-spherical data and also where data has lot of outliers, it will identify tehm seperately.

**Important Terminology for DBSCAN**

- epsilone - User given parameter - Defines size and borders of each neighbourhood. It will depend on domain and we have to trial and error dependeing how many outliers are we getting. 

- Minpoints - User given parameters - Min number of points in neighnourhood to call it a dense region. Density Threshold. Generally choose minpoints >= D+1. D = no. of columns.

- Core point - 

- Border point

- Noisy point

**Disadvantage of DBSCAN**

- Difficult with data whose density is low.

- It is an itterative procedure to determine eps and minpoints.

- computational complexity.
