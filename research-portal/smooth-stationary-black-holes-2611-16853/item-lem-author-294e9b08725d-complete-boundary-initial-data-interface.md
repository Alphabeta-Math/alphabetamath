---
title: Complete boundary initial-data and vanishing momentum interface
status: published
research_item: lem-author-294e9b08725d-complete-boundary-initial-data-interface
dependency_level: 5
sources:
  references: []
---

## Prerequisites

- [lem-author-a4a441da4986-exact-outer-cauchy-section](item-lem-author-a4a441da4986-exact-outer-cauchy-section)
- [lem-author-294e9b08725d-vacuum-section-dominant-energy](item-lem-author-294e9b08725d-vacuum-section-dominant-energy)
- [lem-author-294e9b08725d-stationary-end-extrinsic-decay](item-lem-author-294e9b08725d-stationary-end-extrinsic-decay)
- [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)
- [def-author-cea8e61dc3c6-kerr-asymptotic-charge-conventions](item-def-author-cea8e61dc3c6-kerr-asymptotic-charge-conventions)
- [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)
- [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)
- [math:def-holder-spaces-c-k-alpha-and-their-scaled-norms](https://alphabetamath.cc/item/def-holder-spaces-c-k-alpha-and-their-scaled-norms)
- [math:thm-mean-value-inequality-for-total-derivatives](https://alphabetamath.cc/item/thm-mean-value-inequality-for-total-derivatives)


## Statement

Under the regular stationary-vacuum hypotheses, the section $\overline C=C\cup S$ is a complete smooth three-dimensional initial-data manifold with nonempty compact boundary and one Euclidean end. It satisfies $h_{ij}=\delta_{ij}+O_2(r^{-1})$, $k=O_1(r^{-3})$, $\mu=J=0$, and $\operatorname{tr}_h k=O(r^{-3})$. These imply local $C^{2,\alpha}\times C^{1,\alpha}$ regularity for any $0<\alpha<1$, the usual asymptotic-flat initial-data bounds with any $1/2<q\le1$, and vanishing ADM linear momentum. These are initial-data properties independent of maximality.

Use the induced tensors $h=g|_{T\overline C}$ and $k(U,V)=-g(\nabla_U n,V)$ with the future unit normal $n$. Local Hölder regularity is componentwise on relatively compact smaller coordinate balls in the interior and on smaller boundary half-balls, with the derivatives extending continuously to the flat boundary; it asserts no uniform Hölder norm over the entire noncompact manifold.

## Facts & Assumptions

[F1] Completeness includes the smooth boundary and there is exactly one asymptotically Euclidean end. [lem-author-a4a441da4986-exact-outer-cauchy-section](item-lem-author-a4a441da4986-exact-outer-cauchy-section)

[F2] The vacuum constraint densities vanish and are norm integrable, including with the supplied boundary convention. [lem-author-294e9b08725d-vacuum-section-dominant-energy](item-lem-author-294e9b08725d-vacuum-section-dominant-energy)

[F3] The induced end metric and extrinsic curvature obey the displayed differentiated estimates. [lem-author-294e9b08725d-stationary-end-extrinsic-decay](item-lem-author-294e9b08725d-stationary-end-extrinsic-decay) [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)

[F4] The regular stationary-vacuum hypotheses specify the smooth ambient metric, the spacelike section $\Sigma_0$, its end chart and $C=\Sigma_0\cap\mathcal E$. [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)

[F5] The induced metric $h$, the future unit normal $n$, and $k(U,V)=-g(\nabla_U n,V)$ are smooth on the original spacelike section; the boundary convention includes the smooth induced metric at $S$. [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[F6] The local $C^{m,\alpha}$ classes use Hölder seminorms of the order-$m$ derivatives on relatively compact sets; the boundary-extension class also requires continuous extension of derivatives to the boundary. [math:def-holder-spaces-c-k-alpha-and-their-scaled-norms](https://alphabetamath.cc/item/def-holder-spaces-c-k-alpha-and-their-scaled-norms)

[F7] The ADM momentum uses the outward $h$-unit sphere normal and induced area measure; changing the overall second-fundamental-form sign reverses momentum but preserves its vanishing. [def-author-cea8e61dc3c6-kerr-asymptotic-charge-conventions](item-def-author-cea8e61dc3c6-kerr-asymptotic-charge-conventions)

[F8] On a convex open subset of Euclidean space, a totally differentiable map whose total derivative has operator norm at most $L$ satisfies $|f(x)-f(y)|\le L|x-y|$. [math:thm-mean-value-inequality-for-total-derivatives](https://alphabetamath.cc/item/thm-mean-value-inequality-for-total-derivatives)

## Proof

**Given:** The regular stationary-vacuum hypotheses and the supplied interfaces [F1]–[F8].

**Goal:** Establish the initial-data, local regularity, decay and zero-momentum conclusions without maximality.

1.1 The geometric, completeness and boundary assertions follow from [F1] under the hypotheses of [F4]. By [F5], $h$ and $k$ are restrictions of smooth tensors on $\Sigma_0$, also across $S$. In a smaller ball or flattened boundary half-ball whose closure lies in a smooth chart, component derivatives through order three for $h$ and order two for $k$ are bounded. Apply [F8] to each second component derivative of $h$ and each first component derivative of $k$ on the open ball, or on the convex open interior of the half-ball. The bounded next derivatives give a finite common operator-norm bound $L$, so the differences are at most $L|x-y|$. On a boundary half-ball, continuity of these derivatives extends the same inequality to pairs on the flat boundary by taking interior limits. For $0<\alpha<1$ this is at most $L D^{1-\alpha}|x-y|^\alpha$, where $D$ is the finite diameter. Smoothness gives the continuous boundary extensions, proving the local classes of [F6]. The end estimates of [F3] imply $h-\delta=O_2(r^{-q})$ and $k=O_1(r^{-1-q})$ for every $1/2<q\le1$, and contraction with $h^{-1}=\delta+O(r^{-1})$ gives $\operatorname{tr}_h k=O(r^{-3})$. The zero densities are integrable by [F2]. [F1, F2, F3, F4, F5, F6, F8, algebra]

2.1 In the ADM momentum flux $P_i=(8\pi)^{-1}\lim_{r\to\infty}\int_{S_r}(k_{ij}-(\operatorname{tr}_h k)h_{ij})\nu_h^j\,dA_h$ from [F7], the tensor factor is $O(r^{-3})$ by [F3]. The metric bound $h=\delta+O(r^{-1})$ makes the Cartesian components of $\nu_h$ bounded and the sphere area $O(r^2)$. Thus the absolute value of each flux is $O(r^{-1})$ and tends to zero. The convention in [F7] uses $K=-k$, which reverses that flux and still yields zero. [F3, F7, algebra] ∎
