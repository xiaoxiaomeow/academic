---
date: 2023-04-01
title: Compression of enumerations and gain
slug: compression_of_enumerations_and_gain
showAuthor: false
authors:
  - g_barmpalias
  - me
  - b_zhan
showReadingTime: false
showWordCount: false
links:
- name: arxiv
  url: https://arxiv.org/abs/2304.03030
- name: pdf
  url: https://arxiv.org/pdf/2304.03030.pdf
---

{{< katex >}}

### Abstract

We study the compressibility of enumerations in the context of Kolmogorov complexity, focusing on strong and weak forms of compression and their gain: the amount of auxiliary information embedded in the compressed enumeration. The existence of strong compression and weak gainless compression is shown for any recursively enumerable (r.e.) set. The density problem of r.e. sets with respect to their prefix complexity is reduced to the question of whether every r.e. set is well-compressible, which we study via enumeration games. 

### Content Overview

Let \(C(\cdot|\cdot)\) denote the [conditional Komogorov complexity](https://en.wikipedia.org/wiki/Kolmogorov_complexity#Conditional_versions). 

Let \(A,B\subseteq\omega\). We say that \(A\) is **rK-reducible** to \(B\), written \(A\leq_{rK} B\), if \(C(A\upharpoonright_n|B\upharpoonright_n)\leq O(1)\). Equivalently, if there is a constant \(k\) and a partial computable function \(f\), such that \(f(B\upharpoonright_n)\) outputs an index \(e\) such that \(A\upharpoonright_n\in W_e\) and \(|W_e|\leq k\) for all \(n\), where \(W_e\) is the \(e^\text{th}\) r.e. set. 

Given r.e. set \(A\), we call a r.e. set \(D\) a **compression** of \(A\) if \(A\leq_{rK} D\). 

- The compression is **gainless** if \(D\leq_{rK} A\). 
- The compression is **strong** if \(D\subseteq 2\mathbb{N}\). 
- The compression is **weak** if \(|D\cap[0,2n)|\leq|A\cap[0,2n)|/2\). 

A set \(A\) is well-compressible if it has a gainless strong compression. 

{{< theorem >}}
Every rK-complete set (that is, an r.e. set \(K\) such that \(A\leq_{rK}K\) for any r.e. set \(A\)) has a strong gainless compression. 
{{< /theorem >}}

{{< theorem >}}
Every r.e. set has a strong compression. 
{{< /theorem >}}

{{< theorem >}}
Every r.e. set has a weak gainless compression. 
{{< /theorem >}}

{{< theorem >}}
Let \(r\) represents any of \(rK\) reduction, \(K\) reduction or \(C\) reduction. If r.e. sets \(A,B\) both have strong gainless compression and \(B<_r A\), then there is an r.e. set \(C\) such that \(B<_r C<_r A\). 
{{< /theorem >}}

{{< theorem type="Corollary" >}}
If every r.e. set has a strong gainless compression, then the \(rK\), \(K\) and \(C\) degrees of r.e. sets are dense. 
{{< /theorem >}}

### Open problem

Does every r.e. set have a strong gainless compression? 

### Relevant contents

- Talk - [Compression of enumerations and gain](/~zhangxy/talk/compression-of-enumerations-and-gain/)