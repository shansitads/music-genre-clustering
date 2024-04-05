# 🎻 Music Genre Clustering

> Level 3

### 📝 Analysis

Considering that the goal of this project was to see how quantitative genre classification compares to qualitative genre classification, I thought it would be better to first introduce a qualitative discussion of the results as they compare to my understanding of different genres.

The clustering algorithms eventually formed the following clusters:  
<img src="../assets/classifications.png" alt="clusters" width="30%">

- Classical, folk, jazz were clustered together
- Pop formed its own cluster
- Electronic formed its own cluster
- Hip-Hop formed its own cluster
- Rock formed its own cluster

Notably, classical, folk and jazz all tend to have relatively acoustic sounds but typically of different instruments However, the dataset utlized only contained this information through a confidence score of whether the track was acoustic or not, without identifying the type instrument. Moreover, these genres also often observe similar levels of instrumentalness, speechiness, and liveliness. Therefore, it makes sense that these would be clustered together at a lack of differentiation of instruments utilized.

### 📊 Evaluation Metrics

I selected the:

- Davies-Bouldin Index; and
- Calinski-Harabasz Index

for my evaulation metrics, both of which are popular choices for evaluating clustering algorithms.

Both indices provide easily interpretable results. Lower values of the Davies-Bouldin Index indicate better clustering, as it measures the average similarity between each cluster and its most similar cluster.  
Meanwhile, higher values of the Calinski-Harabasz Index indicate better clustering, as it measures the ratio of dispersion between and within clusters.

In the context of genre classification, tracks have been clustered with others that have apparently similar audio features. So these scores would give us a quantitative method to compare how similar different songs that have grouped together are, and also how different each genre is from the others.

Therefore, by considering the two metrics, we can get a full picture of clustering through the comparison of tracks within each genre as well as across different genre.

### 📚 Resources Utilized

- [Stern, Samuel Walter, "Analysis of Music Genre Clustering Algorithms" (2021). Theses and Dissertations. 2839.](https://dc.uwm.edu/cgi/viewcontent.cgi?article=3844&context=etd)
- [GeeksForGeeks](https://www.geeksforgeeks.org/clustering-metrics/#steps-to-evaluate-clustering-using-sklearn)

### 🎁 Level 3 bonus tasks attempted:

- [x] explaining why a specific evaluation metric is useful for the focus question you chose<br>
- [x] describing what an evaluation metric means in real world terms (in context of your focus question)<br>
- [x] code comments (up to the grader's discretion)<br>
