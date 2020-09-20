# K-Means Clustering
To understand K-Means Clutering, let us first understand a few basic concepts about it. 

So first, lets start with
## What is Clustering?
To state it directly, **clustering is the process of dividing the items/dataset into groups, consisting of similar data-points. And these groups are called clusters**.
The points in the same cluster are as similar as possible while the points in diffent clusters are as dissimilar as possible.

Let me explain by giving an example.
When you go to the supermarket, you see that **the similar things**, such as apple, banana, orange,etc, **are grouped together** in the fruit section. Similarly, potato, onion, garlic, etc are grouped together in the vegetable section. So we can say that these sections **are cluster of similar type** of things, and as mentioned above, **this process of creating clusters is called clustering**.
___
So now that you have basic understanding about clusters, lets us see where clustering can be used.
* On shopping sites, clustering is used to recommend certain products to the customers based on his/her past purchase history.
* It is used in banking to divide customers into various clusters and then give specific offer to specific group based on their account usage, balance,  or particular interests.
* Netflix, Amazon Prime, Disnep+ Hostar and various entertainment sites like these uses clustering to suggest a new show/movie to the person based on this watch history.
These are some simple uses of clustering.

Also talking about clustering, there are mainly three different types of clustering

**1. Exclusive Clustering** 
  * Also known as Hard Clustering, in this tye of clustering **data point or items belongs exclusively to one cluster**. 
  * The K-Means algorithm belongs to this type of clustering.
  
  <p align="center">
  <img src="https://github.com/patelkishan9286/Kishan_ML_K-MeansClustering/blob/master/EC.PNG">
  </p>

**2. Overlapping Clustering**
  * Also known as Soft Clustering, in this type of clustering data point or items belongs to multiple cluster.
  * An example of this type of clustering are Fuzzy C-Means Clustering.
  
  <p align="center">
  <img src="https://github.com/patelkishan9286/Kishan_ML_K-MeansClustering/blob/master/OC.PNG">
  </p>

**3. Hierarchical Clustering**
  * In Hierarchical Clustering, the aim is to produce a hierarchical series of nested clusters.
  * A diagram called Dendrogram graphically represents this hierarchy and is an inverted tree that describes the order in which factors are merged (bottom-up view) or cluster are break up (top-down view).
  
  <p align="center">
  <img src="https://github.com/patelkishan9286/Kishan_ML_K-MeansClustering/blob/master/HC.PNG">
   </p>
___
So now back to **K-Means Clustering**, it **is an unsupervised learning algorithm**.
From the above explanation, you must have understand that in clustering, we do not have a target to predict. We look at the data and then try to club similar observations and form different groups. Hence it is an unsupervised learning problem in which we do not have any fixed target/dependent variable, we only have the independent variables.

The **K** in the k-means stands for **the number of clusters required**.
K-means is a centroid-based algorithm, or a distance-based algorithm, where we calculate the distances to assign a point to a cluster. In K-Means, each cluster is associated with a centroid.
The main objective of the K-Means algorithm is to minimize the sum of distances between the points and their respective cluster centroid.

So to apply K-Means alogrithm, follow the below given steps:
### Step 1 - Select the total number of clusters to be identified.
  * Select the number of cluster needed for the grouping of data.
  * There is a method called the elbow method to efficiently select the value of k.
### Step 2 - Randomly select k distinct points.
  
### Step 3 - Measure the distance between 1st point and selcted k clusters.
### Step 4 - Assign 1st point to the nearest cluster.
### Step 5- Calculate the mean including the new point for the cluster.
### Step 6 - Continue the same procedure for all the points but use the new mean of the cluster to measure the distance from the point.
