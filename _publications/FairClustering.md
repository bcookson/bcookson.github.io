---
title: "Improved Lower Bounds for Proportionally Fair Clustering"
collection: publications
excerpt: 'Benjamin Cookson, Eva Deltl, Yeeseok Oh'
conference: 'Working Paper'
link: '/files/fair-clustering-arxiv-final.pdf'
date: '2026-06-01'
status: 'working'
abstract: >-
  We study proportionally fair clustering, where a set of $k$ centers must be chosen from a metric
  space to represent $n$ agents, and no sufficiently large group of agents should be collectively
  underrepresented. One of the central notions of fairness in this setting is the $\alpha$-core.
  The existence of clusterings in the $(1+\sqrt{2})$-core was established by Chen et al. [2019],
  who also showed instances where the $\alpha$-core is empty for every $\alpha < 2$. Closing this
  gap has remained an open problem for seven years. We make progress from the lower-bound side by
  providing an instance whose $\alpha$-core is empty for every $\alpha < 2.1508$. Our techniques
  rely on establishing connections between variants of the core, namely the Hare core and the Droop
  core; reducing the search for optimal empty-core instances to a highly structured family of
  clustering instances; and using a Mixed Integer Linear Program (MILP) to search for optimal
  lower-bound instances within this reduced space. Using this framework, we also determine tight
  bounds for Droop quota clustering instances with a small number of possible candidate centers and
  a single center to be selected. For each number of centers $m \in \{3,4,5,6\}$, we give the
  exact threshold $\alpha^*_m$ such that an $\alpha^*_m$-core clustering always exists, while for
  every $\alpha < \alpha^*_m$ there is an instance with $m$ centers whose $\alpha$-core is empty.
  Although these values were originally found through computer-aided search, we also provide direct
  proofs that do not rely on MILP certificates.
---
