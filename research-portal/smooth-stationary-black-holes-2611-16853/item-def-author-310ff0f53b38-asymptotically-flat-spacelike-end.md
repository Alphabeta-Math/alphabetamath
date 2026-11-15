---
title: Asymptotically flat spacelike end and derivative decay
status: draft
research_item: def-author-310ff0f53b38-asymptotically-flat-spacelike-end
dependency_level: 0
---

## Prerequisites

- [physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects)
- [physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets](https://alphabetamath.cc/physics/item/def-gr-spacelike-hypersurfaces-and-cauchy-sets)
- [physics:def-gr-metric-selected-connection](https://alphabetamath.cc/physics/item/def-gr-metric-selected-connection)
- [physics:lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form](https://alphabetamath.cc/physics/item/lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form)
- [math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds](https://alphabetamath.cc/item/def-diffeomorphism-and-local-diffeomorphism-of-manifolds)
- [math:def-directional-and-partial-derivatives](https://alphabetamath.cc/item/def-directional-and-partial-derivatives)


## Definition

Let $(M,g,N)$ be a time-oriented smooth Lorentzian four-manifold of signature $(-,+,+,+)$. An end chart consists, for a specified $R>0$, of a spacelike embedded hypersurface $S_{\rm ext}\subset M$ without manifold boundary and a specified diffeomorphism from the open exterior $\{x\in\mathbb R^3:|x|>R\}$ onto $S_{\rm ext}$. A finite-radius boundary sphere, if supplied as additional data, is omitted from this chart. All estimates concern $r=|x|\to\infty$ and are unchanged on restriction to $r>R'$ for any $R'>R$. Let $n$ be its unique smooth future unit normal, $\gamma=g|_{TS_{\rm ext}}$ its induced metric, and $k(v,w)=-g(\nabla^g_vn,w)$ its second fundamental form, with the tangential covariant derivative defined independently of smooth local extensions. The sign of $k$ is fixed here; reversing it does not change the decay condition.

For a scalar chart component $f$ and integer $m\ge0$, write $f=O_m(r^{-b})$ if for each multi-index $\beta=(\beta_1,\beta_2,\beta_3)$ with $|\beta|=\beta_1+\beta_2+\beta_3\le m$ there are $C_\beta,R_\beta$ such that $|\partial_x^\beta f(x)|\le C_\beta r^{-b-|\beta|}$ for $r\ge R_\beta$. Here $\partial_x^\beta=\partial_{x^1}^{\beta_1}\partial_{x^2}^{\beta_2}\partial_{x^3}^{\beta_3}$; tensor estimates apply componentwise in this specified chart. Call these end data asymptotically flat when, for some $\alpha>0$ and integer $m\ge2$, $\gamma_{ij}-\delta_{ij}=O_m(r^{-\alpha})$ and $k_{ij}=O_{m-1}(r^{-1-\alpha})$, for $1\le i,j\le3$. The chart and parameters are witnesses to this existential condition; no invariance under arbitrary changes of chart is asserted.

## Definition references

[physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects)

[physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets](https://alphabetamath.cc/physics/item/def-gr-spacelike-hypersurfaces-and-cauchy-sets)

[physics:def-gr-metric-selected-connection](https://alphabetamath.cc/physics/item/def-gr-metric-selected-connection)

[physics:lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form](https://alphabetamath.cc/physics/item/lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form)

[math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds](https://alphabetamath.cc/item/def-diffeomorphism-and-local-diffeomorphism-of-manifolds)

[math:def-directional-and-partial-derivatives](https://alphabetamath.cc/item/def-directional-and-partial-derivatives)

## Facts & Assumptions

[F1] The metric, spacelike induced geometry and metric-selected connection have their library meanings. [physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects) [physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets](https://alphabetamath.cc/physics/item/def-gr-spacelike-hypersurfaces-and-cauchy-sets) [physics:def-gr-metric-selected-connection](https://alphabetamath.cc/physics/item/def-gr-metric-selected-connection)

[F2] On a spacelike embedded hypersurface without boundary, the future unit normal is unique and smooth, its tangential covariant derivative is independent of local extensions, and the induced metric and second fundamental form are smooth. The supplier uses $K(v,w)=g(\nabla^g_vn,w)$, so the convention here is $k=-K$. [physics:lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form](https://alphabetamath.cc/physics/item/lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form)

[F3] A diffeomorphism between smooth manifolds is a bijective smooth map with smooth inverse. [math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds](https://alphabetamath.cc/item/def-diffeomorphism-and-local-diffeomorphism-of-manifolds)

[F4] For a scalar function on an open subset of $\mathbb R^3$, $\partial_{x^j}f(x)$ is the directional derivative along the $j$th standard basis vector, defined by the derivative at $t=0$ of $t\mapsto f(x+te_j)$ when it exists. [math:def-directional-and-partial-derivatives](https://alphabetamath.cc/item/def-directional-and-partial-derivatives)

## Justification

**Given:** The objects and specified data in the Definition.

**Goal:** Verify that the displayed conditions define unambiguous objects and predicates on these data.

1.1 The open exterior chart and the spacelike embedded hypersurface satisfy the boundaryless hypotheses of [F2]. That supplier gives the unique smooth normal and extension-independent tangential covariant derivative. It also gives smooth induced metric and second fundamental form; taking $k=-K$ preserves smoothness. By [F3] the inverse of the specified diffeomorphism is a smooth coordinate chart on $S_{\rm ext}$. Thus $\gamma_{ij}$ and $k_{ij}$ are well-defined smooth scalar functions in this chart and admit all the iterated coordinate partial derivatives of [F4] used below. [F1, F2, F3, F4]

2.1 For each of finitely many derivatives at each fixed $m$, the displayed inequality is a definite bound on a scalar function outside a sufficiently large ball. Quantifying over their constants, and then over $\alpha$ and $m$, gives the claimed predicate. Replacing $k$ by $-k$ leaves every absolute value unchanged. Restricting to $r>R'$ preserves the bounds after increasing each threshold radius above $R'$; conversely, bounds on that restricted chart already give the required bounds for all sufficiently large $r$ in the original chart. Hence omitting a separately supplied finite-radius boundary sphere has no effect on this decay predicate. [F1, F2, F4, step 1.1] ∎
