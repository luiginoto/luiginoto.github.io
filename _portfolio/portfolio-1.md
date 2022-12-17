---
title: "Neural Re-Ranking for Personalized Home Search"
excerpt: "Implementation and evaluation of a self-attention based context-aware re-ranking model for improving personalized home search experience at Zillow (December 2022)"
collection: portfolio
---

Implementation and evaluation of a self-attention based context-aware re-ranking model for improving personalized home search experience at Zillow as part of the Capstone Project for MS in Data Science at NYU.

[Poster](http://luiginoto.github.io/files/neural_reranking/Capstone_Poster_Team_D.pdf) [Report](http://luiginoto.github.io/files/neural_reranking/Capstone_Final_Report.pdf) [Repository](https://github.com/luiginoto/movielens_recommender_system)

### Abstract
Search Systems generate search results via multiple stages of incremental modeling complexity, where the set of candidate items gets progressively narrowed down and ranked based on some notion of relevance. The last step of this process, the re-ranking layer, is then aimed at refining the ranking produced in the previous steps by modeling the cross-item interactions as well as users’ preference behaviors. In this project we partnered with Zillow Group to improve their search feature by implementing context-aware personalized re-ranking for home search. We adopt a self-attention based neural architecture to directly model the mutual influences between all items in the previously ranked list. The experimental results on the dataset provided by Zillow demonstrate significant performance gains of the proposed model with respect to the considered baselines. Finally, we prove that personalization has a positive impact on the re-ranking problem by conducting a feature ablation study.

### Authors
- Luigi Noto
- Giacomo Bugli
- Guilherme Albertini



