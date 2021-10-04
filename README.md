# KMeans Clustering

## Overview
In this work, I have written the KMeans Clustering Algorithm. The main key point in performance of KMeans is the number of clusters and position of initial centroids. In this work, I have compared the performance of KMeans Clustering Algorithm with two different centroid initialization strategies on different number of clusters (2-10).

### Strategy 1 
In this case, I chose the initial centroids randomly from the given data samples

### Strategy 2
In this case, I chose the first centroid randomly from the given data samples. All the rest of the centroids are chosen in a way that the distance of the current centroid from all the previous centroids is maximal.

## Installation
To use this repo, create a conda environment using ```environment.yml```

```
# from environment.yml
conda env create -f environment.yml
```

## Results
When I ran the code multiple times, it was visible that the plot for Strategy 1 was sometimes getting abnormal. It must be because of random choice of centroids. But, the plot for Strategy 2 showed very minute changes everytime. But still, the plot for Strategy 2 is a lot more smoother than Strategy 1. Therefore, Strategy 2 is better in terms of performance but it has a drawback as well. The model takes more time to train in case of Strategy 2 due to the extra calculations. Thus, it depends on you and the data you have that which strategy is better.
