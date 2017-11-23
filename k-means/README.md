### I'm Harry, here's how i implement K-Means clustering algorithm 
#### This is a website that i have refered
- Article https://mubaris.com/2017-10-01/kmeans-clustering-in-python
- Codes: https://github.com/mubaris/friendly-fortnight
#### So let's get started! Yolo


<br><br><center><h1 style="font-size:3em;color:#2467C0">K-Means Clustering

</h1></center>
<br>
<table>
<col width="600">
<col width="500">
<tr>
<td><img src="https://i.imgur.com/S65Sk9c.jpg" align="middle" style="width:660;height:400px;"/></td>
<td>
<strong>
Clustering is a type of Unsupervised learning.
</strong>  This is very often used when you don’t have labeled data. K-Means Clustering is one of the popular clustering algorithm.<strong> The goal of this algorithm is to find groups(clusters) in the given data</strong>. In this post we will implement K-Means algorithm using Python from scratch.
<br>

</td>
</tr>
</table>
## Use Cases

### K-Means is widely used for many applications.

- Image Segmentation
- Clustering Gene Segementation Data
- News Article Clustering
- Clustering Languages
- Species Clustering
- Anomaly Detection

## Algorithm

### Our algorithm works as follows, assuming we have inputs \(x_1, x_2, x_3, …, x_n\) and value of K

- Step 1 - Pick K random points as cluster centers called centroids.
- Step 2 - Assign each \(x_i\) to nearest cluster by calculating its distance to each centroid.
- Step 3 - Find new cluster center by taking the average of the assigned points.
- Step 4 - Repeat Step 2 and 3 until none of the cluster assignments change.

<td><img src="https://i.imgur.com/k4XcapI.gif" align="middle" style="width:550px;height:360px;"/></td>



<br><br><center><h1 style="font-size:3em;color:#2467C0">Choosing the Value of K
</h1></center>
<br>
<table>
<col width="600">
<col width="500">
<tr>
<td><img src="https://i.imgur.com/k3o6NxK.jpg" align="middle" style="width:660;height:400px;"/></td>
<td>
<strong>
Choosing the Value of K
</strong>
We often know the value of K. In that case we use the value of K. Else we use the Elbow Method.
. We run the algorithm for different values of K(say K = 10 to 1) and plot the K values against SSE(Sum of Squared Errors). And select the value of K for the elbow point as shown in the figure.


<br>

</td>
</tr>
</table>

## HOW HARRY CHOOSE THE FACTOR K? 

### Let's find out what exactly does k influence in the algorithm?
<td><img src="https://www.analyticsvidhya.com/wp-content/uploads/2014/10/K-judgement.png" align="middle" style="width:660;height:400px;"/></td>

<td><img src="https://www.analyticsvidhya.com/blog/wp-content/uploads/2014/10/K-judgement2.png" align="middle" /></td>
