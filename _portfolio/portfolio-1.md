---
title: "MovieLens Recommender System and Extensions"
excerpt: "Implementation and evaluation of a collaborative-filtering recommender system with Spark using the MovieLens dataset. (May 2022)"
collection: portfolio
---

Implementation and evaluation of a collaborative-filtering recommender system with Spark using the MovieLens dataset, with comparison to single-machine implementation and application of approximate nearest neighbor method for accelerated search at query time.

[Report](http://luiginoto.github.io/files/movielens_recommender_system/Project_Report.pdf) [Repository](https://github.com/luiginoto/movielens_recommender_system)

### Abstract
We build and evaluate a collaborative-filtering based recommender system with [Spark alternating least squares (ALS)](https://spark.apache.org/docs/3.0.1/ml-collaborative-filtering.html) implementation using the [MovieLens dataset](https://grouplens.org/datasets/movielens/latest/). We compare the Spark’s parallel ALS model to [lenskit](https://lkpy.readthedocs.io/en/stable/index.html) single-machine implementation in terms of efficiency and model performance. Finally, we implement accelerated search at query time using [Annoy](https://github.com/spotify/annoy) spatial data structure, and compare this fast search method to the brute force approach in terms of query efficiency and quality of recommendation.

### Authors
- Guilherme Albertini
- Giacomo Bugli
- Luigi Noto

<br/>
**Validated Best ALS Results**

|   Data Size   | Reg Param | Rank | Max Iter | MAP@100 | NCDG@100 |
|:-------------:|:---------:|:----:|:--------:|:-------:|:--------:|
| Small (Train) |    0.01   |  30  |    20    |  0.1232 |  0.3541  |
|  Small (Test) |    0.01   |  30  |    20    |  0.0661 |  0.1621  |
|  Full (Train) |    0.1    |  30  |    35    |  0.1795 |  0.2659  |
|  Full (Test)  |    0.1    |  30  |    35    |  0.0832 |  0.1973  |



