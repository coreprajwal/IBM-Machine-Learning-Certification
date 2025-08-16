🧠 Summary:  


## 🧩 Concept of clustering and applications
- clustering basically, forms clusters of similar type of data
- it is used in user segmentation, anomaly detection etc

## 🧠 Apply k-means clustering to segment customers based on characteristics
- In k-means clustering k no. of clusters are creted based on similarity 

## 🧠 Explain different types of clustering ,including partition,density and heirarchical
- density based clustering form separate clusters based on different density and are circular in shape
- partition based clustering has different python functions such make blob and make moon , on which it does partition


## 🧠 Analyze agglomerative and divisive hierarchical clustering, along with their approaches to grouping data points

- Agglomerative hierarchical clustering is a bottom-up aproach, it forms small clusters and forms relationship with other other small clusters to create a bigger clusters
- it is shown with dendrogram
- it measures distance between two points , takes least distance and forms cluster then mean is taken and from that point distance of other points is taken and thus form all relations and clusters

- devisive hierarchical clustering is a top-down aproach , at first it takes whole as single clusters and then find sub clusters and make relations
- it is also shown with dendrogram


## Describe K-means clustering
- k means clustering is a clustering where k numbers of clusters are created from the whole clusters
- separate cohesive groups are creative 

## explain how k-means algorithm works
- at first k centroids are selected from dataset or positions are selected
- then iteratively distance between two points is data point and centroid is calculated
- cluster with minimum distance is assigned to the data point and mean of the is taken
- the mean now becomes the centroid, and this whole process happens iterative until the centroids position gets stable.


## how to determine k
there are three ways to determine k
- silhoutte Analysis - 
- Elbow Method
- Daivis-Bouldin Method


## Describe DBSCAN and how it works
- DBSCAN takes parameters like epsilon(radius) , N (no. of points),Minimum point and creates clusters based on the these parameters
- if numbers of points are within epsilon and more than N --> core points
- If number of points are within epsilon but less than N --> border points
- If points are not within epsilon --> Noise

## Describe HDBSCAN and how it works
- HDBSCAN doesn't require parameters like dbscan
- it is also efficient for finding noise points
- it merges two radius as one to create clusters
- it first find small clusters and then form relation or connection making thi agglomerative method


## 💡 
