---
title: An exterior-contained null segment to a distant target cannot start inward
status: published
research_item: lem-author-fd27ddabb933-inward-branch-exterior-exclusion
dependency_level: 5
---

## Prerequisites

- [lem-author-fd27ddabb933-future-horizon-defining-pair](item-lem-author-fd27ddabb933-future-horizon-defining-pair)
- [lem-author-fd27ddabb933-inward-null-local-horizon-crossing](item-lem-author-fd27ddabb933-inward-null-local-horizon-crossing)
- [physics:thm-gr-local-geodesics-and-exponential-map](https://alphabetamath.cc/physics/item/thm-gr-local-geodesics-and-exponential-map)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [lem-author-fd27ddabb933-outward-graph-null-initial-jets](item-lem-author-fd27ddabb933-outward-graph-null-initial-jets)


## Statement

Work in ZFC. Use the compact spacelike surface $S$, future/outward frame $(n,\nu)$, oriented exterior wedge $\mathcal E$ and smooth spacelike section extension $(\Sigma,h)$ of the outward-graph initial-jets data. For a fixed smooth function $\phi>0$ on $S$, set $F_\epsilon(y)=\exp^h_y(\epsilon\phi(y)\nu_y)$ and $S_\epsilon=F_\epsilon(S)$. Let $n_\epsilon$ be the future unit normal of $\Sigma$ restricted to $S_\epsilon$, and let $\nu_\epsilon$ be the unit normal to $S_\epsilon$ tangent to $\Sigma$ with the outward orientation continued from $\nu$.

Choose $\epsilon>0$ sufficiently small for the inward local crossing lemma, and let $K$ and $\tau_0>0$ be its fixed compact tube and common short affine time. If a future null geodesic segment starts on $S_\epsilon$, remains entirely in the open exterior $\mathcal E$, and ends outside $K$, its initial tangent cannot be a positive multiple of the inward null normal $V_\epsilon=n_\epsilon-\nu_\epsilon$. The conclusion is specific to this sufficiently small graph family near the bifurcation surface, rather than an assertion for arbitrary outer trapped surfaces.

## Facts & Assumptions

[F1] The surface $a=0$,$b>0$ is outside the open exterior and is its local future boundary. [lem-author-fd27ddabb933-future-horizon-defining-pair](item-lem-author-fd27ddabb933-future-horizon-defining-pair)

[F2] For the sufficiently small graphs in the Statement, the ambient affine geodesics starting at $F_\epsilon(y)$ with vector $V_\epsilon(y)$ stay in the fixed compact tube $K$ for $0\le\lambda\le\tau_0$ and cross $a=0,b>0$ at a parameter $\lambda_*\le C\epsilon<\tau_0$. [lem-author-fd27ddabb933-inward-null-local-horizon-crossing](item-lem-author-fd27ddabb933-inward-null-local-horizon-crossing)

[F3] Affine geodesics with the same initial data are unique on their common interval, and positive affine rescaling obeys $\gamma_{p,cV}(t)=\gamma_{p,V}(ct)$ for $c>0$. [physics:thm-gr-local-geodesics-and-exponential-map](https://alphabetamath.cc/physics/item/thm-gr-local-geodesics-and-exponential-map)

[F4] The oriented defining-pair data and smooth spacelike section extension supply the graph family $F_\epsilon(y)=\exp^h_y(\epsilon\phi(y)\nu_y)$ for fixed smooth $\phi>0$, its future unit normal $n_\epsilon$, and its smooth outward unit graph normal $\nu_\epsilon$. The vector $V_\epsilon=n_\epsilon-\nu_\epsilon$ is its specified unhalved future inward null normal, and the sufficiently small positive graphs lie in $\mathcal E$. [lem-author-fd27ddabb933-outward-graph-null-initial-jets](item-lem-author-fd27ddabb933-outward-graph-null-initial-jets)

[A1] Work in ZFC, including the countable and dependent choice required by the invoked geodesic, compactness and causal interfaces. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

## Proof

**Given:** The assumptions in the Statement.

**Goal:** Exclude the inward initial ray for the stated exterior-contained segment.

1.1 Suppose the initial tangent were $cV_\epsilon(y)$ with $c>0$. By [F3], rescale the affine parameter positively so that the initial tangent is exactly the vector $V_\epsilon(y)$ specified in [F4], and let $\ell$ be the rescaled segment length. Uniqueness identifies this segment with the ambient geodesic in [F2] on $[0,\min\{\ell,\tau_0\}]$. If $\ell\le\tau_0$, its endpoint lies in $K$ by [F2], contrary to the given target condition. Thus $\ell>\tau_0$. [F2, F3, F4, given, algebra]

2.1 The segment therefore contains the crossing supplied by [F2], at $\lambda_*<\tau_0$. That point has $a=0$ and $b>0$ and hence does not belong to the open exterior by [F1]. This contradicts the assumed exterior containment of the segment and excludes the inward initial ray. No global claim about causal escape after crossing the horizon is needed. [F1, F2, step 1.1, contradiction] ∎
