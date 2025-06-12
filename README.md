# dbscan-nonlinear-clustering
📄 Documentation: DBSCAN Clustering of Concentric Circles
Objective:
To apply DBSCAN (Density-Based Spatial Clustering of Applications with Noise) to a synthetic dataset consisting of concentric circles and visualize the clustering results.

Tools & Libraries:
Python Libraries:

matplotlib for plotting

numpy for numerical operations

sklearn.datasets for dataset generation

sklearn.cluster.DBSCAN for clustering

Methodology:
Dataset Creation:

Used make_circles to generate a synthetic dataset with two concentric circles.

Parameters:

n_samples=500 (total points)

factor=0.5 (distance between circles)

noise=0.03 (added randomness)

random_state=4 (reproducibility)

Clustering with DBSCAN:

Applied DBSCAN with:

eps=0.1 (maximum distance between two samples for them to be considered neighbors)

min_samples=5 (minimum number of points required to form a dense region)

Cluster labels were predicted using fit_predict.

Visualization:

Used a scatter plot to visualize the clustered data.

Different clusters were color-coded using the viridis colormap.

Axis labels and a descriptive title were added.

Key Learnings:
DBSCAN can effectively cluster non-linearly separable data like concentric circles.

The algorithm automatically identifies noise points.

Parameter tuning (eps and min_samples) is crucial for meaningful clusters.
