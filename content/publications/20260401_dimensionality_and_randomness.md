---
date: 2026-04-01
title: Dimensionality and randomness
slug: dimensionality_and_randomness
showAuthor: false
authors:
  - g_barmpalias
  - me
showReadingTime: false
showWordCount: false
links:
- name: arxiv
  url: https://arxiv.org/abs/2405.06961
- name: pdf
  url: https://arxiv.org/pdf/2405.06961.pdf
- name: doi
  url: https://doi.org/10.1145/3806195
publishedIn:
  name: ACM Transactions on Computational Logic
---

{{< katex >}}

### Abstract

Arranging the bits of a random string or real into \(k\) columns of a two-dimensional array or higher dimensional structure is typically accompanied with loss in the Kolmogorov complexity of the columns, which depends on \(k\). We quantify and characterize this phenomenon for arrays and trees and its relationship to negligible classes. 

### Content Overview

Let \(K(\cdot)\) denote the [prefix-free Komogorov complexity](https://en.wikipedia.org/wiki/Kolmogorov_complexity#Prefix-free_Kolmogorov_complexity_K). The **deficiency** \(d(\sigma)\) of a string \(\sigma\) is \(|\sigma|-K(\sigma)\). The **deficiency** of a set of strings \(E\) is \(d(E)=\sup_{\sigma\in E}d(\sigma)\). \(E\) is **incompressible** if it has finite deficiency. 

Generally it is hard to transform "thin" set of incompressible strings, e.g. the set of prefixes of a random real to a "fat" set of incompressible strings, e.g. a tree. We give two theorems based on this observation, and also give positive results to show how "fat" the set needs to be in order to make this transformation hard.

{{< theorem >}}
No incomplete random real computes an \(g\)-fat set of incompressible strings, if \(g\) is a recursive order with \(\lim_n n/g(n)=0\).
{{< /theorem >}}

{{< theorem >}}
Every random real computes an \(n/(\log n)^2\)-fat set of incompressible strings.
{{< /theorem >}}

{{< theorem >}}
No incomplete random real computes a proper pruned incompressible tree.
{{< /theorem >}}

{{< theorem >}}
Every random real computes a perfect weakly-incompressible tree.
{{< /theorem >}}

These results have a connection to deep \(\Pi^0_1\) classes, and we show that they are not direct corollary of previous results.

{{< theorem >}}
There exists a perfect pruned incompressible tree \(T\leq_T\emptyset''\) which is not a member of any \(\Pi^0_1\) class.
{{< /theorem >}}

{{< theorem >}}
For each \(c\), the class of \(c\)-incompressible perfect trees which are not members of any deep \(\Pi^0_1\) class is comeager in the space of \(c\)-incompressible trees.
{{< /theorem >}}

Finally we study the lost of deficiency as a result of growth of "fatness", and also with a positive result. 

{{< theorem >}}
No incomplete random real computes a tree \(T\) with \(\log|T\cap 2^n|\geq 2\log\log|T\cap 2^n|+d(T\cap 2^n)\).
{{< /theorem >}}

{{< theorem >}}
No incomplete random real computes a tree \(T\) and an order \(g\) with \(\log|T\cap 2^n|\geq g(n)+d(T\cap 2^n)\) such that \(n\mapsto|T\cap 2^n|\) is recursive.
{{< /theorem >}}

{{< theorem >}}
For any recursive order \(g\), every random real computes a perfect pruned incompressible tree \(T\) with \(\log|T\cap 2^n|=g(n)\) and \(\lim_n(\log|T\cap 2^n|-d(T\cap 2^n))=\infty\).
{{< /theorem >}} 

### Open problems

- Is it true that no incomplete random real computes a tree \(T\) and an order \(g\) with \(\log|T\cap 2^n|\geq g(n)+d(T\cap 2^n)\)? 

- How to define a deep \(\Pi^0_2\) class or the depth for higher arithmetical classes? 

### Relevant contents

- Talk - [Dimensionality and randomness](/academic/talks/2024_singapore_math/)
- A related paper by Laurent Bienvenu, Christopher P. Porter, [Deep \(\Pi^0_1\) Classes](https://arxiv.org/abs/1403.0450)