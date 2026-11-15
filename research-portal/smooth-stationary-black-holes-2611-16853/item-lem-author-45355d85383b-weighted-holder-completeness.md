---
title: Weighted Hölder spaces and their Dirichlet kernels are Banach
status: published
research_item: lem-author-45355d85383b-weighted-holder-completeness
dependency_level: 2
---

## Prerequisites

- [def-weighted-holder-spaces](item-def-weighted-holder-spaces)
- [def-exterior-weighted-elliptic-data](item-def-exterior-weighted-elliptic-data)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [math:def-norm-and-normed-space](https://alphabetamath.cc/item/def-norm-and-normed-space)
- [math:def-banach-space](https://alphabetamath.cc/item/def-banach-space)
- [math:thm-uniform-cauchy-criterion-real-functions](https://alphabetamath.cc/item/thm-uniform-cauchy-criterion-real-functions)
- [math:thm-uniform-limit-continuous-real-functions](https://alphabetamath.cc/item/thm-uniform-limit-continuous-real-functions)
- [math:thm-uniform-derivative-limit-on-a-closed-interval](https://alphabetamath.cc/item/thm-uniform-derivative-limit-on-a-closed-interval)
- [math:thm-symmetry-of-higher-mixed-partials](https://alphabetamath.cc/item/thm-symmetry-of-higher-mixed-partials)
- [math:thm-chain-rule-for-total-derivatives](https://alphabetamath.cc/item/thm-chain-rule-for-total-derivatives)
- [math:cor-mean-value-theorem](https://alphabetamath.cc/item/cor-mean-value-theorem)
- [math:thm-connected-subsets-of-r-are-intervals](https://alphabetamath.cc/item/thm-connected-subsets-of-r-are-intervals)
- [math:thm-extreme-value-metric](https://alphabetamath.cc/item/thm-extreme-value-metric)
- [math:lem-closed-subspace-of-a-banach-space-is-banach](https://alphabetamath.cc/item/lem-closed-subspace-of-a-banach-space-is-banach)


## Statement

For the fixed smooth exterior and fixed chart data, $C^{k,\alpha}_\beta$ is complete. For $k\ge0$, restriction to the compact boundary is continuous into $C^0(S)$, and the subspace with zero trace is closed and complete. In particular $X_\beta=\{w\in C^{4,\alpha}_\beta:w|_S=0\}$ and $Y_\beta=C^{2,\alpha}_{\beta-2}$ are real Banach spaces.

## Facts & Assumptions

[F1] The finite-valued weighted space, its fixed compact chart subsets $K_i$ covering $K$, its end annuli $A_R$, and its norm are those of the weighted-space definition. Its Justification establishes the norm axioms and the real vector-space structure. [def-weighted-holder-spaces](item-def-weighted-holder-spaces)

[F2] The exterior is smooth with compact boundary $S$ contained in the compact core; boundary derivatives mean continuous extensions from the interior. The Dirichlet and target spaces are $X_\beta=\{w\in C^{4,\alpha}_\beta:w|_S=0\}$ and $Y_\beta=C^{2,\alpha}_{\beta-2}$. [def-exterior-weighted-elliptic-data](item-def-exterior-weighted-elliptic-data)

[F3] Retain the ambient ZFC convention, including Choice. The sequential limits below use the supplied real completeness results; no additional choice principle is introduced. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F4] All vector operations are pointwise over $\mathbb R$; a Banach space is a normed real vector space in which every norm-Cauchy sequence converges. Here $C^0(S)$ denotes the continuous functions $S\to\mathbb R$, equipped with $\|v\|_{\infty,S}=\sup_{p\in S}|v(p)|$ and its induced metric; for $S=\varnothing$ this is the zero space with zero norm. [math:def-norm-and-normed-space](https://alphabetamath.cc/item/def-norm-and-normed-space) [math:def-banach-space](https://alphabetamath.cc/item/def-banach-space)

[F5] A uniformly Cauchy sequence of real-valued functions on any set has a uniform limit, and a uniform limit of continuous real-valued functions on a metric space is continuous. [math:thm-uniform-cauchy-criterion-real-functions](https://alphabetamath.cc/item/thm-uniform-cauchy-criterion-real-functions) [math:thm-uniform-limit-continuous-real-functions](https://alphabetamath.cc/item/thm-uniform-limit-continuous-real-functions)

[F6] On a closed nondegenerate interval, continuously differentiable functions whose derivatives converge uniformly and whose values converge at one point converge to a differentiable function with that derivative limit. Continuous higher partial derivatives can be permuted. We apply the interval result only to segments strictly inside coordinate domains. [math:thm-uniform-derivative-limit-on-a-closed-interval](https://alphabetamath.cc/item/thm-uniform-derivative-limit-on-a-closed-interval) [math:thm-symmetry-of-higher-mixed-partials](https://alphabetamath.cc/item/thm-symmetry-of-higher-mixed-partials)

[F7] Smooth coordinate changes satisfy the chain rule; iteration expresses derivatives through a fixed order as finite linear combinations of derivatives in the other chart with smooth coefficients. The mean value theorem bounds scalar increments along interior coordinate segments by the segment length times a derivative bound. Boundary versions of these identities follow by continuity of the extended derivative fields. [math:thm-chain-rule-for-total-derivatives](https://alphabetamath.cc/item/thm-chain-rule-for-total-derivatives) [math:cor-mean-value-theorem](https://alphabetamath.cc/item/cor-mean-value-theorem)

[F8] A closed interval is connected. A continuous real-valued function on a nonempty compact metric space is bounded, so this applies to the functions on $S$ and to the finitely many smooth coordinate-transition coefficients on compact overlaps. Empty sets need no boundedness assertion. [math:thm-connected-subsets-of-r-are-intervals](https://alphabetamath.cc/item/thm-connected-subsets-of-r-are-intervals) [math:thm-extreme-value-metric](https://alphabetamath.cc/item/thm-extreme-value-metric)

[F9] A closed linear subspace of a Banach space, with the restricted norm, is Banach. [math:lem-closed-subspace-of-a-banach-space-is-banach](https://alphabetamath.cc/item/lem-closed-subspace-of-a-banach-space-is-banach)

## Proof

**Given:** The fixed exterior and chart data, an integer $k\ge0$, $0<\alpha<1$, a real $\beta$, and the ambient ZFC convention in [F3].

**Goal:** Prove completeness of the weighted norm, continuity of boundary restriction, and completeness of its zero-trace kernel.

1.1 Let $\|\cdot\|_\beta$ abbreviate the stated weighted norm for the fixed $k,\alpha,\beta$. Sums and real multiples preserve local $C^{k,\alpha}$ regularity, and the termwise triangle and homogeneity inequalities preserve finiteness of this norm. If the norm is zero, the order-zero suprema on the core and annuli force the function to vanish everywhere, since these sets cover the exterior. Thus the space is a real normed vector space, as already justified in [F1]. Compactness makes $\|v\|_{\infty,S}$ finite for every $v\in C^0(S)$; the absolute-value inequalities and pointwise separation give its norm axioms, including the specified empty-boundary case. [F1, F2, F4, F8, algebra]

1.2 Let $(w_n)$ be Cauchy in $\|\cdot\|_\beta$. Each coordinate derivative through order $k$ is uniformly Cauchy on every $K_i$ and every fixed $A_R$, since its fixed positive coefficient in the norm can be divided out. The same holds on any sufficiently small compact coordinate ball or boundary half-ball $B$: cover its part in the core by the finitely many $K_i$, cover the remaining part by finitely many compact end patches lying in annuli, and express all derivatives in the coordinates of $B$ using [F7]. The transition coefficients are bounded on the compact intersections by [F8], giving a bound $\max_{|I|\le k}\sup_B|\partial^I(w_n-w_m)|\le C_B\|w_n-w_m\|_\beta$ with $C_B$ independent of $n,m$. By [F5] these derivative fields converge uniformly on $B$ to continuous fields $v_I$. The order-zero limits define a single function $w$ because they are limits of the same scalar values on overlaps. [F1, F2, F3, F5, F7, F8, given]

2.1 On each closed coordinate segment strictly inside a chart, apply [F6] to $\partial^I w_n$ and its derivative in a coordinate direction whenever $|I|<k$. The value at any fixed point converges by step 1.2, and the derivative converges uniformly there by the same step; the mixed-partial identity in [F6] identifies that derivative with the corresponding canonical multi-index derivative. Induction on the order gives $v_I=\partial^I w$ in the interior. Their continuous uniform limits on boundary half-balls supply the required extensions to the boundary. Taking limits in the coordinate-change identities shows that these derivatives agree on overlaps. For $k=0$ only the continuous order-zero limit is needed. [step 1.2, F2, F5, F6, F7]

3.1 A Cauchy sequence is bounded in norm: fix a tail whose distances to one term are at most one and include the finitely many preceding norms. Passing this bound to the limit in each top-order Hölder quotient gives finite Hölder bounds for the extended derivatives of $w$ on each $K_i$ and each fixed annulus. These bounds also give local Hölder regularity in any sufficiently small compact convex coordinate half-ball $B$, even if the compact $K_i$ have not been chosen with interiors covering the core. Indeed their intersections with $B$, together with finitely many compact end patches inside annuli, give a finite closed cover $E_1,\ldots,E_N$ of $B$. In the coordinates of $B$, [F7] transfers the top-order Hölder bounds to each $E_i$: its smooth coefficients are bounded and Lipschitz on the relevant compact overlaps, while lower-order derivatives of $w$ are Lipschitz on $B$ by their bounded first derivatives and [F7]. For two points of $B$, restrict this cover to their joining segment. By connectedness in [F8], the sets containing the endpoints can be joined by a chain of intersecting cover sets, using at most $N$ sets; otherwise the finite unions of the two groups would disconnect that segment. Choose intersection points on the segment and telescope their value differences. Each difference is bounded by $H$ times the segment length to the power $\alpha$, where $H$ is the maximum of the finitely many bounds on the $E_i$, so the total is at most $NH$ times that power. Thus $w$ is locally $C^{k,\alpha}$ up to the boundary in the specified convention. [step 1.2, step 2.1, F1, F2, F7, F8, algebra]

4.1 Given $\varepsilon>0$, choose $J$ so that $\|w_n-w_m\|_\beta\le\varepsilon$ for $n,m\ge J$. Fix $n\ge J$ and a radius $R$. Each derivative supremum and Hölder seminorm of $w_n-w$ is at most the lower limit of the corresponding quantity for $w_n-w_m$: every pointwise value or two-point quotient converges by steps 1.2 and 2.1, and one then takes the supremum. Finite nonnegative sums and maxima preserve this lower-limit inequality. Consequently $N_K(w_n-w)$ plus the entire weighted annular expression at this fixed $R$ is at most $\varepsilon$. Taking the supremum over $R$ yields $\|w_n-w\|_\beta\le\varepsilon$. Step 3.1 supplies the local regularity, and $\|w\|_\beta\le\|w_n\|_\beta+\varepsilon<\infty$ supplies membership in the weighted space. This proves completeness and hence the Banach property. [step 1.1, step 1.2, step 2.1, step 3.1, F1, F4, choose, algebra]

5.1 For every $w$ in the space, its boundary extension is continuous and $\|w|_S\|_{\infty,S}\le N_K(w)\le\|w\|_\beta$, since the $K_i$ cover $S$ and include the order-zero suprema. Thus restriction is a continuous linear map into the normed space $C^0(S)$ defined in [F4]. Its zero-trace kernel is a linear subspace. If $v$ is outside that kernel, some $p\in S$ has $v(p)\ne0$; every $u$ with $\|u-v\|_\beta<|v(p)|/2$ still has $u(p)\ne0$. The complement is therefore open and the kernel is closed, including the case $S=\varnothing$, when the kernel is the whole space. Applying [F9] to the Banach space established in step 4.1 makes this kernel complete for its restricted norm. Taking $k=4$ gives $X_\beta$ and taking $k=2$ with weight $\beta-2$ gives $Y_\beta$ as real Banach spaces. [step 1.1, step 4.1, F1, F2, F4, F9, algebra] ∎
