---
date: 2024-03-01
title: Growth and irreducibility in path-incompressible trees
slug: growth_and_irreducibility_in_path_incompressible_trees
showAuthor: false
authors:
  - g_barmpalias
  - me
showReadingTime: false
showWordCount: false
links:
- name: arxiv
  url: https://arxiv.org/abs/2206.15425
- name: pdf
  url: https://arxiv.org/pdf/2206.15425.pdf
- name: doi
  url: https://doi.org/10.1016/j.ic.2024.105136
publishedIn:
  name: Information and Computation
---

{{< katex >}}

### Abstract

We study randomness-preserving transformations of path-incompressible trees, namely trees of finite randomness deficiency. We characterize their branching density, and show: (a) sparse perfect path-incompressible trees can be effectively densified, almost surely; (b) there exists a path-incompressible tree with infinitely many paths which does not compute any perfect path-incompressible tree with computable oracle-use. 

### Content Overview

A **string** is a finite binary sequence, and a **real** is an infinite one. A **tree** is a set of finite strings closed under prefix. A real \(x\) is a path of a tree \(T\) if \(\sigma\prec x\) implies \(\sigma\in T\). A string branches in a tree \(T\) if it has at least \(2\) incomparable extensions in \(T\). 

Let \(K(\cdot)\) denote the [prefix-free Komogorov complexity](https://en.wikipedia.org/wiki/Kolmogorov_complexity). The **deficiency** of a string \(\sigma\) is \(|\sigma|-K(\sigma)\). The **deficiency** of a set of strings is the supremum of the deficiencies of its members. 

A tree is **path-incompressible** if it has finite deficiency. A tree is **proper** if it has infinitely many paths. A tree \(T\) is **perfect** if each string in \(T\) branches in \(T\). 

{{< theorem >}}
There is a path-incompressible proper tree that does not wtt-compute any path-incompressible perfect tree. 
{{< /theorem >}}

### Open problem

Is there a path-incompressible proper tree that does not compute any path-incompressible perfect tree?