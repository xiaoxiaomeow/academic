---
date: 2025-09-01
title: Computable one-way functions on the reals
slug: computable_oneway_functions_on_the_reals
showAuthor: false
authors:
  - g_barmpalias
  - me
showReadingTime: false
showWordCount: false
links:
- name: arxiv
  url: https://arxiv.org/abs/2406.15817
- name: pdf
  url: https://arxiv.org/pdf/2406.15817.pdf
- name: doi
  url: https://doi.org/10.1016/j.ic.2025.105327
publishedIn:
  name: Information and Computation
---

{{< katex >}}

### Abstract

A major open problem in computational complexity is the existence of a one-way function, namely a function from strings to strings which is computationally easy to compute but hard to invert. Levin (2023) formulated the notion of one-way functions from reals (infinite bit-sequences) to reals in terms of computability, and asked whether partial computable one-way functions exist. We give a strong positive answer using the hardness of the halting problem and exhibiting a total computable one-way function. 

### Content Overview

We regard a Turing functional \(f\) as a (possibly partial) function from \(2^\omega\) to \(2^\omega\), that is, \(f(x)\) is the real \(y\) such that \(y(n)=f^x(n)\) (the output of \(f\) with oracle \(x\) and input \(n\)). 

Given functions \(f,g\), we say that \(g\) **inverts** \(f\) on \(y\) if \(f(g(y))=y\), that is, \(g\) outputs one of the preimage of \(y\). We say that \(g\) is an **inversion** of \(f\) if \(g\) inverts \(f\) on any \(y\in{\rm ran}f\). 

A function \(f\) is **random-preserving** if it maps randoms to randoms. 

{{< theorem >}}
There is a random-preserving total surjective Turing functional \(f\) such that any inversion of \(f\) computes \(\emptyset'\).
{{< /theorem >}}

We may also give \(g\) the access to a random oracle \(r\). By letting 
\[L_{f,g}=\{(y,r):f(g(y,r))=y\},\]
Levin defined a Turing functional \(f\) to be **one-way** if \(\mu(L_{f,g})=0\) for all Turing functionals \(g\), and asked if there is a random-preserving one-way function. We give a positive answer. 

{{< theorem >}}
There is a random-preserving total surjective Turing functional \(f\) such that any function \(g\) with \(\mu(L_{f,g})>0\) computes \(\emptyset'\).
{{< /theorem >}}

### Relevant contents

- Talk - [Computable one-way functions on the reals](/academic/talks/2024_singapore_comp/) at Singapore School of Computing seminar
- Talk - [Computable oneway functions on the reals](/academic/talks/2025_hangzhou/) at Hangzhou Delta23