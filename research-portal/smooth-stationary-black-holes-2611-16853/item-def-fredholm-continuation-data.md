---
title: Fredholm and Banach continuation interfaces
status: published
research_item: def-fredholm-continuation-data
dependency_level: 0
---

## Prerequisites

- [math:def-banach-space](https://alphabetamath.cc/item/def-banach-space)
- [math:def-c-k-map-between-banach-spaces](https://alphabetamath.cc/item/def-c-k-map-between-banach-spaces)
- [math:def-fredholm-operator-cokernel-and-index](https://alphabetamath.cc/item/def-fredholm-operator-cokernel-and-index)
- [math:def-compact-linear-operator](https://alphabetamath.cc/item/def-compact-linear-operator)
- [math:thm-implicit-function-theorem-for-banach-spaces](https://alphabetamath.cc/item/thm-implicit-function-theorem-for-banach-spaces)
- [math:thm-fredholm-index-is-stable-under-compact-perturbations](https://alphabetamath.cc/item/thm-fredholm-index-is-stable-under-compact-perturbations)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [math:def-product-norms-on-finitely-many-normed-spaces](https://alphabetamath.cc/item/def-product-norms-on-finitely-many-normed-spaces)
- [math:thm-finite-products-of-banach-spaces-are-banach](https://alphabetamath.cc/item/thm-finite-products-of-banach-spaces-are-banach)
- [math:thm-compact-implies-the-other-compactness-forms](https://alphabetamath.cc/item/thm-compact-implies-the-other-compactness-forms)
- [math:def-frechet-derivative-between-banach-spaces](https://alphabetamath.cc/item/def-frechet-derivative-between-banach-spaces)
- [math:thm-metric-continuity-characterisations](https://alphabetamath.cc/item/thm-metric-continuity-characterisations)
- [math:thm-reals-cauchy-complete](https://alphabetamath.cc/item/thm-reals-cauchy-complete)


## Definition

Assume the Axiom of Choice. Let $X,Y$ be real Banach spaces: real normed vector spaces complete for their norm metrics. A bounded linear map $L:X\to Y$ is **Fredholm** if its kernel is finite dimensional, its range is closed, and its cokernel $Y/\operatorname{ran}L$ is finite dimensional. Its **index** is $\operatorname{ind}L=\dim\ker L-\dim(Y/\operatorname{ran}L)$.

Equip $\mathbb R\times X$ with the maximum product norm $\|(q,w)\|_{\max}=\max\{|q|,\|w\|_X\}$, for which it is a real Banach space. A **local continuation problem** consists of an open set $U\subseteq\mathbb R\times X$ for this norm and a $C^1$ map $\mathcal H:U\to Y$. Here $C^1$ means Fréchet differentiable with derivative continuous in operator norm. A **zero** is $(q,w)\in U$ with $\mathcal H(q,w)=0$. At such a point the partial derivative $D_w\mathcal H(q,w):X\to Y$ is $D\mathcal H(q,w)$ restricted to vectors of the form $(0,v)$. A **bounded isomorphism** is a bounded linear bijection with bounded linear inverse.

If $D_w\mathcal H(q_0,w_0)$ is a bounded isomorphism at a zero, the implicit-function theorem provides open neighborhoods $A$ of $q_0$ and $B$ of $w_0$ and a unique $C^1$ map $w:A\to B$ whose graph is exactly the zero set of $\mathcal H$ in $A\times B$. This criterion requires invertibility; Fredholm index zero alone does not supply it.

For an endpoint $q_*$, a branch $w(q)$ of zeros can be continued to a zero at $q_*$ by a limit argument when a sequence $q_n\to q_*$ has $w(q_n)\to w_*$ in $X$, $(q_*,w_*)\in U$, and any additional admissibility or graph conditions required by the particular problem hold at the limit. A set of branch values is **relatively compact** when its closure in $X$ is compact for the norm metric. Relative compactness of the branch values can supply a convergent subsequence; it does not by itself ensure that the limit remains in $U$ or satisfies those additional conditions.

If $L$ is Fredholm and $K:X\to Y$ is a compact linear operator, meaning that it maps bounded sets to relatively compact sets, then $L+K$ is Fredholm with the same index. This statement alone does not identify the kernel of $L+K$.

## Justification

The Fredholm terminology and index are those of [math:def-fredholm-operator-cokernel-and-index](https://alphabetamath.cc/item/def-fredholm-operator-cokernel-and-index), and the differentiability convention is that of [math:def-c-k-map-between-banach-spaces](https://alphabetamath.cc/item/def-c-k-map-between-banach-spaces). By [math:thm-reals-cauchy-complete](https://alphabetamath.cc/item/thm-reals-cauchy-complete), every Cauchy sequence of real numbers for the absolute-value metric converges to a real number. Consequently $\mathbb R$ with its absolute-value norm is Banach by [math:def-banach-space](https://alphabetamath.cc/item/def-banach-space). The chosen norm is the maximum product norm of [math:def-product-norms-on-finitely-many-normed-spaces](https://alphabetamath.cc/item/def-product-norms-on-finitely-many-normed-spaces). Since $\mathbb R$ with its absolute-value norm and $X$ are Banach, [math:thm-finite-products-of-banach-spaces-are-banach](https://alphabetamath.cc/item/thm-finite-products-of-banach-spaces-are-banach) makes $\mathbb R\times X$ Banach. The product parameter space and the partial derivative fit the hypotheses of [math:thm-implicit-function-theorem-for-banach-spaces](https://alphabetamath.cc/item/thm-implicit-function-theorem-for-banach-spaces), with parameter space $\mathbb R$, unknown space $X$, and target $Y$; the stated graph conclusion follows under its bounded-isomorphism hypothesis and Choice. Index zero is insufficient for invertibility: the zero map $\mathbb R\to\mathbb R$ has one-dimensional kernel and cokernel, hence index zero, but is not injective. For the endpoint assertion, the differentiability-implies-continuity argument in the Remarks of [math:def-frechet-derivative-between-banach-spaces](https://alphabetamath.cc/item/def-frechet-derivative-between-banach-spaces) applies to the $C^1$ map $\mathcal H$ on the open subset $U$ of the real Banach space $\mathbb R\times X$, so $\mathcal H$ is continuous on $U$. Give $U$ the restricted maximum-norm metric and $Y$ its norm metric. These are metric spaces, so the choice-free implication (a) to (d) of [math:thm-metric-continuity-characterisations](https://alphabetamath.cc/item/thm-metric-continuity-characterisations) makes $\mathcal H:U\to Y$ sequentially continuous. The assumed component limits give $\|(q_n,w(q_n))-(q_*,w_*)\|_{\max}=\max\{|q_n-q_*|,\|w(q_n)-w_*\|_X\}\to0$: for each positive tolerance, both terms are smaller than it once $n$ exceeds their two thresholds. Since the sequence consists of zeros and $(q_*,w_*)\in U$, sequential continuity yields $\mathcal H(q_*,w_*)=\lim_n\mathcal H(q_n,w(q_n))=0$; preservation of any extra conditions must be checked separately. If the branch values have compact closure $C\subseteq X$, [math:thm-compact-implies-the-other-compactness-forms](https://alphabetamath.cc/item/thm-compact-implies-the-other-compactness-forms), assertions 1 and 3, applies to $C$ with its restricted norm metric: compactness implies countable compactness and then sequential compactness. Thus the sequence of branch values has a subsequence converging to a point of $C\subseteq X$. This extraction alone says nothing about membership of the associated limit pair in $U$ or preservation of additional admissibility conditions. The compact-perturbation assertion is exactly [math:thm-fredholm-index-is-stable-under-compact-perturbations](https://alphabetamath.cc/item/thm-fredholm-index-is-stable-under-compact-perturbations) under its stated hypotheses.
