---
title: Choosing a smooth separating regular level from an average bound
status: published
research_item: lem-author-423fe0348a31-regular-separating-level
dependency_level: 7
sources:
  references:
    - title: Liviu I. Nicolaescu, The co-area formula (2021 revision)
      url: https://metaphor.ethz.ch/x/2021/fs/401-3462-00L/sc/extras/Nicolaescu.pdf
      locator: Section 3, printed p. 8, opening definition of Hausdorff measures;
        equation (2.5), printed p. 7
      statement: The Hausdorff covering cost is multiplied by omega_r/2^r before
        taking the limit as the diameter bound tends to zero. For r=2 this
        factor is pi/4.
      hypotheses: A separable metric space and nonnegative dimension r. Here r=2 and
        the metric is the intrinsic Riemannian length metric on each component
        of the compact smooth region.
      reading_limits: Read the opening definition in Section 3 and equation (2.5) for
        the unit-ball volume. Also checked Theorem 5.3 and the
        nonnegative-weight argument for Corollary 5.4 for compatibility with the
        existing coarea supplier; no reconstruction of their proofs is claimed.
---

## Prerequisites

- [math:thm-morse-sard-for-smooth-manifolds](https://alphabetamath.cc/item/thm-morse-sard-for-smooth-manifolds)
- [math:thm-a-regular-level-set-is-an-embedded-submanifold](https://alphabetamath.cc/item/thm-a-regular-level-set-is-an-embedded-submanifold)
- [lem-author-423fe0348a31-riemannian-lipschitz-coarea](item-lem-author-423fe0348a31-riemannian-lipschitz-coarea)
- [math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold)
- [math:def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary](https://alphabetamath.cc/item/def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary)
- [math:def-embedded-smooth-submanifold-with-boundary](https://alphabetamath.cc/item/def-embedded-smooth-submanifold-with-boundary)
- [math:thm-intermediate-value](https://alphabetamath.cc/item/thm-intermediate-value)
- [math:cor-local-normal-form-for-submersions](https://alphabetamath.cc/item/cor-local-normal-form-for-submersions)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [math:thm-choice-implies-dependent-implies-countable-choice](https://alphabetamath.cc/item/thm-choice-implies-dependent-implies-countable-choice)
- [math:prop-order-and-scalar-rules-for-the-nonnegative-integral](https://alphabetamath.cc/item/prop-order-and-scalar-rules-for-the-nonnegative-integral)
- [math:cor-integral-over-a-null-set-vanishes](https://alphabetamath.cc/item/cor-integral-over-a-null-set-vanishes)
- [math:def-regular-and-critical-points-and-values](https://alphabetamath.cc/item/def-regular-and-critical-points-and-values)
- [math:def-smooth-map-between-manifolds-with-boundary](https://alphabetamath.cc/item/def-smooth-map-between-manifolds-with-boundary)
- [math:def-hausdorff-measure](https://alphabetamath.cc/item/def-hausdorff-measure)
- [def-lipschitz-cut-area-data](item-def-lipschitz-cut-area-data)
- [` Liviu I. Nicolaescu, The co-area formula (2021 revision) · Section 3, printed p. 8, opening definition of Hausdorff measures; equation (2.5), printed p. 7 `](https://metaphor.ethz.ch/x/2021/fs/401-3462-00L/sc/extras/Nicolaescu.pdf)


## Statement

Work in ZFC. Let $(R,k)$ be a compact smooth three-dimensional manifold with boundary and smooth Riemannian metric $k$. Suppose $\partial R=B_-\sqcup B_+$, where $B_-$ and $B_+$ are disjoint unions of boundary components. Let $f:R\to\mathbb R$ be smooth up to the boundary, with $f=c_-$ on $B_-$ and $f=c_+$ on $B_+$, where $c_-<a<b<c_+$. No constancy on boundary neighborhoods is assumed.

Let $A,\epsilon\in\mathbb R$. On each component of $R$, let $\mathcal H_{k,\mathrm{un}}^2$ be unnormalised Hausdorff measure for the intrinsic length metric, and set $\mathcal H_k^2=(\pi/4)\mathcal H_{k,\mathrm{un}}^2$, summing over components. This is the normalized two-dimensional metric Hausdorff cut-area convention. If $\int_a^b\mathcal H_k^2(\{x\in R:f(x)=s\})\,ds<(A+\epsilon)(b-a)$, then there is a regular value $t\in(a,b)$ of $f|_{R^\circ}$ whose full level $D=\{x\in R:f(x)=t\}$ has area at most $A+\epsilon$.

The level $D$ is a compact smooth embedded surface without boundary, possibly empty or disconnected, and meets every continuous path in $R$ from $B_-$ to $B_+$. It is nonempty whenever such a path exists. The sublevel $\Omega=\{x\in R:f(x)\le t\}$, with its induced smooth structure, is a compact embedded three-dimensional submanifold with boundary $\partial\Omega=B_-\sqcup D$.

## Facts & Assumptions

[A1] Work in ZFC, including the axiom of choice. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] Under countable choice, the critical values of a smooth map between smooth manifolds form a null set. Apply this to the boundaryless interior and target $\mathbb R$. [math:thm-morse-sard-for-smooth-manifolds](https://alphabetamath.cc/item/thm-morse-sard-for-smooth-manifolds)

[F2] A nonempty regular level of a smooth map is an embedded submanifold of the stated codimension. [math:thm-a-regular-level-set-is-an-embedded-submanifold](https://alphabetamath.cc/item/thm-a-regular-level-set-is-an-embedded-submanifold)

[F3] For a Lipschitz height constant near boundary parts exhausting the boundary, scalar coarea supplies a measurable normalized Hausdorff level-area function on intervening intervals. The supplier also shows, by bounding the gradient and integrating along curves, that a smooth function on a compact Riemannian region is Lipschitz for the intrinsic length distance on each component. [lem-author-423fe0348a31-riemannian-lipschitz-coarea](item-lem-author-423fe0348a31-riemannian-lipschitz-coarea)

[F4] A continuous real function on a closed interval takes every value between its endpoint values. [math:thm-intermediate-value](https://alphabetamath.cc/item/thm-intermediate-value)

[F5] At a submersion point, adapted coordinates put a smooth map in local projection form. [math:cor-local-normal-form-for-submersions](https://alphabetamath.cc/item/cor-local-normal-form-for-submersions)

[F6] The metric is smooth and positive definite, boundary smoothness uses half-space charts with local smooth extensions, smooth maps are continuous and have coordinate representatives smooth in the local-extension sense, and an embedded submanifold with boundary has a smooth structure making its inclusion a smooth embedding. [math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold) [math:def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary](https://alphabetamath.cc/item/def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary) [math:def-embedded-smooth-submanifold-with-boundary](https://alphabetamath.cc/item/def-embedded-smooth-submanifold-with-boundary) [math:def-smooth-map-between-manifolds-with-boundary](https://alphabetamath.cc/item/def-smooth-map-between-manifolds-with-boundary)

[F7] The axiom of choice implies countable choice, supplying the hypothesis of [F1]. [math:thm-choice-implies-dependent-implies-countable-choice](https://alphabetamath.cc/item/thm-choice-implies-dependent-implies-countable-choice)

[F8] Nonnegative integrals are monotone and positively homogeneous, and their restriction to a measurable null set vanishes. [math:prop-order-and-scalar-rules-for-the-nonnegative-integral](https://alphabetamath.cc/item/prop-order-and-scalar-rules-for-the-nonnegative-integral) [math:cor-integral-over-a-null-set-vanishes](https://alphabetamath.cc/item/cor-integral-over-a-null-set-vanishes)

[F9] A regular value is a target point all of whose fibre points are submersion points; an empty fibre is allowed. A critical value is a target point that is not regular. [math:def-regular-and-critical-points-and-values](https://alphabetamath.cc/item/def-regular-and-critical-points-and-values)

[F10] Unnormalised Hausdorff measure is the limit of infimal diameter-squared covering costs. The normalized cut-area convention here is $\mathcal H_k^2=(\pi/4)\mathcal H_{k,\mathrm{un}}^2$ on each metric component, with component measures summed. The factor is the dimension-two specialization of the cited coarea source's $\omega_r/2^r$ normalization. [math:def-hausdorff-measure](https://alphabetamath.cc/item/def-hausdorff-measure) [def-lipschitz-cut-area-data](item-def-lipschitz-cut-area-data)

## Proof

**Given:** The region, metric, boundary partition, smooth function, constants and strict average bound in the Statement, working in ZFC.

**Goal:** Choose the stated regular level and prove its area, separation and sublevel-boundary properties.

1.1 Choose $\alpha=(c_-+a)/2$ and $\beta=(b+c_+)/2$, and define $P(s)=\min\{\beta,\max\{\alpha,s\}\}$ and $v=P\circ f$. For $r\le s$, the three intervals cut out by $\alpha,\beta$ give $0\le P(s)-P(r)\le s-r$; hence $P$ is $1$-Lipschitz. By compactness the smooth gradient of $f$ is bounded, and integrating $df$ along piecewise smooth curves proves the length-Lipschitz bound used in [F3]. Thus $v$ is length-Lipschitz on each component. Continuity and the exact boundary values give neighborhoods of $B_-$ and $B_+$ on which $f<\alpha$ and $f>\beta$, respectively. On these neighborhoods $v=\alpha$ and $v=\beta$. The full boundary is exhausted by these parts, so [F3] applies to $v$ on $(a,b)$. For every $s\in(a,b)$, $\{v=s\}=\{f=s\}$, and this set lies in $R^\circ$ because the only boundary values of $f$ are $c_-$ and $c_+$. Consequently the full level-area function in the hypothesis is measurable, with the normalization fixed in [F10] and the interior interpretation supplied by coarea. [given, A1, F3, F6, F10, choose, construct, algebra]

2.1 By [A1] and [F7], [F1] applies to $f|_{R^\circ}:R^\circ\to\mathbb R$. Its regular values in $(a,b)$ therefore have full Lebesgue measure $b-a$. Put $M=A+\epsilon$; the strict hypothesis and nonnegativity of area imply $M>0$. If every regular value in $(a,b)$ had area greater than $M$, monotonicity on that full-measure set and the null-set rule in [F8] would give $\int_a^b\mathcal H_k^2(\{f=s\})\,ds\ge M(b-a)$, contrary to the hypothesis. Hence choose a regular $t\in(a,b)$ with level area at most $M$. [given, A1, F1, F7, F8, F9, step 1.1, choose, algebra]

3.1 Since $\partial R=B_-\sqcup B_+$ and $c_-<t<c_+$, $D=f^{-1}(t)$ misses all of $\partial R$. It is closed in compact $R$ and hence compact. If nonempty, it is an embedded codimension-one submanifold of $R^\circ$ by [F2], so it is a smooth surface without boundary. If empty, the empty surface has all these properties. No connectedness is required. [given, F2, F6, F9, step 2.1]

3.2 For any continuous path $\gamma:[0,1]\to R$ with $\gamma(0)\in B_-$ and $\gamma(1)\in B_+$, the function $f\circ\gamma$ is continuous with endpoint values $c_-$ and $c_+$. By [F4], it takes the value $t$, so the path meets $D$. In particular the existence of such a path implies $D\ne\varnothing$. [given, F4, F6, step 2.1]

4.1 The sublevel $\Omega=f^{-1}(( -\infty,t])$ is closed in compact $R$, so it is compact. At a point with $f<t$ it agrees locally with $R$, while points with $f>t$ have a neighborhood disjoint from it. At every point of $D\subset R^\circ$, regularity and [F5] give a smooth transverse coordinate $y_1=f-t$ (compose the projection coordinate with the inverse target chart); thus $\Omega$ has the half-space chart $y_1\le0$ and boundary $y_1=0$. Near $B_-$ it agrees with $R$ by continuity and $c_-<t$, so its boundary there is exactly the original boundary part $B_-$. Near $B_+$ it is empty by $c_+>t$. These exhaust the boundary cases. The charts are restrictions or smooth changes of the given charts, so they give the induced smooth structure and a smooth embedding into $R$. Therefore $\partial\Omega=B_-\sqcup D$, as asserted. [given, F5, F6, F9, step 2.1, step 3.1] ∎
