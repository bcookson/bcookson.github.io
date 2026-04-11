---
title: "Unifying Proportional Fairness in Centroid and Non-Centroid Clustering"
collection: publications
excerpt: 'Benjamin Cookson, [Nisarg Shah](https://www.cs.toronto.edu/~nisarg/), Ziqi Yu'
conference: '[NeurIPS 2025](https://neurips.cc): Proc. of The Thirty-Ninth Annual Conference on Neural Information Processing Systems, 2025'
link: 'https://arxiv.org/abs/2601.00447'
date: '2025-9-23'
status: 'conference'
note: 'Spotlight Presentation (Top 3.2% of submissions)'
abstract: >-
  Proportional fairness criteria inspired by democratic ideals of proportional representation have received growing attention in the clustering literature. Prior work has investigated them in two separate paradigms. Chen et al. [ICML 2019] study centroid clustering, in which each data point's loss is determined by its distance to a representative point (centroid) chosen in its cluster. Caragiannis et al. [NeurIPS 2024] study non-centroid clustering, in which each data point's loss is determined by its maximum distance to any other data point in its cluster. We generalize both paradigms to introduce semi-centroid clustering, in which each data point's loss is a combination of its centroid and non-centroid losses, and study two proportional fairness criteria -- the core and, its relaxation, fully justified representation (FJR). Our main result is a novel algorithm which achieves a constant approximation to the core, in polynomial time, even when the distance metrics used for centroid and non-centroid loss measurements are different. We also derive improved results for more restricted loss functions and the weaker FJR criterion, and establish lower bounds in each case.
---
