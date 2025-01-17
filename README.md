# Real-Time Indexing of Arbitrarily Attributed Point Clouds

Link to pdf: [here](real-time-indexing-of-arbitrarily-attributed-point-clouds.pdf)

## Abstract

The demand for up-to-date airborne or terrestrial Light Detection and Ranging (LiDAR) data sets is increasing. This works by emitting a laser beam from a scanner. Based on the time of flight, the distance between each reflection point and scanner can be calculated, resulting in 3D point clouds. These point clouds are typically stored unindexed during acquisition. After acquisition, processing and indexing algorithms have to be run as time-consuming batch processes. To avoid this post-processing, the necessary processing steps can be implemented in real-time pipelines to further process and store data during acquisition. Not only spatial indexing but also indexing of many possible attributes of LiDAR points play an important role in applications such as data quality assurance or real-time preview. In this thesis, a real-time approach for attribute indexing of LiDAR point clouds is presented, which extends the spatial index structure of Modifiable Nested Octrees with attribute indexing. The attribute index is implemented by storing attribute ranges contained in each subtree. In addition to spatial restrictions, attribute filters can be defined in the form of attribute-value ranges for queries. Nodes whose ranges do not overlap with the attribute filters can then be sorted using the attribute ranges stored in the octree nodes. An implementation of the approach is presented and measured using a terrestrially acquired dataset of 365 million points. Indexing speeds of over 400 000 points per second can be achieved, and the time for queries with attribute filters can be reduced to 1%-50% of the time required for linear filtering of all indexed points, while on average 33% of all unwanted points can be discarded. These values are achievable on simple consumer hardware, provided a fast hard disk is available.

## Cite

```
@misc{Hermann_2023,
	title        = {Real-Time Indexing of Arbitrarily Attributed Point Clouds},
	author       = {Hermann, Paul},
	year         = 2023,
	url          = {https://publica.fraunhofer.de/handle/publica/458643},
	language     = {en}
}
```
