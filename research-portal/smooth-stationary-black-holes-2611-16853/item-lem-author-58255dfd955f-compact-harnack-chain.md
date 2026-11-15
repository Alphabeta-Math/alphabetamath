---
title: Finite Harnack chains on fixed compact connected interior sets
status: draft
research_item: lem-author-58255dfd955f-compact-harnack-chain
dependency_level: 2
---

## Prerequisites

- [def-exterior-weighted-elliptic-data](item-def-exterior-weighted-elliptic-data)
- [lem-author-58255dfd955f-local-potential-harnack](item-lem-author-58255dfd955f-local-potential-harnack)
- [math:def-compact-space](https://alphabetamath.cc/item/def-compact-space)
- [math:def-connected-space](https://alphabetamath.cc/item/def-connected-space)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)


## Statement

Let $(\Sigma,h)$ be a smooth three-dimensional Riemannian exterior and let $K\subset\Sigma^\circ$ be a nonempty compact connected subset, with compactness and connectedness taken in its subspace topology. There are finitely many interior coordinate balls $U_i$, $1\le i\le N$, with compact closures in their chart domains, whose concentric half-balls $H_i$ cover $K$. Each $H_i$ meets $K$, and the graph with vertices $1,\ldots,N$ and an edge between distinct $i,j$ exactly when $H_i\cap H_j\cap K\ne\varnothing$ is connected, meaning any two vertices can be joined by a finite sequence of edges. All balls are Euclidean in their respective coordinates. For any positive real function $u$ on $\bigcup_i U_i$, if $C_*\ge1$ and $u(x)\le C_*u(y)$ for every $x,y\in H_i$ and every $i$, then $\sup_Ku\le C_*^N\inf_Ku$. Thus the conditional comparison applies to every positive solution of $(\Delta_h-V)u=0$ for which these local comparisons hold.

In particular, work in ZFC for the following analytic consequence. Fix such a finite chart cover. Consider smooth Riemannian metrics $h$, potentials $V:\bigcup_i U_i\to[0,\infty)$ bounded on each $U_i$, and positive real $C^2$ functions $u$ solving $(\Delta_h-V)u=0$ pointwise there, where $\Delta_h=\operatorname{div}_h\operatorname{grad}_h$. Write $r_i$ for the coordinate radius of $U_i$ and, in its coordinates, put $m_i=\sqrt{\det(h_{ab})}$, $A_i=(m_i h^{ab})$ and $q_i=m_iV$. Suppose fixed constants $\lambda_i>0$, $M_i<\infty$ and $Q_i\ge0$, independent of the family member, satisfy $\xi^TA_i(x)\xi\ge\lambda_i|\xi|^2$, $\|A_i(x)\|_{\mathrm{op}}\le M_i$ and $q_i(x)\le Q_i$ on $U_i$ for every $\xi\in\mathbb R^3$. Then the comparison is uniform over the family: $C_*$ can be chosen using only the finitely many parameters $3$, $M_i/\lambda_i$ and $r_i^2Q_i/\lambda_i$. No measurability or smoothness of $V$ beyond these hypotheses is required. The preceding conditional chain comparison does not impose a sign condition on $V$ when the local comparisons are supplied independently.

## Facts & Assumptions

[F1] Compact subsets are compact in their subspace topology by [math:def-compact-space](https://alphabetamath.cc/item/def-compact-space): every relatively open cover has a finite subcover. Connected subsets admit no partition into two disjoint nonempty relatively open sets by [math:def-connected-space](https://alphabetamath.cc/item/def-connected-space).

[F2] The smooth exterior, its interior charts, the Riemannian metric and the Laplacian convention are those of [def-exterior-weighted-elliptic-data](item-def-exterior-weighted-elliptic-data). The letter $K$ here denotes the subset in the Statement, not necessarily the compact core of that definition. The sets $U_i,H_i$ and their graph are defined in the Statement; they are not required to be metric balls.

[F3] [lem-author-58255dfd955f-local-potential-harnack](item-lem-author-58255dfd955f-local-potential-harnack) applies to a nonnegative real $C^2$ pointwise solution on a coordinate ball for a smooth metric and a bounded nonnegative potential, with the displayed bounds on $A_i,q_i$. It gives a half-ball comparison constant at least one depending only on dimension, $M_i/\lambda_i$ and $r_i^2Q_i/\lambda_i$. The analytic consequence inherits its ZFC assumption, including [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice); that imported assumption is used precisely when this supplier is invoked in step 3.1. The finite-cover and finite-chain arguments themselves require no arbitrary-index choice.

## Proof

**Given:** The data and hypotheses in the Statement and [F1]–[F3].

**Goal:** The finite connected cover, conditional chain comparison and stated uniform analytic consequence.

**Proof technique:** direct.

1.1 Consider all interior chart balls centered at points of $K$ with compact closures inside their chart domains, together with their concentric half-balls. Such balls exist around every point by shrinking an interior coordinate neighborhood. The traces of these half-balls on $K$ are a relatively open cover of $K$, so [F1] supplies a finite subcover; retain the associated balls and discard any empty traces. Write $U_i,H_i$, $1\le i\le N$, for the resulting balls and half-balls. If their graph were disconnected, fix a vertex and let $I$ consist of the vertices reachable from it by finite edge sequences. Then $I$ and its complement are both nonempty, and there is no edge between them. The unions of $H_i\cap K$ over these two index sets are nonempty, relatively open, disjoint, and cover $K$. This contradicts connectedness in [F1], proving the geometric assertion. [given, F1, F2]

2.1 For $x,y\in K$, choose half-balls containing them. By step 1.1 their vertices are joined by a finite edge sequence; deleting segments between repeated vertices gives a path of $s\le N$ distinct vertices. At each edge take a point in the corresponding intersection with $K$. The resulting sequence starts at $x$, ends at $y$, and each consecutive pair lies in one of the $s$ half-balls. Applying the assumed local comparisons and multiplying gives $u(x)\le C_*^s u(y)\le C_*^N u(y)$, also when $s=1$. Taking the supremum in $x$ and then the infimum in $y$ proves the conditional bound. These extrema are finite and positive as bounded by any fixed value through the pairwise inequalities; continuity is not needed for this conditional argument. [given, step 1.1, algebra]

3.1 For the analytic family, on each fixed $U_i$ the metric is smooth, $V$ is bounded and nonnegative, $u$ is positive and $C^2$, and the pointwise equation and all three coefficient bounds are exactly those of [F3], with dimension three. Thus [F3] supplies a constant $C_i\ge1$ using only $3$, $M_i/\lambda_i$ and $r_i^2Q_i/\lambda_i$, common to all family members. Take $C_*=\max_{1\le i\le N}C_i$ and apply step 2.1. Both $N$ and these coefficient parameters are fixed, so the resulting comparison is uniform as asserted. [given, F2, F3, step 2.1] ∎
