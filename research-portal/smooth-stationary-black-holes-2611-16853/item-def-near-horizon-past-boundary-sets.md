---
title: Compact remainder, causal cut and generator endpoint map
status: published
research_item: def-near-horizon-past-boundary-sets
dependency_level: 5
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF pp. 24–25, Lemma 4.3 and paragraph preceding Lemma 4.4
      statement: The article defines the remainder K, its relative boundary D, and the
        set A of points of the comparison sphere whose past null geodesics reach
        D, with the endpoint map F.
      hypotheses: The stationary section and causal-boundary setting of Section 4; the
        citation is attribution for the article notation.
      reading_limits: The frozen extracted article text on these pages was read; the
        rendered PDF and the proofs of the surrounding lemmas were not
        independently checked for this definition.
---

PDF p. 24: ` Lemma 4.3 notation `; PDF p. 25: ` paragraph before Lemma 4.4 `

## Prerequisites

- [def-stationary-section-time](item-def-stationary-section-time)
- [def-coordinate-comparison-spheres](item-def-coordinate-comparison-spheres)
- [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)
- [def-null-screen-expansion-and-focal-data](item-def-null-screen-expansion-and-focal-data)
- [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)
- [math:def-riemannian-distance-on-a-connected-manifold](https://alphabetamath.cc/item/def-riemannian-distance-on-a-connected-manifold)
- [math:lem-extended-reals-complete](https://alphabetamath.cc/item/lem-extended-reals-complete)


## Definition

Fix a sufficiently small $q>0$ and use the supplied stationary section data, writing $\Sigma=\Sigma_{q,0}$, $\Sigma^\circ=\Sigma\setminus S$, and $v=v_q$. Thus $\Sigma^\circ$ is the level set $v=0$ and has induced Riemannian metric $h_q$. Assume that $\Sigma$ is a connected smooth Riemannian manifold with boundary $S$, with metric extending $h_q$ to the boundary. Let $\rho:\Sigma\to[0,+\infty]$ be given by $\rho(x)=\inf_{y\in S}d_{h_q}(x,y)$, with the infimum taken in the extended real line and $\inf\varnothing=+\infty$. Here $d_{h_q}$ is intrinsic distance on $\Sigma$. Define $S_\eta=\{x\in\Sigma:\rho(x)=\eta\}$ for finite $\eta>0$. If $S\ne\varnothing$, then $\rho$ is the usual finite nonnegative boundary distance; if $S=\varnothing$, then $\rho\equiv+\infty$ and $S_\eta=\varnothing$.

Use the comparison sphere $C=C_q$, its stationary translate $C_t$, and the stationary cylinder $\mathscr C$. Supply the closed region $B\subset\Sigma$ described as the portion inside $\mathscr C$, including $S$; the choice of inside is part of the data. All chronological relations are relative to the exterior $\mathcal E$ with metric $g_q$: $I^-_{\mathcal E}(C_t)$ consists of points joined to a point of $C_t$ by a future-directed timelike curve in $\mathcal E$. Define $K=B\setminus I^-_{\mathcal E}(C_t)$, regarding $S$ as disjoint from this subset of $\mathcal E$, and define $D=\partial_{\Sigma^\circ}(K\cap\Sigma^\circ)$, the boundary in the topology of $\Sigma^\circ$.

For the endpoint construction, assume $v$ is temporal on $\mathcal E$, meaning its differential is positive on every nonzero future-directed causal vector. Assume $C_t$ is a spacelike two-surface with a specified outward future null normal direction at each point, and supply for each $c\in C_t$ a past-directed affinely parametrized null geodesic $\gamma_c$ starting at $c$ in the opposite direction, on an interval containing zero and staying in $\mathcal E$ on the portion considered. Here a null geodesic has nonzero null tangent and zero covariant acceleration; its affine parameter increases toward the past. Put $A=\{c\in C_t:\gamma_c\text{ meets }D\}$, and for $c\in A$ define $F(c)$ to be its point of intersection with $D$. Once $t$ is fixed, $C_t$ may be denoted by $C$. No compactness, coverage of $D$, smoothness, or area property of these sets or of $F$ is asserted by these definitions.

## Definition references

[def-stationary-section-time](item-def-stationary-section-time)

[def-coordinate-comparison-spheres](item-def-coordinate-comparison-spheres)

[def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)

[def-null-screen-expansion-and-focal-data](item-def-null-screen-expansion-and-focal-data)

[def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[math:def-riemannian-distance-on-a-connected-manifold](https://alphabetamath.cc/item/def-riemannian-distance-on-a-connected-manifold)

[math:lem-extended-reals-complete](https://alphabetamath.cc/item/lem-extended-reals-complete)

## Facts & Assumptions

[F1] The stationary section interface supplies $\Sigma^\circ=\{v=0\}$, its induced metric, and the convention that causal relations use $g_q$ on $\mathcal E$. [def-stationary-section-time](item-def-stationary-section-time) [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[F2] The comparison-sphere interface supplies $C_t$ and its stationary cylinder; the inside region is separately specified above. [def-coordinate-comparison-spheres](item-def-coordinate-comparison-spheres)

[F3] Chronological past is defined by future-directed timelike reachability in the specified manifold, and a relative boundary is closure minus interior in its specified topology. [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)

[F4] The intrinsic distance is the infimum of lengths of piecewise smooth connecting curves on the connected Riemannian manifold with boundary. [math:def-riemannian-distance-on-a-connected-manifold](https://alphabetamath.cc/item/def-riemannian-distance-on-a-connected-manifold)

[F5] Null normal directions and affine null geodesics use the stated Lorentzian conventions; a temporal differential is positive on future causal vectors. [def-null-screen-expansion-and-focal-data](item-def-null-screen-expansion-and-focal-data) [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)

[F6] Every subset of the extended real line has an infimum there, with $\inf\varnothing=+\infty$; for a nonempty real set bounded below this agrees with its real infimum. [math:lem-extended-reals-complete](https://alphabetamath.cc/item/lem-extended-reals-complete)

## Justification

**Given:** The section, boundary metric, inside region, temporal function and chosen geodesic family in the Definition.

**Goal:** Verify that the displayed sets and endpoint map are unambiguously defined.

1.1 For each $x\in\Sigma$, the set $\{d_{h_q}(x,y):y\in S\}$ consists of finite nonnegative reals. If $S\ne\varnothing$, this set is nonempty and bounded below by zero, so its extended-real infimum agrees with its real infimum and is finite, bounded above by $d_{h_q}(x,y_0)$ for any fixed $y_0\in S$. If $S=\varnothing$, its extended-real infimum is $+\infty$, so every finite level set $S_\eta$ is empty. This defines $\rho:\Sigma\to[0,+\infty]$ and all the displayed level sets without a nonempty-boundary assumption. The specified inside region and chronological past determine $K$; taking closure minus interior in $\Sigma^\circ$ determines $D$, including if either set is empty. [given, F1, F2, F3, F4, F6]

2.1 Along each past-directed null geodesic, $v$ strictly decreases as its affine parameter increases, because its tangent is the negative of a future-directed causal vector and $dv$ is positive on such vectors. Consequently the geodesic meets the level set $\Sigma^\circ=\{v=0\}$ at most once. Since $D\subset\Sigma^\circ$, every $c\in A$ has exactly one intersection point with $D$, so $F:A\to D$ is a function. This argument assumes the displayed family and does not prove its existence or that every point of $D$ is reached. [F1, F5, step 1.1] ∎
