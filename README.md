# Image Clustering
### Overview
This repository contains my implementation of the K-Means clustering algorithm for handwritten digit images.
The dataset consists of 10,740 images, each represented as a 28x28 matrix of pixel values, flattened into a 1x784 vector. 
The goal is to cluster similar images together (in this case, K is set to 10 for the digits 0-9).

### Implementation
🔯Starting with a comprehensive Data Analysis, I visualized different styles of the same digit, recognizing the variability in pixel values.

🔯For Data Preprocessing, specific features contributing to distinct styles were ignored, and averaging pixel values with Gaussian smoothing was employed to enhance image similarity.

🔯Dimensionality Reduction played a crucial role, with Principal Component Analysis (PCA) reducing the dataset dimension from 784 to 65 and t-distributed Stochastic Neighbor Embedding (t-SNE) further reducing dimensions to 2D. 

🔯The core lies in the K-Means Clustering algorithm, where I implemented functions for generating random centroids, assigning clusters based on Euclidean distances, updating centroids, and running the K-Means algorithm until convergence.

🔯 Finally, the optimal number of clusters was determined through an evaluation process involving the plotting of inertia and silhouette score metrics, leading to the selection of K=10 for the final clustering solution. 

### Results/ Observation
The clustering solution achieved a V-measure metric score of 0.80 on the test dataset, demonstrating its effectiveness in grouping similar handwritten digit images.
