
# HW6: Clustering - K-means

This project focuses on the implementation of the K-means clustering algorithm and its variant, K-means++. The task involves applying these algorithms to perform color image quantization, a process that compresses images by reducing the number of colors.

## Description

Color image quantization transforms an image into a representation that uses a smaller subset of colors compared to the original. This process reduces the number of bits needed for color representation, compressing the image with minimal perceived difference from the original.

K-means clustering is used here to group similar colors, and the color of each pixel is replaced with the centroid of the closest cluster. The algorithms used are:
- **K-means**
- **K-means++**: An improved version of K-means that optimizes the choice of initial centroids.

## Algorithms

### K-means

K-means groups the image pixels in the RGB space into a specified number of clusters, based on the Minkowski distance. Each pixel is assigned to the nearest centroid, and the centroids are recalculated iteratively until convergence or until a maximum number of iterations is reached.

### K-means++

K-means++ improves the initialization of the centroids to avoid poor clustering. It selects initial centroids that are spread out, which reduces the chance of getting stuck in local minima and helps the algorithm converge faster.

