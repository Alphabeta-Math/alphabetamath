---
title: Riemannian Lipschitz coarea on compact interior bands
status: published
research_item: lem-author-423fe0348a31-riemannian-lipschitz-coarea
dependency_level: 6
sources:
  references:
    - title: The co-area formula
      url: https://metaphor.ethz.ch/x/2021/fs/401-3462-00L/sc/extras/Nicolaescu.pdf
      locator: Liviu I. Nicolaescu, Theorem 5.3 and Corollary 5.4, pp. 14–15; Lemma
        1.1, p. 3; Section 3, p. 8
      statement: For a Lipschitz map from a C1 Riemannian manifold of dimension n+k to
        one of dimension k, integration of the metric Jacobian over a measurable
        set equals integration of the n-dimensional Hausdorff measures of its
        fibers. The corresponding weighted formula holds for nonnegative
        measurable weights, including the extended nonnegative case.
      hypotheses: Manifolds without boundary with their Riemannian distances; a
        Lipschitz map and a measurable set or nonnegative measurable weight.
        Hausdorff measures use the source's Euclidean-volume normalization. The
        present application is componentwise on the interior of a smooth
        three-region, with real-valued map.
      reading_limits: Read the theorem and corollary statements and the corollary's
        monotone-convergence argument, the Jacobian definition, and the
        normalization material at the indicated locations. The full proof of the
        theorem was not reconstructed.
---

## Prerequisites

- [lem-author-423fe0348a31-scalar-metric-jacobian](item-lem-author-423fe0348a31-scalar-metric-jacobian)
- [lem-author-423fe0348a31-interior-coarea-boundary-treatment](item-lem-author-423fe0348a31-interior-coarea-boundary-treatment)
- [def-lipschitz-cut-area-data](item-def-lipschitz-cut-area-data)
- [math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [` The co-area formula · Liviu I. Nicolaescu, Theorem 5.3 and Corollary 5.4, pp. 14–15; Lemma 1.1, p. 3; Section 3, p. 8 `](https://metaphor.ethz.ch/x/2021/fs/401-3462-00L/sc/extras/Nicolaescu.pdf)


## Statement

Let $(R,k)$ be a compact smooth Riemannian three-region with boundary, and let $u:R\to\mathbb R$ be Lipschitz for its intrinsic length distance. Suppose that $u$ is constant near each of two boundary parts whose union is $\partial R$, with the two constants outside an interval $I$ on opposite sides. For every Borel interval $J\subset I$,

$$\int_{\{x\in R:u(x)\in J\}}|\nabla_k u|\,dV_k=\int_J\mathcal H_k^2(\{x\in R:u(x)=t\})\,dt.$$

Here $dV_k$ is Riemannian volume, $\nabla_k u$ is the almost-everywhere weak gradient characterized by $k(\nabla_k u,\cdot)=du$, and $\mathcal H_k^2$ is normalized two-dimensional Hausdorff measure for the metric. A smooth $u$ satisfying the same boundary condition also satisfies the identity. More generally, for any nonnegative measurable $w$ on $R^\circ$,

$$\int_{R^\circ}w|\nabla_k u|\,dV_k=\int_{\mathbb R}\left(\int_{\{x\in R^\circ:u(x)=t\}}w\,d\mathcal H_k^2\right)dt.$$

Both sides are extended nonnegative integrals. Level area here is Hausdorff area; it is not defined to be BV perimeter.

## Statement references

[lem-author-423fe0348a31-interior-coarea-boundary-treatment](item-lem-author-423fe0348a31-interior-coarea-boundary-treatment)

[def-lipschitz-cut-area-data](item-def-lipschitz-cut-area-data)

[math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold)

## Facts & Assumptions

[A1] Work in ZFC, including the axiom of choice. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] The metric supplies intrinsic curve length and Riemannian volume. [math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold)

[F2] The Lipschitz height has almost-everywhere weak gradient and normalized Hausdorff cut-area conventions as stated above. [def-lipschitz-cut-area-data](item-def-lipschitz-cut-area-data)

[F3] At almost every point the scalar metric coarea Jacobian is $|\nabla_k u|$. [lem-author-423fe0348a31-scalar-metric-jacobian](item-lem-author-423fe0348a31-scalar-metric-jacobian)

[F4] The boundary has zero three-dimensional volume, levels in $I$ miss it, and the restriction of $u$ to each interior component is Lipschitz for that component's length distance. [lem-author-423fe0348a31-interior-coarea-boundary-treatment](item-lem-author-423fe0348a31-interior-coarea-boundary-treatment)

[F5] The Riemannian Lipschitz coarea formula and its nonnegative weighted form are the independent inputs recorded below.

## Proof

**Given:** The region, metric, height, boundary constants and interval in the Statement.

**Goal:** Prove the band and weighted identities, including the smooth-height case.

1.1 Apply the cited coarea formula to $u$ on each connected component of $R^\circ$, with target $\mathbb R$ and dimensions three and one. By the boundary-treatment result the restriction is Lipschitz for the component distance; the scalar Jacobian is $|\nabla_k u|$ almost everywhere. The source's full-dimensional Hausdorff measures are Riemannian volume and Lebesgue measure under its normalization. Summing over the countably many components gives the weighted identity, with nonnegative integrals interpreted in the extended sense. [given, A1, F1, F2, F3, F4, F5]

2.1 Take the weight to be the indicator of $\{u\in J\}$ on the interior. It is measurable because $u$ is continuous and $J$ is Borel. Its restriction to the fiber at $t$ is one when $t\in J$ and zero otherwise. For $t\in I$ the fiber has no boundary points, and the boundary has zero volume, so the resulting equality is exactly the displayed band identity on $R$. If $u$ is smooth on compact $R$, its gradient is bounded; integrating its derivative along curves shows that it is Lipschitz for the intrinsic length distance on each component, so the same application proves the smooth case. [given, F1, F4, step 1.1] ∎

## External input

The cited Riemannian coarea theorem applies to Lipschitz maps between $C^1$ Riemannian manifolds and expresses the integral of their metric Jacobian as the integral of normalized Hausdorff measures of fibers. Its weighted corollary gives the same identity for nonnegative measurable weights; its proof uses monotone convergence. The source input is used only on the boundaryless interior, while the boundary treatment and identification of the scalar Jacobian are supplied by the local dependencies.
