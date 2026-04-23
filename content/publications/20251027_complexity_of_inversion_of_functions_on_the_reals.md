---
date: 2025-10-27
title: Complexity of inversion of functions on the reals
slug: complexity_of_inversion_of_functions_on_the_reals
showAuthor: false
authors:
  - g_barmpalias
  - me
  - m_wang
showReadingTime: false
showWordCount: false
links:
- name: arxiv
  url: https://arxiv.org/abs/2412.07592
- name: pdf
  url: https://arxiv.org/pdf/2412.07592.pdf
- name: doi
  url: https://doi.org/10.1017/S0960129525100224
publishedIn:
  name: Mathematical Structures in Computer Science
---

{{< katex >}}

### Abstract

We study the complexity of deterministic and probabilistic inversions of partial computable functions on the reals. 

### Content Overview

We regard a Turing functional \(f\) as a (possibly partial) map (function) from \(2^\omega\) to \(2^\omega\), that is, \(f(x)\) is the real \(y\) such that \(y(n)=f^x(n)\) (the output of \(f\) with oracle \(x\) and input \(n\)) for all \(n\). In this way we can talk about functions from \(2^\omega\) to \(2^\omega\) and the partial computable ones. Let \(\mathsf{ML}\) be the collection of all Martin-Löf random reals. 

Given functions \(f,g\), \(g\) is an \textbf{inversion} of \(f\) if \(f(g(y))=y\) for all \(y\in f(2^\omega)\). More generally, we give \(g\) access to a random oracle and only require it to succeed on positive measure, that is, we consider

\[L_{f,g}=\{(x,r):f(g(f(x),r))=f(x)\},\]
\[R_{f,g}=\{(y,r):f(g(y,r))=y\}.\]

Given partial computable \(f\), we define \(f\) to be

- **oneway** if \(\mu(f^{-1}(\mathsf{ML}))>0\) and \(\mu(R_{f,g})=0\) for all partial computable \(g\). 
- **left-oneway** if \(\mu(\mathsf{dom}(f))>0\) and \(\mu(L_{f,g})=0\) for all partial computable \(g\). 
- **right-oneway** if \(\mu(f(2^\omega))>0\) and \(\mu(R_{f,g})=0\) for all partial computable \(g\). 

We also define \(f\) to be \(w\)-oneway if we quantify over all \(w\)-computable \(g\). 

A function \(f\) is **random-preserving** if \(\mu(\mathsf{dom}(f))>0\) and \(f\) maps randoms to randoms. 

In the paper we explore the basic properties of partial computable functions and probabilistic inversions of them. 

{{< theorem >}}
There is a total computable random-preserving surjection \(f\) which has no continuous inversion. 
{{< /theorem >}}

{{< theorem >}}
For partial computable \(f\), \(\mu(f^{-1}(\mathsf{ML}))>0\) if and only if \(f\) extends a partial computable random-preserving function. 
{{< /theorem >}}

{{< theorem >}}
If \(f\) is oneway then \(f\) is right-oneway. If \(f\) is right-oneway and random-preserving then \(f\) is left-oneway. 
{{< /theorem >}}

{{< theorem >}}
There is a partial computable random-preserving left-oneway function that is not right-oneway. 
{{< /theorem >}}

Also we want to characterize the collection of oracles that can compute probabilistic inversion of all partial computable functions. 

{{< theorem >}}
For any oracle \(w\), \(w\) computes a probabilistic inversion of every total computable \(f\) (i.e. every total computable \(f\) is not \(w\)-oneway) if and only if \(\emptyset'\leq_T w\). 
{{< /theorem >}}

{{< theorem >}}
For any oracle \(w\), if \(\emptyset''\leq_T w\) then \(w\) computes a probabilistic inversion of every partial computable \(f\) (i.e. every partial computable \(f\) is not \(w\)-oneway). 
{{< /theorem >}}

We are also interested in injective oneway functions. 

**Fact**. Every total computable injective \(f\) is not oneway. 

{{< theorem >}}
For any oracle \(w\), if \(\emptyset'\leq_{LR} w\) then \(w\) computes a probabilistic inversion of every partial computable injective \(f\) (i.e. every partial computable injective \(f\) is not \(w\)-oneway). 
{{< /theorem >}}

{{< theorem >}}
There is a partial computable injective left-oneway function. 
{{< /theorem >}}

### Open problem

- What are, exactly, the collection of oracles \(w\) such that every partial computable \(f\) is not \(w\)-oneway? 

- Is there a partial computable injective oneway function? 

- What are, exactly, the collection of oracles \(w\) such that every partial computable injective \(f\) is not \(w\)-oneway? 

### Relevant contents

- Talk - [Computable oneway functions on the reals](/academic/talks/2025_hangzhou/) at Hangzhou Delta23