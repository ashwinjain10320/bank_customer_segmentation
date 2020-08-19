# bank_customer_segmentation

It is very important for banks to classify its customers into groups to ensure proper flow of money inside and out. I have come up with a project that could do the task for the bank. This task was easily achieved with the use of **unsupervised machine learning.**


### what is unsupervised learning?
Unsupervised learning is a type of machine learning algorithm used to draw inferences from datasets consisting of input data without labeled responses. Unlike supervised learning, it does not gives any kind of output rather is needed to answer simple questions on inferences and conclusions.

### on what basis people are grouped?
![image.png](attachment:https://github.com/ashwinjain10320/bank_customer_segmentation/blob/master/image.png)

### how do i achieved the task?
 workflow of project : 
 
 1] At first I cleaned as well as removed nan values from the data set in order to make it work effectively for solution to my problem. I had to do data visualization for better performance.
 
 2] now i made use of an unsupervised learning algorithm that is called **K-Means clustering**.
 ##### what is Kmeans clustering?
    K-means clustering is one of the simplest and popular unsupervised machine learning algorithms. In other words, the K-means algorithm identifies k number of centroids, and         then allocates every data point to the nearest cluster, while keeping the distance from centroids as small as possible.
    steps involved in KMeans clustering:

    a] Identifying number of clusters K.
    b] selecting random K points for being centroid.
    c] Assigning data points to nearest cluster.
    d] Calculating new centroid.
    e] Reassigning each datapoint to nearest closest centroid.
    f] repeat d] and e] for more better results.
##### how to find optimal number of clusters?
for this we make use of ***WCSS(Within Cluster Sum Of Squares) or we can call it the Elbow method***
formula-> sum(dist(Pi,C1)^2) + sum(dist(Pi,C2)^2) +sum(dist(Pi,C3)^2)
afterwards we plot graph between k and number of clusters and take the elbow part point as an optimistic data point

##### now we apply KMeans method to find centroid for all features
##### finally we search for cluster that are being needed as per our requirement 
##### last but not the least we make use of PCA(Principal component Analysis) that performs dimensionality reductions while keeping unchanged original information and we form a scatterplot that looks like this.
![result.png](attachment:https://github.com/ashwinjain10320/bank_customer_segmentation/blob/master/result.png)
