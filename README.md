# Subspace Clustering via Good Neighbors

By Jufeng Yang, Jie Liang, Kai Wang, Ming-Hsuan Yang

## Abstract

Finding the informative clusters of a high-dimensional dataset is at the core of numerous applications in computer vision, where spectral based subspace clustering algorithm is arguably the most widely-studied methods due to its empirical performance and provable guarantees under various assumptions. Such algorithms first compute a linear representation for each sample based on a dictionary, and construct an affinity graph for spectral clustering. It is well-known that sparsity and connectivity of the affinity graph play important rules for effective subspace clustering. However, it is difficult to simultaneously optimize both factor due to their conflicting nature, and most existing methods are designed to deal with only one factor. In this paper, we propose an algorithm to optimize both sparsity and connectivity by finding good neighbors which induce key connections among samples within a subspace. First, an initial coefficient matrix is generated from the input dataset. For each sample, we find its good neighbors which not only have large coefficients but are strongly connected to each other. We reassign the coefficients of good neighbors and eliminate other entries to generate a new coefficient matrix, which can be used by spectral clustering methods. Both theoretical and empirical results show that few good neighbors obtained by the proposed algorithm can recover the subspace effectively, and the post-processing module of finding good neighbors can be complementary to most of the subspace clustering algorithms. Experiments on five benchmark datasets show that the proposed algorithm performs favorably against the state-of-the-art methods in terms of accuracy with a negligible increase in speed.

## Citation

If you find our method useful in your research, please kindly cite our paper:

    @article{yang2019subspace,
    	author={Yang, Jufeng and Liang, Jie and Wang, Kai and Rosin, Paul and Yang, Ming-Hsuan},
    	title={Subspace clustering via good neighbors},
    	journal={IEEE Transactions on Pattern Analysis and Machine Intelligence},
    	year={2019}
    }

## Architecture
<p align="left">
<img src="pipeline.JPG" alt="framework" width="900px">
</p>

For more details, please refer to our [paper](http://liangjie.xyz/).

## Usage

1. Clone this repository;

```shell
git clone https://github.com/JLiangNKU/FGNSC
```

2. Open matlab and cd into the repository;

3. Run main.m and get the clustering result of the extended Yale B dataset.

## Contact

Please feel free to contact me if you have any questions via liang27jie@gmail.com.
