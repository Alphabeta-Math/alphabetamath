---
title: Shifting a temporal function permits a controlled compact restriction
status: published
research_item: lem-author-3bd197b76c61-positive-temporal-compact-restriction
dependency_level: 6
---

## Prerequisites

- [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)
- [thm-maximal-normal-angle-estimate-input](item-thm-maximal-normal-angle-estimate-input)
- [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)
- [lem-author-89004136b63c-compact-neighborhood-localization](item-lem-author-89004136b63c-compact-neighborhood-localization)
- [math:thm-extreme-value-metric](https://alphabetamath.cc/item/thm-extreme-value-metric)
- [lem-author-89004136b63c-compact-temporal-persistence](item-lem-author-89004136b63c-compact-temporal-persistence)
- [lem-author-89004136b63c-uniform-inverse-metric-continuity](item-lem-author-89004136b63c-uniform-inverse-metric-continuity)
- [physics:def-gr-inverse-metric-and-musical-isomorphisms](https://alphabetamath.cc/physics/item/def-gr-inverse-metric-and-musical-isomorphisms)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [math:def-smooth-manifold](https://alphabetamath.cc/item/def-smooth-manifold)
- [math:def-topological-manifold-without-boundary](https://alphabetamath.cc/item/def-topological-manifold-without-boundary)
- [math:thm-compact-subset-of-a-hausdorff-space-is-closed](https://alphabetamath.cc/item/thm-compact-subset-of-a-hausdorff-space-is-closed)
- [math:def-subspace-topology-top](https://alphabetamath.cc/item/def-subspace-topology-top)
- [math:thm-closed-subspace-of-a-compact-space-is-compact](https://alphabetamath.cc/item/thm-closed-subspace-of-a-compact-space-is-compact)
- [math:def-compact-space](https://alphabetamath.cc/item/def-compact-space)
- [math:thm-compactness-agrees-with-metric-compactness](https://alphabetamath.cc/item/thm-compactness-agrees-with-metric-compactness)


## Statement

Work in ZFC, including the Axiom of Choice.

Let $g_j$ be smooth time-oriented Lorentz metrics of signature $(-,+,+,+)$ on a common smooth four-manifold, converging in $C^2$ near a nonempty compact ambient set $Q$ to a time-oriented Lorentz metric $g_*$. Assume the time orientations are compatible near $Q$: a fixed continuous field $Z$ is future timelike for $g_*$ and for every sufficiently large $j$ for $g_j$. Let a fixed smooth $\tau$ have past timelike $g_*$-gradient near $Q$. Let $M_j\subset Q$ be compact smooth $g_j$-spacelike maximal hypersurfaces, smooth up to their actual boundaries, with future unit normals $n_j$ whose coordinate components on $\partial M_j$ are uniformly bounded in a fixed finite coordinate cover near $Q$.

For all sufficiently large $j$, $\operatorname{grad}_{g_j}\tau$ is past timelike on $Q$ and its norm $\alpha_j=\sqrt{-g_j^{-1}(d\tau,d\tau)}$ has a uniform positive lower bound. After shifting $s=\tau+1-\min_Q\tau$, one has $1\le s\le T=1+\max_Q\tau-\min_Q\tau$ on $Q$. The entire nonnegative-$s$ portion of each $M_j$ is exactly $M_j$, and the temporal weighted-normal theorem gives a uniform bound for $-g_j(n_j,-\operatorname{grad}_{g_j}\tau)$ on all of $M_j$. In particular it applies to compact restrictions with controlled artificial cuts, provided those cuts are retained as actual boundaries.

## Facts & Assumptions

[A1] Work in ZFC, including the Axiom of Choice, as required by the weighted normal theorem [F1]. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] The weighted normal theorem, including its actual-boundary term and geometric coefficient hypotheses, is [thm-maximal-normal-angle-estimate-input](item-thm-maximal-normal-angle-estimate-input).

[F2] Smooth spacelike maximality, normals and induced conventions are [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data). The stated compactness and coordinate bound on boundary normals are hypotheses of this lemma, not consequences of merely having a local temporal function.

[F3] The temporal-function and time-orientation conventions are [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data); in particular a timelike metric gradient is past directed relative to $Z$ exactly when $d\tau(Z)>0$.

[F4] Finite compact chart pieces covering $Q$ are supplied by [lem-author-89004136b63c-compact-neighborhood-localization](item-lem-author-89004136b63c-compact-neighborhood-localization). After restricting these pieces to $Q$ as justified in step 1.1, [math:thm-extreme-value-metric](https://alphabetamath.cc/item/thm-extreme-value-metric) applies to each nonempty compact coordinate image and each continuous real function on it. Taking the finitely many extrema on these restricted pieces gives extrema attained in $Q$.

[F5] The compact temporal covector $d\tau$ persists with its orientation relative to $Z$ under metric perturbation by [lem-author-89004136b63c-compact-temporal-persistence](item-lem-author-89004136b63c-compact-temporal-persistence). Uniform convergence of the inverse coefficients on compact chart pieces is supplied by [lem-author-89004136b63c-uniform-inverse-metric-continuity](item-lem-author-89004136b63c-uniform-inverse-metric-continuity).

[F6] The inverse metric and musical isomorphisms are [physics:def-gr-inverse-metric-and-musical-isomorphisms](https://alphabetamath.cc/physics/item/def-gr-inverse-metric-and-musical-isomorphisms). In particular, $\operatorname{grad}_g\tau=(d\tau)^{\sharp_g}$, so $g(\operatorname{grad}_g\tau,X)=d\tau(X)$ and $g(\operatorname{grad}_g\tau,\operatorname{grad}_g\tau)=g^{-1}(d\tau,d\tau)$.

[F7] A smooth manifold has an underlying Hausdorff topological manifold. [math:def-smooth-manifold](https://alphabetamath.cc/item/def-smooth-manifold) [math:def-topological-manifold-without-boundary](https://alphabetamath.cc/item/def-topological-manifold-without-boundary) Every compact subset of a Hausdorff space is closed. [math:thm-compact-subset-of-a-hausdorff-space-is-closed](https://alphabetamath.cc/item/thm-compact-subset-of-a-hausdorff-space-is-closed) Closed sets in a subspace are traces of ambient closed sets, and restrictions of continuous maps are continuous. [math:def-subspace-topology-top](https://alphabetamath.cc/item/def-subspace-topology-top) A closed subspace of a compact space is compact. [math:thm-closed-subspace-of-a-compact-space-is-compact](https://alphabetamath.cc/item/thm-closed-subspace-of-a-compact-space-is-compact) Compactness has its intrinsic finite-open-subcover meaning. [math:def-compact-space](https://alphabetamath.cc/item/def-compact-space) For a metric space with its metric topology this agrees with metric compactness, including for subspaces. [math:thm-compactness-agrees-with-metric-compactness](https://alphabetamath.cc/item/thm-compactness-agrees-with-metric-compactness)

## Proof

**Given:** ZFC including the Axiom of Choice, and the sequence, compatible time orientations, nonempty compact ambient set, temporal function and boundary-normal bound. **Goal:** Verify every localization hypothesis of the weighted theorem and the uniform raw temporal-gradient bound.

1.1 Use [F4] to refine the given coordinate cover to finitely many compact chart pieces $C_\ell$ covering $Q$. The ambient smooth manifold is Hausdorff by [F7], so its compact subset $Q$ is closed. Set $K_\ell=C_\ell\cap Q$. By [F7], $K_\ell$ is closed in compact $C_\ell$ and hence compact. Discard empty intersections; the remaining $K_\ell$ still cover nonempty $Q$ and are all subsets of $Q$. Each restricted chart is a homeomorphism onto its coordinate image: an open cover of that image pulls back to an open cover of $K_\ell$, whose finite subcover pushes forward to a finite subcover of the image. Thus the coordinate images are compact, and [F7] identifies their Euclidean metric subspaces as compact metric spaces. Restrictions of continuous real functions remain continuous by [F7]. Applying [F4] on each such image and then taking the minimum and maximum of the finitely many attained extrema gives the extrema on $Q$, attained at points of $Q$. The continuous positive function $h_*=-g_*^{-1}(d\tau,d\tau)$ therefore has $0<m=\min_Q h_*\le\max_Q h_*=M<\infty$. The fixed derivatives of $\tau$ are bounded on these pieces. By [F5], metric convergence gives uniform inverse-metric convergence, hence $h_j=-g_j^{-1}(d\tau,d\tau)\to h_*$ uniformly on $Q$. For late $j$, $m/2\le h_j\le M+1$, so $a_0=\sqrt{m/2}\le\alpha_j\le a_1=\sqrt{M+1}$. Moreover [F3] gives $d\tau(Z)>0$, and the persistence lemma in [F5], applied to $(g_*,Z,d\tau,Q)$, identifies these timelike gradients as past directed relative to $Z$. The common orientation hypothesis makes this precisely the orientation used for the future normals $n_j$. [F3, F4, F5, F6, F7, given, algebra]

2.1 By [F4], the fixed smooth function $\tau$ attains finite extrema on nonempty $Q$. Thus $s=\tau+1-\min_Q\tau$ satisfies $1\le s\le T=1+\max_Q\tau-\min_Q\tau$, with $ds=d\tau$. Put $V_j=-\alpha_j^{-1}\operatorname{grad}_{g_j}\tau$ and $v_j=-g_j(n_j,V_j)$. By [F3] and step 1.1, $V_j$ is future unit timelike. Uniform inverse-metric bounds, fixed first derivatives of $\tau$ and $\alpha_j\ge a_0$ bound its coordinate components. The assumed component bounds for $n_j$ on every actual $\partial M_j$, together with the uniform metric bounds, give a common $B\ge1$ with $v_j\le B$ there. On the same finite compact cover, metric $C^2$, inverse-metric $C^0$ and fixed shifted-function $C^3$ norms are uniformly bounded. [F2, F3, F4, F5, F6, given, step 1.1, algebra]

3.1 Apply [F1] under [A1] with temporal function $s$ to $M_j$ itself, using the common time orientation and the smooth actual boundary from the hypotheses. Its entire nonnegative portion is compact and contained in $Q$, since $s\ge1$ on $M_j\subset Q$. The coefficient and temporal-norm hypotheses follow from steps 1.1 and 2.1. With the common exponent $\mu>4$, the theorem gives $\sup_{M_j}s^\mu v_j\le2\max\{2T^\mu,T^\mu B\}=:C$. Its boundary supremum is bounded by $T^\mu B$, or is zero when the boundary is empty. Since $s\ge1$, $v_j\le C$ throughout $M_j$, and $-g_j(n_j,-\operatorname{grad}_{g_j}\tau)=\alpha_jv_j\le a_1 C$. For a compact restriction the same argument includes every artificial cut in the actual boundary and uses its assumed normal bound. This proves all the assertions. [A1, F1, F2, F3, F6, step 1.1, step 2.1, algebra] ∎
