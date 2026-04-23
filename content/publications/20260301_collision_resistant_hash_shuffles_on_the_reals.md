---
date: 2026-03-01
title: Collision-resistant hash-shuffles on the reals
slug: collision_resistant_hash_shuffles_on_the_reals
showAuthor: false
authors:
  - g_barmpalias
  - me
showReadingTime: false
showWordCount: false
links:
- name: arxiv
  url: https://arxiv.org/abs/2501.02604
- name: pdf
  url: https://arxiv.org/pdf/2501.02604.pdf
- name: doi
  url: https://doi.org/10.1016/j.ic.2026.105426
publishedIn:
  name: Information and Computation
---

{{< katex >}}

### Abstract

Oneway real functions are effective maps on positive-measure sets of reals that preserve randomness and have no effective probabilistic inversions. We construct a oneway real function which is collision-resistant: the probability of effectively producing distinct reals with the same image is zero, and each real has uncountable inverse image.

### Content Overview

We regard a Turing functional \(f\) as a (possibly partial) function from \(2^\omega\) to \(2^\omega\), that is, \(f(x)\) is the real \(y\) such that \(y(n)=f^x(n)\) (the output of \(f\) with oracle \(x\) and input \(n\)) for all \(n\). In this way we can talk about functions from \(2^\omega\) to \(2^\omega\) and the partial computable ones. Let \(\mathsf{MLR}\) be the collection of all Martin-Löf random reals. 

Given functions \(f\) and \(g\), \(g\) is an **probabilistic inversion** of \(f\) if 

\[\mu(\{(y,r):f(g(y,r))=y\})>0.\]

We define partial computable \(f\) to be **oneway** if it is random-preserving (\(f(\mathsf{MLR})\subseteq\mathsf{MLR}\)) and it has no partial computable probabilistic inversion. 

Given functions \(f,g\), we also consider 

\[\{r:g(r)=(x,z),x\neq z,f(x)=f(z)\}\]

which are the random oracles on which \(g\) can produce **siblings** of \(f\). 

We define partial computable \(f\) to be **collision-resistant** if no partial computable \(g\) can produce siblings of \(f\) with positive probability. 

{{< theorem >}}
There exists a total computable \(f\) which is
- a random-preserving oneway surjection
- collision-resistant and nowhere injective

and for each random \(w\not\geq_T 0'\),
- \(w\) does not compute any probabilistic inversion of f
- \(w\) does not compute any pair of f-siblings.
{{< /theorem >}}

{{< theorem >}}
For each noncomputable r.e. set \(A\) there is a total computable nowhere injective surjective function \(f\) such that
- f is oneway and collision-resistant relative to almost all oracles
- f is not oneway and not collision-resistant relative to \(A\).
{{< /theorem >}}

### Relevant contents

- Talk - [Computable oneway functions on the reals](/academic/talks/2025_hangzhou/) at Hangzhou Delta23