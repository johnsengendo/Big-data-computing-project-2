# Big-data-computing
## Clustering of data points
Clustering is a great technique in data science for processing big data based on similarities. For example grouping different customers in a market based on thier behaviour and similarities. Also clustering can be applied in analysing and grouping networks on social media sites.
In this project, I cluster points based on the similarity of distance between them.
The main task of the project was to find the number of clusters [ selected between 8 - 12] in the dataset that gives the best silhouette coefficient which is a measure of how similar a data point is within a cluster compared to other clusters (separation).

### Different clusters are created in the data and the center of each clustar is selected among the data points.
* To evaluate similarities among points, I use the [KMean clustering](https://scikit-learn.org/stable/modules/generated/sklearn.cluster.KMeans.html) algorithm where distance computation among points are computed.
* I use Intellij to run the program [program](clustering.JPG) by inputting the number of clusters needed and cluster centers are selected from the data.
* I returns the sum of squared euclidean distances between the pair of points. That is, a point and its closest center. 
* Points that are close to a particular center are put in a similar cluster.
### Clustering illustration using silhouette <br>
![BER](clustering.JPG)

* Silhouette coefficient was used to evaluate how good my clustering was. 
* A value near +1 indicates that the sample points are far away from the neighboring clusters and so points are well clusterd. 
* A value of 0 indicates that the sample points are on or very close to the decision boundary between two neighboring clusters and negative values indicates that the sample points might have been assigned to the wrong cluster.
