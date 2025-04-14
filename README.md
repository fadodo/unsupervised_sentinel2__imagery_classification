# Unsupervised_sentinel2__imagery_classification
Unsupervised Sentinel 2 imagery land cover classification using GEE and geemap package

Two clustering methods have been tested: 
- method 1  : Xmeans
X-Means extends the K-Means clustering algorithm by efficiently estimating the optimal number of clusters within a specified range.
The algorithm iteratively evaluates potential cluster splits using a Bayesian Information Criterion (BIC) to determine the most likely number of clusters.
Users can customize parameters like the minimum and maximum number of clusters, iterations, distance function, and randomization seed for fine-grained control over the clustering process.
Implemented within Earth Engine, X-Means offers a scalable solution for geospatial data analysis and pattern recognition tasks.

- method 2: LVQ
 The algorithm learns by adjusting cluster prototypes based on the input data during training epochs.
LVQ learns a set of codebook vectors (prototypes) that represent clusters in the data. It assigns each data point to the cluster whose prototype is most similar. The prototypes are adjusted iteratively based on training data (even in unsupervised mode, it needs training samples to define the initial prototypes).


Discussions:
- LVQ is potentially better at defining complex cluster shapes. Unlike X-means,LVQ isn't strictly tied to spherical clusters. It can adapt to more irregular cluster boundaries depending on the distribution of the training data.

[XMeans model](https://github.com/fadodo/unsupervised_sentinel2__imagery_classification/blob/main/xmeans_clusterred.html)

[LVQ model](https://github.com/fadodo/unsupervised_sentinel2__imagery_classification/blob/main/lvq_clustered.html)
