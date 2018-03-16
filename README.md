# Clustering analysis

A k-means cluster analysis was conducted to identify underlying subgroups of adolescents based on their similarity of responses
on 11 variables that represent characteristics that could have an impact on deviant behavior. 
Clustering variables included two binary variables measuring whether or not the adolescent had ever used alcohol or marijuana,
as well as quantitative variables measuring alcohol problems, scales measuring violence, depression, self-esteem, 
parental presence, parental activities, family connectedness, as well as school connectedness and school achievements .
 
All clustering variables were standardized to have a mean of 0 and a standard deviation of 1. 
We split the data into training (70% of the observations) and test dataset (30% of the observations), 
random state ensure that the data will be split the same way when the code is run again

A series of k-means cluster analyses were conducted on the training data specifying k=1-7 clusters, using Euclidean distance.
The variance in the clustering variables that was accounted for by the clusters (r-square) 
was plotted for each of the seven cluster solutions in an elbow curve to provide guidance for choosing the number of clusters 
to interpret.

![w1](https://user-images.githubusercontent.com/18068773/37516930-1e5e1172-2910-11e8-9275-882025d67050.png)

This plot shows the decrease of the average distance of the observations from the cluster centroids as the number of clusters increases. 
The elbow curve suggests that the 2, 3 and 6-cluster solutions might be interpreted. The results below are for an interpretation of the 3-cluster solution.
Canonical discriminant analyses was used to reduce the 11 clustering variable down a few variables that accounted for most of the variance in the clustering variables. 

![w2](https://user-images.githubusercontent.com/18068773/37517200-e7ae3106-2910-11e8-9f6a-438a7e3b4c7e.png)

A scatterplot of the first two canonical variables by cluster indicated that the observations in clusters in dark green  and purple were densely packed with relatively low within cluster variance, and did not overlap very much with the yellow cluster. Cluster Yellow was generally distinct, and the observations had less spread suggesting low within cluster variance.  The results of this plot suggest that the best cluster solution may have been 2 , so it will be especially important to also evaluate the 2 cluster solution.

![w3](https://user-images.githubusercontent.com/18068773/37517293-30d0ad1e-2911-11e8-9bd4-c14a33b5db78.png)

The means on the clustering variables shows that compared to other clusters,  cluster 0 includes the least adolescents having used alcohol, marijuana and had the lowest number of alcohol problems, violence, depression. They had greater self-esteem , school and family connectedness, higher GPA and parents activity and presence.  So cluster 0 include the least troubled adolescents
Cluster 2 includes the adolescents who had highly used alcohol and marijuana, experienced more alcohol problems, and violent behavior, they appear also to have higher levels of depression, lower self-esteem and school achievement  as well as the lowest levels of school and family connectedness , parents presence and activity.
Cluster 1 include adolescents who had more used Alcohol but tend to fall in between the two other clusters in the use of Marijuana,  having alcohol problems, engaging in violence, depression, self-esteem, school and family connectedness, parents activity and GPA, with the exception of having higher parental involvement in activities. 




